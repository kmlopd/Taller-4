<template>
    <div class="post-div">
        <div class="imagen">
            <img src="https://www.cinemascomics.com/wp-content/uploads/2015/09/The-Flash-promo-season-2-picset-e1451157751839.jpg.webp" alt="/">
            <img src="https://ntvb.tmsimg.com/assets/p10781465_b_h8_ay.jpg?w=960&h=540" alt="/">
        </div>
            <p>The Flash es una serie de televisión estadounidense de superhéroes desarrollada por Greg Berlanti, Andrew Kreisberg y Geoff Johns, que se emite en The CW en Estados Unidos. Está basada en el personaje de DC Comics Barry Allen / Flash, un superhéroe disfrazado que lucha contra el crimen con el poder de moverse a velocidades sobrehumanas. 
            Es una serie derivada de Arrow, que existe en el mismo universo ficticio. La serie sigue a Barry Allen, interpretado por Grant Gustin, un investigador de escenas del crimen que obtiene velocidad sobrehumana, que usa para luchar contra criminales, incluidos otros que también han adquirido habilidades sobrehumanas.
            Otros miembros del elenco de larga data han incluido a Candice Patton, Danielle Panabaker, Carlos Valdes, Tom Cavanagh y Jesse L. Martin.</p>
           <p>
            Un piloto de puerta trasera, la recepción positiva que recibió Gustin durante sus dos apariciones como Barry en Arrow llevó a los ejecutivos a elegir desarrollar un piloto completo para utilizar un presupuesto más amplio y ayudar a desarrollar el mundo de Barry con más detalle.
            La serie se filmó principalmente en Vancouver, Columbia Británica, Canadá.
           </p>
           <p>
            The Flash se estrenó en Norteamérica el 7 de octubre de 2014, donde el piloto se convirtió en el segundo estreno más visto en la historia de The CW, después de The Vampire Diaries en 2009. Ha sido bien recibida por la crítica y el público, y ganó el premio People's Choice por «Nuevo drama de televisión favorito» en 2014.
            La serie, junto con Arrow, ha lanzado personajes para su propio programa, Legends of Tomorrow, que se estrenó el 21 de enero de 2016. En marzo de 2022, la serie fue renovada para una novena y última temporada, que se estrenó el 8 de febrero de 2023.La serie finalizó el 24 de mayo de 2023.
           </p>
           <PostLink v-for="post in posts" :key="post.tittle"
                :tittle="post.tittle"
                :resumen="post.resumen"
                :link="post.link"
                :url="post.url"
            />
           <PostImagen/>
    </div>
</template>

<script lang="ts">
    import { defineComponent, DefineComponent } from 'vue';
    import PostImagen from "./PostImagen.vue";
    import PostLink from './PostLink.vue';
    import Datos from '@/assets/posts.json';

    export default defineComponent({
         name: "PostDiv",
         components: {
          PostImagen,
          PostLink
    },
    props: {
        img: {
            type: String,
            default: ""
        },
        img2: {
            type: String,
            default: ""
        }
    },
     computed: {
        posts: () => {
            return Datos.map((post: any) => {
                return post
            })
        }
    }
})
</script>

<style lang="scss" scoped>
p {
    font-family: 'Times New Roman', Times, serif;
    font-size: 25px;
    text-align: justify;
}

h2 {
    font-weight: bold;
    color: blue;
    text-align: center;
    justify-content: center;
}

.imagen {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

img {
    width: 420px;
    height: 210px;
}
</style>