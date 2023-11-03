<script>
	const aboutUsText = [
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			icon: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			icon: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			icon: ''
		},
		{
			title: 'Lorem ipsum is placeholder',
			desc: 'Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing industries for previewing layouts and visual mockups.',
			icon: ''
		}
	];
</script>

<section>
	<a name="about" />

	<div class=" mx-auto flex max-w-7xl flex-col items-center px-5 py-8 sm:px-6 lg:px-8">
		<div class="prose-primary prose mx-auto flex w-full max-w-3xl flex-col text-left">
			<div class="mx-auto w-full ">
				<h1 class="text-primary">Lorem ipsum is placeholder text commonly used.</h1>
				<h2 class="text-violet-800">Lorem ipsum is placeholder text commonly used.</h2>
				<p class="text-violet-800">
					Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing
					industries for previewing layouts and visual mockups.
				</p>
			</div>
		</div>

		<div
			class="mx-auto my-10 flex max-w-7xl flex-col items-center  pb-10 "
		>
			{#each aboutUsText as text}
				<div
					class="mx-auto my-10 flex max-w-7xl flex-col items-center border-b border-primary pb-10 sm:flex-row"
				>
					<div
						class="inline-flex h-20 w-20 flex-shrink-0 items-center justify-center rounded-full bg-gray-50 text-primary sm:mr-10"
					>
						<img src={text.icon} class='' alt="" />
					</div>
					<div class="prose-md prose mt-6 flex-grow text-center sm:mt-0 sm:text-left">
						<h2 class='text-violet-800'>{text.title}</h2>
						<p class='text-violet-800'>
							{text.desc}
						</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
