<script>
import AppCard from './AppCard.vue'
import dataObjects from '../assets/data/dataobjects'

export default {
    components: {
        AppCard
    },
    data() {
        return {
            listaFumetti: dataObjects,
            dataObjects
        }
    }
}

</script>

<template lang="">
    <div class="black">
        <div class="container">
            <h1>ciao</h1>
            <div class="card-container" :v-for="(fumetto,index) in listaFumetti" :key="index">
                <img src="fumetto.thumb" alt="">
                <span>{{ fumetto.series }}</span>
            </div>
        </div>
    </div>   
</template>

<style lang="scss">
@use '../styles/partials/mixins' as *;

.black {
    background-color: #000;
    @include flex-center;

    .container {
        width: 1200px;
        @include flex-center;
        align-items: center;

        h1 {
            color: #fff;
        }
    }
}
</style>