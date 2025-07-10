<script>
	import ButtonOutline from './buttons/Button-outline.svelte';
	import Button from './buttons/Button.svelte';

	let name = 'Mahmood Fazile';
	let role = 'UI/UX designer';
	let funfatcs = [
		{ number: 5, text: 'Experiences' },
		{ number: 20, text: 'Project done' },
		{ number: 80, text: 'Happy Clients' }
	];
</script>

<!-- Section Hero -->
<section class="section-hero">
	<div class="pt-64 pb-36">
		<div class="section-container">
			<!-- Hero Area -->
			<div
				class="relative z-[1] grid grid-cols-1 items-center gap-20 sm:gap-24 lg:grid-cols-2 2xl:grid-cols-[1fr_minmax(0,1.25fr)] 2xl:gap-32"
			>
				<div class="">
					<h1 class="text-white-dark-medium mb-6 text-2xl font-semibold tracking-[1px]">
						Hi, I am <br /> <span class="text-white-dark text-3xl font-bold">{name}</span>
					</h1>
					<h2
						class="from-primary to-primary-dark mb-4 bg-linear-to-r bg-clip-text text-5xl leading-[1.2] font-bold tracking-[2px] text-transparent xl:text-6xl 2xl:text-7xl"
					>
						{role}
					</h2>
					<!-- Social Icon -->
					<div class="mt-8 mb-14 flex flex-wrap gap-5">
						<a
							href="http://www.instagram.com"
							target="_blank"
							rel="noopener noreferrer"
							aria-label="facebook"
							class="border-white-darker hover:border-primary inline-flex size-10 items-center justify-center rounded-full border bg-white/5 transition-all duration-300"
						>
							<img src="assets/images/icons/icon-instagram.svg" alt="instagram" />
						</a>
						<a
							href="http://www.linkedin.com"
							target="_blank"
							rel="noopener noreferrer"
							aria-label="facebook"
							class="border-white-darker hover:border-primary inline-flex size-10 items-center justify-center rounded-full border bg-white/5 transition-all duration-300"
						>
							<img src="assets/images/icons/icon-linkedin-line.svg" alt="linkedin" />
						</a>
						<a
							href="http://www.dribble.com"
							target="_blank"
							rel="noopener noreferrer"
							aria-label="facebook"
							class="border-white-darker hover:border-primary inline-flex size-10 items-center justify-center rounded-full border bg-white/5 transition-all duration-300"
						>
							<img src="assets/images/icons/icon-dribble.svg" alt="dribble" />
						</a>
						<a
							href="http://www.behance.com"
							target="_blank"
							rel="noopener noreferrer"
							aria-label="facebook"
							class="border-white-darker hover:border-primary inline-flex size-10 items-center justify-center rounded-full border bg-white/5 transition-all duration-300"
						>
							<img src="assets/images/icons/icon-behance-line.svg" alt="behance" />
						</a>
					</div>
					<!-- Social Icon -->

					<!-- Hero Buttons -->
					<div class="flex flex-wrap gap-6">
						<Button buttonText={'Hire Me'} buttonLink={'#contact'} />
						<ButtonOutline buttonText={'Download CV'} buttonLink={'https://www.example.com'} />
					</div>
					<!-- Hero Buttons -->

					<!-- Fun-fact Block-->
					<ul
						class="mt-14 flex max-w-xl flex-col justify-center divide-y-[1px] rounded-lg bg-white/5 p-6 sm:flex-row sm:divide-x-[1px] sm:divide-y-0 xl:mt-20"
					>
						{#each funfatcs as funfactItem}
							<li
								class="py-6 first-of-type:pt-0 last-of-type:pb-0 sm:px-8 sm:py-0 sm:first-of-type:pl-0 sm:last-of-type:pr-0"
							>
								<span class="text-primary mb-4 block text-2xl font-extrabold"
									>{funfactItem.number}+</span
								>
								<span class="block font-bold text-white">{funfactItem.text}</span>
							</li>
						{/each}
					</ul>
					<!-- Fun-fact Block-->
				</div>
				<div class="mt-28 flex justify-center lg:mt-0 lg:justify-end">
					<div
						class="relative inline-flex size-80 justify-center rounded-full bg-white/5 sm:size-96 lg:size-[450px] xl:size-[550px] 2xl:size-[618px]"
					>
						<img
							src="assets/images/hero-user-img.png"
							alt="Hero User"
							width="520"
							height="781"
							class="absolute bottom-0"
						/>
						<img src="" alt="" />
					</div>
				</div>
				<div class="absolute top-0 left-0 -z-[1] duration-[4000]">
					<img src="assets/images/hero-shape.svg" alt="hero-shape" width="748" height="677" />
				</div>
			</div>
			<!-- Hero Area -->
		</div>
	</div>
</section>
<!-- Section Hero -->
