<template>
  <div id="app">
      <!--    <Demo></Demo>-->
      <Layout></Layout>
  </div>
</template>

<script>
    // import Demo from './components/Demo.vue'
    import Layout from "./components/Layout";

    export default {
        name: 'app',
        components: {
            // Demo,
            Layout
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
