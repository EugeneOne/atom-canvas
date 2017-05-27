<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <myCanvas :dotsNum="dotsNum" :isColor="false"></myCanvas>
  </div>
</template>

<script>
import myCanvas from './canvas'
export default {
  name: 'hello',
  components: {
    myCanvas
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      dotsNum: 60,
      roundColor: "red",
      lineColor: ""
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
