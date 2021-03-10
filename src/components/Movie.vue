<template>
<div class="movie" @click="setActiveMovie">
  <div class="media">
    <img src="" alt="">

  </div>

</div>
</template>

<script>
export default {
  name: 'movie',
  props: {
    msg: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
