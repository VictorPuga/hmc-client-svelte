<script>
  import { Button, Input } from "../components";
  function print() {
    console.log("hey");
  }
</script>

<h1>Hola</h1>
<Button title="hey" variant="primary" on:click={print} />
<Button title="hey" variant="ghost" href="/hey" />
<Input placeholder="hey" onEnter={console.log} />
