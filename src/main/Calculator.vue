<template>
  <div class="calculator">
      <Display value="1000"/>
      <Button label="AC" triple @onCalc="clearMemory"/>
      <Button label="/" operation @onCalc="setOperation"/>
      <Button label="7" @onCalc="addDigit"/>
      <Button label="8" @onCalc="addDigit"/>
      <Button label="9" @onCalc="addDigit"/>
      <Button label="*" operation @onCalc="setOperation"/>
      <Button label="4" @onCalc="addDigit"/>
      <Button label="5" @onCalc="addDigit"/>
      <Button label="6" @onCalc="addDigit"/>
      <Button label="-" operation @onCalc="setOperation"/>
      <Button label="1" @onCalc="addDigit"/>
      <Button label="2" @onCalc="addDigit"/>
      <Button label="3" @onCalc="addDigit"/>
      <Button label="+" operation @onCalc="setOperation"/>
      <Button label="0" double @onCalc="addDigit"/>
      <Button label="." @onCalc="addDigit"/>
      <Button label="=" operation @onCalc="setOperation"/>
      
     
  </div>
</template>

<script>
import Display from "../components/Display"
import Button from "../components/Button"

export default {
components: { Button, Display },
methods: {
  clearMemory(){
    console.log('Limpar Memória!')
  },
  setOperation(operation) {
    console.log('Operação ' + operation)
  },
  addDigit(n) {
    console.log('Digito ' + n)
  },
}
}
</script>

<style>
.calculator {
    width: 235px;
    height: 320px;
    border-radius: 5px;
    overflow: hidden;

    display: grid;
    grid-template-columns: repeat(4, 25%);
    grid-template-rows: 1fr 48px 48px 48px 48px 48px;
}

</style>