<script>
  export let value = "";
</script>

<div class="tela">
  <span id="valor">{value}</span>
</div>

<style>
  .tela {
    flex-basis: 100%;
    background-color: aliceblue;
    margin-bottom: 0.5em;
    padding: 0.5em;
  }

  #valor {
    display: flex;
    justify-content: end;
    font-size: 32px;
    font-family: "Orbitron", sans-serif;
  }
</style>
