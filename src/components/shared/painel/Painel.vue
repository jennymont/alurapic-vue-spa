<template>
  <div class="painel">
    <h2 class="painel-titulo">{{ titulo }}</h2>

    <slot class="painel-conteudo"></slot>
    <button class="alterar">Alterar</button>
    <button class="remover">Remover</button>
  </div>
</template>

<script>
export default {
    props: ['titulo']
};
</script>

<style scoped>
.painel {
    padding: 0 auto;
    border: solid 2px grey;
    display: inline-block;
    margin: 5px;
    box-shadow: 5px 5px 10px grey;
    width: 200px;
    height: 100%;
    vertical-align: top;
    text-align: center;
  }

  .painel .painel-titulo {
    text-align: center;
    border: solid 2px;
    background: lightblue;
    margin: 0 0 15px 0;
    padding: 10px;
    text-transform: uppercase;
  }
  .alterar{
    background-color: yellow;
    font-size: 15px;
    font-weight: bold;
  }
  .remover{
    background-color: red;
    font-size: 15px;
    font-weight: bold;
  }

 *{
      box-shadow: 5px 5px 0px black;
  }

</style>