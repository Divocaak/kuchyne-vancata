<svelte:head>
	<link
		href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
		rel="stylesheet"
		integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
		crossorigin="anonymous"
	/>
	<script
		src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
		integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
		crossorigin="anonymous"
	></script>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@300&display=swap"
		rel="stylesheet"
	/>
	<link href="https://fonts.googleapis.com/css2?family=Noto+Sans&display=swap" rel="stylesheet" />
	<link
		href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@500&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<nav class="navbar navbar-expand-lg bg-body-tertiary">
	<div class="container-fluid">
		<span class="navbar-brand mb-0 h1">LOGO</span>
		<button
			class="navbar-toggler"
			type="button"
			data-bs-toggle="collapse"
			data-bs-target="#navbarSupportedContent"
			aria-controls="navbarSupportedContent"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
			<span class="navbar-toggler-icon"></span>
		</button>
		<div class="collapse navbar-collapse" id="navbarSupportedContent">
			<ul class="navbar-nav me-auto mb-2 mb-lg-0">
				<li class="nav-item">
					<a class="nav-link noto-sans-regular" aria-current="page" href="/">Úvod</a>
				</li>
				<li class="nav-item">
					<a class="nav-link noto-sans-regular" href="/flow">Co vás čeká?</a>
				</li>
				<li class="nav-item">
					<a class="nav-link noto-sans-regular" href="/projects">Realizace</a>
				</li>
				<li class="nav-item">
					<a class="nav-link noto-sans-regular" href="/about">O mně</a>
				</li>
				<li class="nav-item">
					<a class="nav-link noto-sans-regular" href="#contact">Kontakt</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

<slot></slot>

<footer class="text-center" id="contact">
	<div class="container p-4">
		<div class="row">
			<div class="col-lg-6 col-md-12 mb-4 mb-md-0">
				<h5 class="text-uppercase">tohle tu nebude</h5>
				<p>bude tu logo</p>
			</div>
			<div class="col-lg-6 col-md-12 mb-4 mb-md-0">
				<p class="noto-sans-light contact">
					Petr Vančata<br />
					Soběslav, 392 01<br />
					<a href="tel:+420723522223">+420 723 522 223</a><br />
					<a href="mailto:petrvancata@email.cz">petrvancata@email.cz</a>
				</p>
			</div>
		</div>
	</div>
	<div class="text-center p-3">
		© 2020 Copyright:
		<a href="https://mdbootstrap.com/">MDBootstrap.com</a>
	</div>
</footer>

<style>
	:root {
		--dark: #4e3d33;
		--light: #f3e2d8;
		--semi: #c89c82;
	}

    :global(.color-light){
        color: var(--light) !important;
    }

    :global(.color-dark){
        color: var(--dark) !important;
    }

	a {
		color: var(--light);
		text-decoration: none;
        transition: all ease-in-out .15s;
	}

    a:hover{
        color: var(--semi);
    }

	nav {
		background-color: var(--dark) !important;
	}

	.nav-link {
		color: var(--light) !important;
	}

	footer {
		background-color: var(--dark);
		color: var(--light);
	}

	:global(.noto-sans-light) {
		font-family: 'Noto Sans', sans-serif !important;
		font-optical-sizing: auto !important;
		font-weight: 300 !important;
		font-style: normal !important;
		font-variation-settings: 'wdth' 100 !important;
	}

	:global(.noto-sans-regular) {
		font-family: 'Noto Sans', sans-serif !important;
		font-optical-sizing: auto !important;
		font-weight: 400 !important;
		font-style: normal !important;
		font-variation-settings: 'wdth' 100 !important;
	}

	:global(.noto-sans-bolder) {
		font-family: 'Noto Sans', sans-serif !important;
		font-optical-sizing: auto !important;
		font-weight: 500 !important;
		font-style: normal !important;
		font-variation-settings: 'wdth' 100 !important;
	}
</style>
