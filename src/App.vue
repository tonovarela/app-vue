<template>
<div class="container">
    <div class="jumbotron">
        <button class="btn btn-primary"  @click="componenteSeleccionado='IniciarSesion'">Iniciar sesion</button>
        <button class="btn btn-primary"  @click="componenteSeleccionado='RecuperarClave'">Recuperar contraseña</button>
        <keep-alive>
       <component :is="componenteSeleccionado"></component>
        </keep-alive>
    </div>
</div>
</template>

<script>

import IniciarSesion     from './Componentes/iniciarSesionComponent';
import RecuperarClave    from './Componentes/recuperarClaveComponent';
export default {

    components: {
    
       IniciarSesion: IniciarSesion,
       RecuperarClave: RecuperarClave
    },
    data(){
        return {
            componenteSeleccionado:'IniciarSesion'
        }
    }
}
</script>

<style scoped>
h3{
    color:red;
}
