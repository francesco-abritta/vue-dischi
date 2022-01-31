<template>
    <div class="items">
        <div v-for="(elemento, indice) in cards" :key="indice" class="card">
            <div class="image"><img src="cards.poster" alt=""></div>
            <div class="title">{{cards.title}}</div>
            <div class="author">{{cards.author}}</div>
            <div class="year">{{cards.year}}</div>
        </div>
    </div>
    
</template>

<script>
import axios from "axios";
export default {
    name: 'Card',
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

<style>
    .items{
        display: flex;
        flex-wrap: wrap;
        max-width: 1000px;
    }

    .card{
        height: 300px;
        width: 170px;
        padding: 10px;
        text-align: center;
        margin: 0px 25px 15px 0px;
        background-color: #2D3A46;
    }

    .title{
        color: white;
        text-transform: uppercase;
        font-style: bold;
        margin: 15px 0;
        font-size: 20px;
    }

    .author, .year{
        color: #7A776F;
        font-size: 15px;
    }
</style>