<template>
    <div class="post-link">
        <h3>{{ tittle }}</h3>
        <p>
            {{ resumen }}
        </p>
        <a :href="link" >
            <img :src="url" alt="/">
            Sinopsis Season
        </a>
        
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
        link: {
            type: String,
             default: ""
        },
        url: {
            type:String ,
            default:""
        }
    }
})
</script>

<style lang="scss" scoped>
.post-link{
    display: flex;
    flex-direction: column;
    background-color: blueviolet;
    margin-bottom: 18px;
    border-radius: 30px;
}

p {
    text-align: justify;
    padding-left: 20px;
    padding-right: 8px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 20px;
    color: white;
}

h3 {
    text-align: center;
    font-family: 'Times New Roman', Times, serif;
    color: rgb(36, 0, 215);
}

a {
    width: 40%;
    padding-bottom: 8px;
    padding-left: 25px;
    color: violet;
    font-family: 'Times New Roman', Times, serif;
    font-size: 20px;
}

a:hover {
    color: blue;
    font-size: 24px;
 }

 img {
    width: 20vw;
    height: 20vh;
 }
</style>