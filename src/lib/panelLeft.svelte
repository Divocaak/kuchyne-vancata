<script>
	export let imgPath;
	export let height = 'auto';
</script>

<div class="m-0" style="--height: {height}">
	<div class="p-5 color-dark">
		<slot></slot>
	</div>
	<img src={imgPath} alt={imgPath} />
</div>

<style>
	:root {
		--fade-position: 75%;
		--height: auto;
	}

	div {
		position: relative;
		min-height: 50vh;
		height: var(--height);
		overflow: hidden;
	}

	div div {
		position: absolute;
		left: 0;
		height: 100%;
		width: var(--fade-position);
		z-index: 2;
		background: linear-gradient(
			90deg,
			var(--light) var(--fade-position),
			rgba(255, 255, 255, 0) 100%
		);
	}

	div img {
		position: absolute;
		right: 0;
		z-index: 1;
		min-width: calc(100% - var(--fade-position));
		height: 100%;
	}

	@media (max-width: 768px) {
		div{
			height: auto;
		}

		div div {
			position: relative;
			height: 100%;
			width: 100%;
			z-index: 2;
			background: var(--light);
		}

		div img {
			position: relative;
			z-index: 1;
			min-width: calc(100% - var(--fade-position));
			width: 100%;
			height: 100%;
		}
	}
</style>
