<script>
	let className;
	export { className as class };
</script>

<style>
	.bg-fullbleed {
		max-width: none !important;
		width: 100vw;

		position: relative;
		left: 50%;
		transform: translate(-50vw);
	}

	[class*="max-w"].bg-fullbleed {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

	[class*="max-w"].bg-fullbleed > .wrapper {
		max-width: var(--max-width);
		display: block;
		box-sizing: content-box;
		width: 100vw;
		flex-shrink: 0;
		flex-basis: 100%;
	}
</style>

<div class="{className}">
	<div class="wrapper">
		<slot></slot>
	</div>
</div>
