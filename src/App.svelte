<script>
  import Calculadora from "./components/Calculadora.svelte";
</script>

<main>
  <Calculadora />
</main>

<style>
  :global(body) {
    background-color: #151718;
  }

  :root {
    --cor-fundo: #555;
  }
  main {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
</style>
