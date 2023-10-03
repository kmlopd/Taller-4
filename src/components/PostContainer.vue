<template>
     <div class="post-container">
        <h1>THE FLASH SERIE</h1>
        <post-div/>
    </div>
</template>

<script lang="ts">
    import { computed, defineComponent, DefineComponent } from 'vue';
    import PostDiv from './PostDiv.vue';
    //import Datos2 from "@/assets/posts2.json";

    export default defineComponent({
        name: "PostContainer",
        components: {
            PostDiv,
        }
    })
</script>

<style lang="scss" scoped>

body{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-content: center;
}
.post-container {
    width: 95%;
    height: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    /*background-image: linear-gradient(45deg, lightblue 12%, blue 180%);*/
    /*background-image: linear-gradient(140deg, #262B39,#323847);*/
    background-image:linear-gradient(45deg, #21D4FD 0%, #B721FF 108%);
    flex-direction: column;
    align-content: center;
    padding: 8px 15px;
    align-items: center;
    border-radius: 35px;
}
</style>