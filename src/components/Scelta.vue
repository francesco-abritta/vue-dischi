<template>
    <div class="select">
        <div class="scelta">Scegli:</div>
        <select name="genere" id="select">
            <option value="Tutti">Tutti</option>
            <option value="Rock">Rock</option>
            <option value="Pop">Pop</option>
            <option value="Jazz">Jazz</option>
            <option value="Metal">Metal</option>
        </select>
    </div>            
</template>

<script>
export default {

}
</script>

<style>
    .select{
        background-color: #1E2D3B;
        text-align: center;
        padding-top: 20px;
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