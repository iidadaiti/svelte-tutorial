<script>
	let hovering;

	function enter() {
		hovering = true;
	}

	function leave() {
		hovering = false;
	}
</script>

<div role="button" tabindex="-1" on:mouseenter={enter} on:mouseleave={leave}>
	<slot hovering={hovering} />
</div>
