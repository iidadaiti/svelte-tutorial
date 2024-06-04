<script>
  import { onInterval } from "./utils.js";
  import { onDestroy } from "svelte";

  let counter = 0;
  let interval = 1000;
  export let callback;

  onInterval(callback, interval);
</script>

<p>
  This component executes a callback every
  {interval} millisecond{interval === 1 ? "" : "s"}
</p>

<style>
  p {
    border: 1px solid blue;
    padding: 5px;
  }
</style>
