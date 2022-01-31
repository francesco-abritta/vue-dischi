<template>
  <div>
      <div class="main">
          <div class="items">
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
              <div class="card">
                  <div class="image"><img src="https://picsum.photos/140/140" alt=""></div>
                  <div class="title">Titolo Titolo Titolo</div>
                  <div class="author">Autore</div>
                  <div class="year">anno</div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style>
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