<script>
	const links = [
		{
			text: 'Główna',
			anchor: '/'
		},
		{
			text: 'O nas',
			anchor: '#about'
		},
		{
			text: 'Ceny',
			anchor: '#price'
		},
		{
			text: 'Społeczność',
			anchor: '#сommunity'
		},
		{
			text: 'F.A.Q.',
			anchor: '#faq'
		},
		{
			text: 'Contact',
			anchor: '#contact'
		}
	];

	let showNav = false;
</script>

<header>
	<nav class="bg-primary shadow ">
		<div class="container mx-auto px-6 py-4">
			<div class="lg:flex lg:items-center lg:justify-between">
				<div class="flex items-center justify-between">
					<a href="/" class="mx-auto ">
						<img class="h-12 w-auto" src="./images/logo.svg" alt="Logo oglo" />
					</a>

					<!-- Mobile menu button -->
					<div class="flex lg:hidden">
						<button
							on:click={() => (showNav = !showNav)}
							type="button"
							class=" gray-200 text-secondary hover:text-gray-400 focus:text-gray-400 focus:outline-none"
							aria-label="toggle menu"
						>
							{#if !showNav}
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="h-6 w-6"
									fill="none"
									viewBox="0 0 24 24"
									stroke="currentColor"
									stroke-width="2"
								>
									<path stroke-linecap="round" stroke-linejoin="round" d="M4 8h16M4 16h16" />
								</svg>
							{:else}
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="h-6 w-6"
									fill="none"
									viewBox="0 0 24 24"
									stroke="currentColor"
									stroke-width="2"
								>
									<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
								</svg>
							{/if}
						</button>
					</div>
				</div>
				<!-- :class="translate-x-0 opacity-100 ' : 'opacity-0 -translate-x-full']"  -->
				<!-- Mobile Menu open: "block", Menu closed: "hidden" -->
				<div
					class="absolute inset-x-0 {showNav
						? 'py-6'
						: ''}  z-20 w-full bg-primary  px-6 shadow-md transition-all duration-300 ease-in-out lg:relative lg:top-0 lg:mt-0 lg:w-auto lg:translate-x-0 lg:bg-transparent lg:p-0 lg:opacity-100 lg:shadow-none lg:dark:bg-transparent"
				>
					<div class="-mx-4 {showNav ? '' : 'hidden'} lg:flex lg:items-center">
						{#each links as link}
							<a
								href="{link.anchor}"
								class="mx-4 mb-2 block capitalize text-gray-200 hover:text-secondary">{link.text}</a
							>
						{/each}
					</div>
				</div>
			</div>
		</div>
	</nav>

	<div class="flex w-full justify-center rounded-xl">
		<div
			class="h-[34rem]  w-11/12 rounded-xl bg-cover bg-center"
			style="background-image: url('./images/hero.svg');"
		>
			<div class="flex h-full w-full items-center justify-center bg-violet-900/60">
				<div class="text-center">
					<div class="text-center">
						<h1
							class="max-w-5xl text-2xl font-bold leading-none tracking-tighter text-neutral-200 md:text-5xl lg:max-w-7xl lg:text-6xl"
						>
							Zautomatyzuj swoje <br class="hidden lg:block" />
							<span class="text-secondary">ogłoszenia</span>
						</h1>
						<p class="mx-auto mt-8 max-w-xl text-base leading-relaxed text-gray-200">
							Oglo - to system do zarządzania sprzedażą wielokanałową opracowany przez i dla
							społeczności.
						</p>
						<div class="mx-auto mt-6 flex w-full max-w-2xl justify-center gap-2">
							<div class="mt-3 rounded-lg sm:mt-0">
								<button
									class="transform rounded-xl bg-secondary px-5 py-4 text-center text-base font-medium text-white transition duration-500 ease-in-out hover:bg-primary focus:outline-none lg:px-10"
									>Rozpoczęcie</button
								>
							</div>
							<div class="mt-3 rounded-lg sm:mt-0 sm:ml-3">
								<a
									href="#about"
									class="block transform items-center rounded-xl border-2 border-white px-5 py-3.5 text-center text-base font-medium text-neutral-200 shadow-md transition duration-500 ease-in-out hover:bg-white hover:text-primary focus:outline-none  lg:px-10"
									>Zobacz funkcje</a
								>
							</div>
						</div>

						\
					</div>
				</div>
			</div>
		</div>
	</div>
</header>
