<template>
<div class="container">
    <div class="jumbotron">
        <mostrar-formulario>
            <h3 slot="titulo"> Iniciar sesión</h3>
            <div slot="elementos">
                <div class="form-group">
                    <label for="correo">Correo Electronico</label>
                    <input type="email" class="form-control" id="correo" placeholder="Escribr tu correo" />
                </div>
                <div  class="form-group">
                    <label for="clave">Contraseña</label>
                    <input type="password" class="form-control" id="clave" placeholder="Escribr tu constraseña" />
                </div>
            </div>
        <button slot="boton" class="btn btn-primary">Iniciar sesión</button>
        </mostrar-formulario>
    </div>
</div>
</template>

<script>
import MostrarFormulario from './mostrarFormularioComponent';
export default {

    components: {
        MostrarFormulario
    },
    destroyed(){
        console.log("Se esta destruyendo");
    },
    activated(){
console.log("Activado");
    },
    deactivated(){
console.log("Desactivado");
    }
}
</script>

<style scoped>
h3{
    color:red;
}
