<template>
     <div class="post-container">
        <h1>THE FLASH SERIE</h1>
        <post-div/>
    </div>
</template>

<script lang="ts">
    import { computed, defineComponent, DefineComponent } from 'vue';
    import PostDiv from './PostDiv.vue';
    //import datos from "@/assets/posts.json";

    export default defineComponent({
        name: "PostContainer",
        components: {
            PostDiv,
        },
    })
</script>

<style lang="scss" scoped>
.post-container {
    width: 95%;
    height: 100%;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    background-image: linear-gradient(45deg, lightblue 12%, blue 180%);
    flex-direction: column;
    align-content: center;
    padding: 8px 15px;
    align-items: center;
}
</style>