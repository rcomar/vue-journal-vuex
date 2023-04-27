<template>

<div class="entry-title d-flex justify-content-between p-2">
    <div>
        <span class="text-success fs-3 fw-bold">26</span>
        <span class="mx-1 fs-3">Abril</span>
        <span class="mx-2 fs-4 fw-light">2023, Miercoles</span>
    </div>

    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fa fa-trash-alt"></i>
        </button>

        <button class="btn btn-primary">
            Subir foto
            <i class="fa fa-upload"></i>
        </button>
    </div>

</div>
<hr>
<div class="d-flex flex-column px-3 h75">
    <textarea placeholder="¿Qué sucedio hoy?" name="" id="" cols="30" rows="10"></textarea>    
</div>

<Fab icon="fa-save"/>

<img class="img-thumbnail" src="https://cdna.artstation.com/p/assets/images/images/024/222/768/4k/michael-oberschneider-concept-design-in-flight-pods-open-01-logo.jpg" alt="Imagen">

</template>
<script>

import { defineAsyncComponent } from "vue";

export default{
    components: {
        Fab: defineAsyncComponent(() => import('../components/FabComponent.vue'))
    }
}
</script>
<style lang="scss" scoped>
    
    textarea {
        font-size: 20px;
        border: none;
        height: 100%;

        &:focus {
            outline:none;
        }
    }
img {
    width: 200px;
    position:fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>