<template>
  <div>
      <div class="main">
          <div class="items"></div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style>
    .main{
        height: calc(100vh - 60px);
        background-color: #1E2D3B;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .items{
        height: 300px;
        background-color: red;
    }
</style>