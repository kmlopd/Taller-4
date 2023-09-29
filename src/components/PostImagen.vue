<template>
    <div class="post-imagen">
        <div class="imag">
            <img src="https://imgsrc.cineserie.com/2016/08/2138202.jpg?ver=1" alt="/" />
            <a href="https://el-diario-de-yuuki.blogspot.com/2016/09/the-flash-temporada-1-resena-de-serie.html">Ver Mas...</a>
        </div>
        <div class="imag">
            <img src="https://cl.buscafs.com/www.tomatazos.com/public/uploads/images/63963/63963_173x260.jpg" alt="/" />
            <a href="https://el-diario-de-yuuki.blogspot.com/2016/10/the-flash-temporada-2-resena-de-serie.html">Ver Mas...</a>
        </div>
        <div class="imag">
            <img src="https://pm1.aminoapps.com/6445/586b7bb4423e7c4f7ff4a91cbae62865ac762ee6_hq.jpg" alt="/" />
            <a href="https://es.ign.com/the-flash-cw/118886/news/the-flash-analisis-de-la-tercera-temporada">Ver Mas...</a>
        </div>
        <div class="imag">
            <img src="https://www.formulatv.com/images/series/posters/800/834/dest_1.jpg" alt="/" />
            <a href="https://www.cineycine.com/series/the-flash-temporada-4/">Ver Mas...</a>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent, DefineComponent } from 'vue';
import PostLink from './PostLink.vue';

export default defineComponent({
    name: "PostImagen",
    components: {
        PostLink
    },
})
</script>

<style lang="scss" scoped>
 .post-imagen {
    display: flex;
 }
.imag {
    padding-right: 4px;
}
 img {
    width: 22vw;
    height: 60vh;
 }

 a{
    color: purple;
    font-size: 20px;
 }
</style>