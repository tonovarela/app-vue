<template>
<div class="container">
    <div class="jumbotron">
        <mostrar-formulario>
            <h3 slot="titulo"> Recuperar contraseña</h3>
            <div slot="elementos">
                <div class="form-group">
                    <label for="correo">Correo Electronico</label>
                    <input type="email" class="form-control" id="correo" placeholder="Escribr tu correo" />
                </div>
            </div>
        <button slot="boton" class="btn btn-primary">Recuperar</button>
        </mostrar-formulario>
    </div>
</div>
</template>

<script>
import MostrarFormulario from './mostrarFormularioComponent';
export default {

    components: {
        MostrarFormulario
    }
}
</script>

<style scoped>
h3{
    color:red;
}
