<script>
	const faqData = [
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		},
		{
			question: 'Lorem ipsum is placeholder',
			answer:
				'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.'
		}
	];
</script>

<section class="bg-[#330066]">
	<div class="container mx-auto px-6 py-12">
		<h2
			class="max-w-3xl text-2xl  font-bold leading-none tracking-tighter text-neutral-200 md:text-5xl lg:max-w-5xl lg:text-4xl"
		>
			Często zadawane pytania
		</h2>

		<a name="faq" />

		<div class="mt-4 space-y-8 lg:mt-12 ">
			{#each faqData as faq}
				<!-- card -->
				<button
					class="w-full max-w-2xl rounded-lg bg-primary p-8"
					on:click={() => (faq.open = !faq.open)}
				>
					<div class="flex w-full items-center justify-between">
						<h1 class="font-semibold text-white">
							{faq.question}
						</h1>

						<span class="rounded-full bg-secondary text-primary">
							{#if faq.open}
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="h-6 w-6"
									fill="none"
									viewBox="0 0 24 24"
									stroke="currentColor"
								>
									<path
										stroke-linecap="round"
										stroke-linejoin="round"
										stroke-width="2"
										d="M18 12H6"
									/>
								</svg>
							{:else}
								<svg
									xmlns="http://www.w3.org/2000/svg"
									class="h-6 w-6"
									fill="none"
									viewBox="0 0 24 24"
									stroke="currentColor"
								>
									<path
										stroke-linecap="round"
										stroke-linejoin="round"
										stroke-width="2"
										d="M12 6v6m0 0v6m0-6h6m-6 0H6"
									/>
								</svg>
							{/if}
						</span>
					</div>

					{#if faq.open}
						<p class="mt-6 text-left text-sm text-gray-300">
							{faq.answer}
						</p>
					{/if}
				</button>
				<!-- card -->
			{/each}
		</div>
	</div>
</section>
