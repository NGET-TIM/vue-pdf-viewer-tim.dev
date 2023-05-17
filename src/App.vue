<template>
  <div>
    <WebViewer :path="`${publicPath}lib`"/>
  </div>
</template>

<script>
import WebViewer from './components/WebViewer.vue'

export default {
  name: 'app',
  components: {
    WebViewer
  },
  data () {
    return {
      publicPath: "http://localhost:5173/"
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
}
</style>
