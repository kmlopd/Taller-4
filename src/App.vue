<template>
  <post-container />
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import PostContainer from './components/PostContainer.vue';
export default defineComponent({
  components: {
    PostContainer
  }
})
</script>

<style lang="scss">
 h1 {
  text-align: center;
 }

 body {
    display: flex;
    justify-content: center;
    background-color: lightblue;
    align-items: center;
 }
</style>
