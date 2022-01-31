<template>
  <div>
      <div class="header">
          <img src="../assets/img/logo-small.svg" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style scoped>
    .header{
        height: 60px;
        background-color: #2D3A46;
        display: flex;
        align-items: center;
    }

    img{
        height: 40px;
        padding-left: 20px;
    }
</style>