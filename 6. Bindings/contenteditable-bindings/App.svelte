<script>
  let html = "<p>Write some text!</p>";
</script>

<div contenteditable="true" bind:innerHTML={html} />
<div contenteditable="true" bind:innerText={html} />
<div contenteditable="true" bind:textContent={html} />

<pre>{html}</pre>

<style>
  [contenteditable] {
    padding: 0.5em;
    border: 1px solid #eee;
    border-radius: 4px;
  }
</style>
