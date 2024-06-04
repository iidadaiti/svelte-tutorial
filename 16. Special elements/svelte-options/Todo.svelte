<svelte:options immutable />

<script>
  import { afterUpdate } from "svelte";
  import flash from "./flash.js";

  export let todo;

  let button;

  afterUpdate(() => {
    flash(button);
  });
</script>

<button bind:this={button} type="button" on:click>
  {todo.done ? "👍" : ""}
  {todo.text}
</button>

<style>
  button {
    all: unset;
    display: block;
    cursor: pointer;
    line-height: 1.5;
  }
</style>
