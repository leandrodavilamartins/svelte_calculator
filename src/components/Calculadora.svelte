<script>
  import Botao from "./Botao.svelte";
  import Linha from "./Linha.svelte";
  import Tela from "./Tela.svelte";

  let valor = "";

  let writeValue = (event) => {
    console.log(event.target.textContent);
  };
</script>

<div class="calculadora">
  <Linha>
    <Tela value={valor} />
  </Linha>
  <Linha>
    <Botao texto="AC" triplo destaque />
    <Botao texto="x" operacao />
  </Linha>
  <Linha>
    <Botao texto="1" on:click={writeValue} />
    <Botao texto="2" />
    <Botao texto="3" />
    <Botao texto="+" operacao />
  </Linha>
  <Linha>
    <Botao texto="4" />
    <Botao texto="5" />
    <Botao texto="6" />
    <Botao texto="-" operacao />
  </Linha>
  <Linha>
    <Botao texto="7" />
    <Botao texto="8" />
    <Botao texto="9" />
    <Botao texto="/" operacao />
  </Linha>
  <Linha>
    <Botao texto="." />
    <Botao texto="0" />
    <Botao texto="=" duplo operacao />
  </Linha>
</div>

<style>
  .calculadora {
    background-color: var(--cor-fundo);
    display: flex;
    flex-direction: column;
    width: 400px;
    align-content: space-between;
    height: 60vh;
    padding: 0.5em;
    border-radius: 0.5em;
  }
</style>
