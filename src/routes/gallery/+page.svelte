<div class="gal-row p-1 p-md-5 m-0">
	<div class="gal-col px-1 px-md-3">
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

	.gal-col img{
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
</style>
