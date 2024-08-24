<div class="gal-row p-1 p-md-5">
	<div class="gal-col px-1 px-md-3">
		<video class="mb-1 mb-md-4" autoplay muted controls loop preload>
			<source src="/vids/0.mp4" type="video/mp4" />
			Your browser does not support the video tag.
		</video>
		<img src="/pics/0.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/1.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/4.jpg" alt="gallery element" class="mb-1 mb-md-4" />
	</div>
	<div class="gal-col px-1 px-md-3">
		<img src="/pics/2.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/3.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/5.jpg" alt="gallery element" class="mb-1 mb-md-4" />
	</div>
	<div class="gal-col px-1 px-md-3">
		<img src="/pics/6.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/8.jpg" alt="gallery element" class="mb-1 mb-md-4" />
		<img src="/pics/7.jpg" alt="gallery element" class="mb-1 mb-md-4" />
	</div>
</div>

<style>
	.gal-row,
	.gal-col {
		box-sizing: border-box;
	}

	.gal-row {
		display: flex;
		flex-wrap: wrap;
		background-color: var(--light);
	}

	.gal-col {
		flex: 33%;
		max-width: 33%;
	}

	.gal-col img,
	video {
		position: relative;
		width: 100%;
		vertical-align: middle;
	}

	@media (max-width: 768px) {
		.gal-col {
			flex: 50%;
			max-width: 50%;
		}
	}

	/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
	@media (max-width: 600px) {
		.column {
			flex: 100%;
			max-width: 100%;
		}
	}
</style>
