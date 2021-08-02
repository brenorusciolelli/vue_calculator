<template>
  <footer>
      {{ footerTemplate}}
  </footer>
</template>

<script>
export default {
    data() {
        return {
            footerTemplate: 'Desenvolvido por Breno Rusciolelli - 2021'
        }
    },
}
</script>

<style>
footer {
    position: absolute;
    bottom: 0;
    width: 100%;
    background-color: rgba(128, 128, 128, 0.513);
}
</style>