<script>
import AppCard from './AppCard.vue'
import dataObjects from '../assets/data/dataobjects.js'

export default {
    components: {
        AppCard,
        dataObjects
    },
    data() {
        return {
            listaFumetti: dataObjects

        }
    }
}

</script>

<template lang="">
    <div class="jumbotron">
        <img src="../assets/Images/jumbotron.jpg" alt="">
    </div>
    <div class="black">
        <div class="container">  
            <span class="label-blue">Current series</span>         
            <AppCard class="card-container" v-for="(fumetto,index) in listaFumetti" :key="index" :serie="fumetto"></AppCard>
        </div>
        
    </div>   
</template>

<style lang="scss">
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;

.jumbotron {
    width: 100%;
    display: flex;
    height: 400px;


    img {
        width: 100%;
        object-fit: cover;
        object-position: top;
    }
}

.black {
    background-color: #1c1c1c;
    @include flex-center;

    .container {
        width: 1200px;
        display: flex;
        align-items: flex-start;
        gap: 1rem;
        padding: 2rem 0;
        flex-wrap: wrap;
        position: relative;

        h1 {
            color: #fff;
        }

        .label-blue {
            background-color: $primary;
            color: #fff;
            padding: 0.5rem 3rem;
            font-family: $text-primary;
            font-size: 2rem;
            position: absolute;
            top: -2rem;
            left: 0;
        }
    }
}
</style>