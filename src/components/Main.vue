<template>
  <div>
        <Scelta />
        <div class="main">
            <div class="items">
                <Card v-for="(elemento, indice) in cards" :key="indice" :album="elemento"/>
            </div>
        </div>
  </div>
</template>

<script>
import Card from './Card.vue'
import Scelta from './Scelta.vue'
import axios from "axios";


export default {
    name: 'Main',
    components: {
        Card,
        Scelta
    },
    data() {
        return {
            apiURL: "https://flynn.boolean.careers/exercises/api/array/music",
            cards: [],
        }
    },
    created(){
        this.getCards();
    },
    methods: {
        getCards(){
            axios
                .get(this.apiURL)
                .then( (risposta) => {
                    // handle success
                    this.cards = risposta.data.response;
                })
                .catch(function (error) {
                    // handle error
                    console.log(error);
                });
        }
    }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap');

    .main{
        min-height: calc(100vh - 60px);
        background-color: #1E2D3B;
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: 'Roboto' , sans-serif;
    }

    .items{
        display: flex;
        flex-wrap: wrap;
        max-width: 1000px;
    }
</style>