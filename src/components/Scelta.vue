<template>
    <div class="select">
        <div class="scelta">Scegli:</div>
        <select name="genere" @change="$emit('filtra', GenereSelezionato)" v-model="GenereSelezionato">
            <option value="">Tutti</option>
            <option value="Rock">Rock</option>
            <option value="Pop">Pop</option>
            <option value="Jazz">Jazz</option>
            <option value="Metal">Metal</option>
        </select>
    </div>            
</template>

<script>
export default {
    name: "Scelta",
    data() {
        return{
            GenereSelezionato:"",
        }
    }
}
</script>

<style scoped lang="scss">
@import '../assets/var.scss';

    .select{
        background-color: $background;
        text-align: center;
        padding: 20px 0;
        display: flex;
        justify-content: center;
        font-size: 20px;
        color: white;
        font-family: 'Roboto' , sans-serif;
    }

    .scelta{
        margin-right: 10px;
    }

    select{
        background-color: #1E2D3B;
        border: 0;
        font-size: 20px;
        color: white;
        cursor: pointer;
    }
</style>