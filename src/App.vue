<template>
  <div id="app">
   <formulario />
  </div>
</template>

<script>

import formulario from "./components/Formulario.vue"
export default {
  name: 'App',
  components:{
    formulario
  }

}
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    background: rgb(255 255 255);
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
</style>
