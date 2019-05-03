<template>
  <div id="app">
    <p> {{ sayHello() }} - <a v-bind:href="link">Google</a> </p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      title: 'Hello World!',
      alternateTitle: 'Hello Manó!',
      link: 'http://google.com'
    }
  },
  methods: {
    sayHello: function () {
      return this.title
    },
    changeTitle: function () {
      return this.alternateTitle
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
