<script>
  export let texto = "";
  export let duplo = false;
  export let triplo = false;
  export let operacao = false;
  export let destaque = false;
</script>

<button
  class="botao"
  class:duplo
  class:triplo
  class:operacao
  class:destaque
  on:click
>
  {texto}
</button>

<style>
  .botao {
    flex-basis: 25%;
    margin: 0;
    font-size: 2.2rem;
    font-family: "Orbitron", sans-serif;
  }
  .duplo {
    flex-basis: 50%;
  }
  .triplo {
    flex-basis: 75%;
  }
  .operacao {
    background-color: #ff3e00;
    color: #ffffff;
  }
  .destaque {
    background-color: yellow;
  }
</style>
