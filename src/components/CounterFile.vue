<template>
    <div class="text-center">
    <h1 style="margin-block-end: 5px;">{{ counter }}</h1>
    <button @click="incremento" style="margin-bottom:10px;"> increment </button>
    <button @click="reset" style="margin-top:10px;"> reset </button>

    </div>
    <div>
    <img :src="require('../assets/img/mojabi.jpg')" alt="mojabi" style="width: 500px; height: auto;">
    </div>
</template>

<script>

    import { ref } from'vue';

    export default{
    setup() {
        const counter= ref(0);
        return{counter};
    },

    methods: {
        incremento(){
            this.counter++;
        },

        reset(){
            this.counter = 0;
        }
    }
    }
</script>

<style>

.content-center {
    display: flex;
    flex-direction: column;
    align-items: center; 
    justify-content: center;
    height: 220px;
    text-align: center;
}
</style>