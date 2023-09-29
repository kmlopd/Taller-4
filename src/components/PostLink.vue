<template>
    <div class="post-link">
        <h3>{{ tittle }}</h3>
        <p>
            {{ resumen }}
        </p>
    </div>
</template>

<script lang="ts">
 import { defineComponent, DefineComponent } from 'vue';

export default defineComponent({
    name: "PostLink",
     props: {
        tittle: {
            type: String,
            default: ""
        },
        resumen: {
            type: String,
            default: ""
        },
    }
})
</script>

<style lang="scss" scoped>
.post-link{
    display: flex;
    flex-direction: column;
}
</style>