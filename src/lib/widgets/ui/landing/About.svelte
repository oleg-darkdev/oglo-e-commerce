<script>
	const aboutUsText = [
		{
			title: 'Automatyczna publikacja ogłoszeń',
			desc: 'Obecnie skupiamy się na platformach na OLX i Allegro oraz na Instagramie i Facebooku.',
			icon: '',
			link: ''
		},
		{
			title: 'Przystępne i elastyczne ceny',
			desc: 'Oferujemy które pomogą Ci osiągnąć cele bez nadmiernych kosztów.',
			icon: '',
			link: '#prices'
		},
		{
			title: 'Dobry ceł i głęboką filozofią.',
			desc: 'Projekt jest open source i jest dostępny do użytku na prywatnych serwerach.',
			icon: '',
			link: '#сommunity'
		},

	];
</script>

<section>
	<a name="about" />

	<div class=" mx-auto flex max-w-7xl flex-col items-center px-5 py-8 sm:px-6 lg:px-8">
		<div class="prose-primary prose mx-auto flex w-full max-w-3xl flex-col text-left">
			<div class="mx-auto w-full ">
				<h1 class="text-primary">Stworzony z myślą o małych przedsiębiorcach i społeczności.</h1>
				<h2 class="text-violet-800">Lorem ipsum is placeholder text commonly used.</h2>
				<p class="text-violet-800">
					Lorem ipsum is placeholder text commonly used in the graphic, print, and publishing
					industries for previewing layouts and visual mockups.
				</p>
			</div>
		</div>

		<div class="mx-auto my-10 flex max-w-5xl flex-col items-center  pb-10 ">
			{#each aboutUsText as text}
				<div
					class="mx-auto my-6 flex between  w-full items-center border-b border-primary pb-10 sm:flex-row"
				>
					<!-- <div
						class="inline-flex h-20 w-20 flex-shrink-0 items-center justify-center rounded-full bg-gray-50 text-primary sm:mr-10"
					>
						<img src={text.icon} class='' alt="" />
					</div> -->
					<div class="prose-md prose mt-2 w-full flex-grow text-center sm:mt-0 sm:text-left">
						<h2 class="text-violet-800">{text.title}</h2>
						<p class="text-violet-800">
							{text.desc}
						</p>
					</div>
					<div class="">
						<a
							href={text.link}
							class="block w-full transform items-center rounded-xl border-2 border-white bg-primary px-10 py-3.5 text-center text-base font-medium text-white shadow-md transition duration-500 ease-in-out focus:outline-none focus:ring-2 focus:ring-gray-500 focus:ring-offset-2"
							>Więcej informacji</a
						>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
