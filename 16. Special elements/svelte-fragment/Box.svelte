<div class="box">
	<slot name="header">No header was provided</slot>
	<p>Some content between header and footer</p>
	<slot name="footer" />
</div>

<style>
	.box {
		display: flex;
		flex-direction: column;
		gap: 1em;
	}
</style>
