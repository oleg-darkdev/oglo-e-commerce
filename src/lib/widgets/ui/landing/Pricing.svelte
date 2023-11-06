<script>
	const microPlan = [
		{
			text: 'Jedno zlecenie',
			price: '$0.30'
		},
		{
			text: 'Pozycje katalogu',
			price: '$0.03'
		},
		{
			text: '1 GB danych',
			price: '$0.30'
		}
		// {
		//   text: 'API połączeńie:',
		//   price: '$0,00012'
		// },
	];

	const macroPlan = [
		{
			text: 'Jedno zlecenie',
			price: '$0.15'
		},
		{
			text: 'Pozycje katalogu',
			price: '$0.015'
		},
		{
			text: '1 GB danych',
			price: '$0.20'
		}
		// {
		//   text: 'API połączeńie:',
		//   price: '$0,00012'
		// },
	];

	const basicInclude = ['Nielimitowani użytkownicy', 'Wszystkie języki'];
</script>

<section class="relative z-30 -my-8 ml-20 w-8/12 rounded-xl bg-[#330066]">
	<div class="relative mx-auto w-full max-w-7xl items-center py-24 md:px-12 lg:px-16">
		<div class="mx-auto flex w-full flex-wrap items-start justify-center gap-4 px-5 lg:px-0">
			<div class="w-full md:text-center lg:w-2/6 lg:text-left xl:w-1/3">
				<a name="price" />
				<div class="flex flex-col p-8 lg:p-0">
					<strong class="mb-1 text-xs font-semibold uppercase tracking-widest text-secondary" />
					<span class="tracking-relaxed mb-8 text-2xl font-bold text-neutral-300 lg:text-4xl">
						Nasze ceny są idealne dla mikro i małych przedsiębiorców.
					</span>
					<p class="mx-auto mb-4 text-xl font-light text-gray-500 text-opacity-70 lg:pr-10">
						Oferujemy przystępne i elastyczne ceny, które pomogą Ci osiągnąć cele bez nadmiernych
						kosztów.
					</p>
					<p class="mx-auto mb-2 text-xl font-light text-gray-500 text-opacity-70 lg:pr-10">
						Dokonuj sprzedaży każdego miesiąca - bez limitów i bez obowiązkowej opłaty
						abonamentowej.
					</p>
				</div>
			</div>
			<div class="w-full md:w-2/6 xl:w-1/4">
				<div class="relative flex h-full flex-col rounded-xl bg-gray-50 p-8 hover:border-white">
					<span class="mb-4 text-base font-medium uppercase tracking-widest text-violet-900">
						Micro
					</span>
					<span class="mb-8 flex items-center text-base font-medium tracking-tight text-violet-900">
						Dla mikroprzedsiębiorców
					</span>
					<div class="flex  items-end text-3xl font-black leading-none text-violet-900 lg:text-4xl">
						<span class="text-violet-900">$0 </span>
						<span class="ml-4 font-light text-violet-800">/ FREE </span>
					</div>
					<ul class="mt-8">
						{#each basicInclude as basic}
							<li
								class=" my-3 flex items-center text-base font-medium tracking-tight text-violet-900"
							>
								<span
									class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center text-violet-900"
								>
									<svg
										fill="none"
										stroke="currentColor"
										stroke-linecap="round"
										stroke-linejoin="round"
										stroke-width="2.5"
										class="h-3 w-3"
										viewBox="0 0 24 24"
									>
										<path d="M20 6L9 17l-5-5" />
									</svg>
								</span>
								<strong>{basic}</strong>
							</li>
						{/each}

						<li
							class="mb-2 flex items-center text-base font-medium tracking-tight text-violet-900 text-opacity-70"
						>
							<span
								class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center text-violet-900 text-opacity-70"
							>
								<svg
									fill="none"
									stroke="currentColor"
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2.5"
									class="h-3 w-3"
									viewBox="0 0 24 24"
								>
									<line x1="18" y1="6" x2="6" y2="18" />
									<line x1="6" y1="6" x2="18" y2="18" />
								</svg>
							</span>
							Lifetime Support.
						</li>
						{#each microPlan as price}
							<li
								class="between my-3 flex flex-wrap items-center text-base font-light tracking-tight text-violet-900"
							>
								<strong class="max-w-[40px]">{price.text}</strong>
								<span class="ml-1 font-bold">{price.price}</span>
							</li>
						{/each}
					</ul>

					<!-- <div class="mt-8">
            <button class="w-full items-center block px-10 py-3.5 text-base font-medium text-center text-blue-600 transition duration-500 ease-in-out transform border-2 border-white shadow-md rounded-xl focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500 bg-white">Download</button>
          </div> -->
				</div>
			</div>
			<div class="w-full md:w-2/6 xl:w-1/4">
				<div class="relative flex h-full flex-col rounded-xl bg-secondary p-8 hover:border-white">
					<span class="mb-4 text-base font-medium uppercase tracking-widest text-white">
						Macro
					</span>
					<span class="mb-8 flex items-center text-base font-medium tracking-tight text-white">
						Dla małych przedsiębiorców.
					</span>
					<div class="flex items-end text-3xl font-black leading-none text-white lg:text-4xl">
						<span>
							<span>$8</span>
							<del class="text-2xl font-normal text-white">$16</del>
						</span>
					</div>
					<ul class='mt-8'>
						{#each basicInclude as basic}
							<li
								class=" mb-2 flex items-center text-base font-medium tracking-tight text-white"
							>
								<span
									class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center text-white"
								>
									<svg
										fill="none"
										stroke="currentColor"
										stroke-linecap="round"
										stroke-linejoin="round"
										stroke-width="2.5"
										class="h-3 w-3"
										viewBox="0 0 24 24"
									>
										<path d="M20 6L9 17l-5-5" />
									</svg>
								</span>
								<strong>{basic}</strong>
							</li>
						{/each}

						<li class="mb-2 flex items-center text-base font-medium tracking-tight text-white">
							<span
								class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center text-white"
							>
								<svg
									fill="none"
									stroke="currentColor"
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2.5"
									class="h-3 w-3"
									viewBox="0 0 24 24"
								>
									<path d="M20 6L9 17l-5-5" />
								</svg>
							</span>
							<strong>Lifetime Support</strong>
						</li>
						{#each macroPlan as price}
							<li
								class="between my-3 flex flex-wrap items-center text-base font-light tracking-tight text-white"
							>
								<strong class="max-w-[40px]">{price.text}</strong>
								<span class="ml-1 font-bold">{price.price}</span>
							</li>
						{/each}
					</ul>

					<!-- <div class="mt-8">
            <button class="w-full items-center block px-10 py-3.5 text-base font-medium text-center text-blue-600 transition duration-500 ease-in-out transform border-2 border-white shadow-md rounded-xl focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500 bg-white">Buy for $69</button>
          </div> -->
				</div>
			</div>
		</div>

		<div class="mx-auto mt-8 w-10/12">
			<img
				src="./images/social.svg"
				alt=""
				class="h-[300px] w-full rounded-xl border-2 border-secondary"
			/>
		</div>
	</div>
</section>

