<template>
  <div>
      <div class="main">
            <Card />
      </div>
  </div>
</template>

<script>
import Card from './_Card.vue'

export default {
    name: 'Main',
    components: {
        Card
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
</style>