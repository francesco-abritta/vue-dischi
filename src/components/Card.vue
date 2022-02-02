<template>
    <div class="card">
        <div class="image"><img :src="album.poster" alt=""></div>
        <div class="title">{{album.title}}</div>
        <div class="author">{{album.author}}</div>
        <div class="year">{{album.year}}</div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        album: Object
    }
}
</script>

<style scoped lang="scss">
    

    .card{
        height: 300px;
        width: 170px;
        padding: 20px;
        text-align: center;
        margin: 0px 25px 15px 0px;
        background-color: #2D3A46;

        img{
            height: 130px;
            width: 130px;
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
    }

    
</style>