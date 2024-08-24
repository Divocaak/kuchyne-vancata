<script>
	export let imgPath;
	export let height = 'auto';
</script>

<div style="--height: {height}">
	<img src={imgPath} alt={imgPath} />
	<div class="color-dark">
		<div>
			<slot></slot>
		</div>
	</div>
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
		right: 0;
		height: 100%;
		width: var(--fade-position);
		z-index: 2;
		background: linear-gradient(
			-90deg,
			var(--semi) var(--fade-position),
			rgba(255, 255, 255, 0) 100%
		);
	}

	div img {
		position: absolute;
		left: 0;
		z-index: 1;
		min-width: calc(100% - var(--fade-position));
		height: 100%;
	}

	@media (max-width: 768px) {
		div div {
			position: relative;
			height: 100%;
			width: 100%;
			z-index: 2;
			background: var(--semi);
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
