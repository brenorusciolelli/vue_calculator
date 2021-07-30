<template>
  <div id="app">
    <h1>Calculadora</h1>
    <Calculator />
  </div>
</template>

<script>
import Calculator from "./main/Calculator"

export default {
  components: { Calculator }
}
</script>

<style>
@font-face {
  font-family: "RobotoMono";
  src: url("./fonts/RobotoMono-Bold.ttf");
}

*{
  font-family: "RobotoMono", monospace;
}

body{
  margin: 0;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;

  color: #fff;
  background: linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(80,38,153,1) 39%, rgba(102,0,255,1) 96%);
  
}
</style>