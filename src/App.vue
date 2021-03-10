<template>
  <div class= "app">
    <header>
      <div class="container-fluid bg-primary text-light">
       <div class="row">
         <div class="col text-center">
            <h1> Welcome to the Vue Movie Search</h1>
         </div>
        </div>
      </div>
    </header>
  <main class="container">
    <div class="row">
      <div class="col">
        <form @submit.prevent="search">
          <input class="mx-1"  type="text" placeholder="Movie Title?" >
          <button type="submit" class="btn btn-outline-success">Search</button>
        </form>
      </div>
    </div>
    <div class="row">
      <div class="col-6">
        <MovieResults />
      </div>
      <div class="col-6">
        <MovieDetails />
      </div>
    </div>
  </main>
  <footer>
    <div>Made by GEo</div>
  </footer>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
