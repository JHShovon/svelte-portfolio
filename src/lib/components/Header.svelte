<script>
	import Button from './buttons/Button.svelte';

	let menus = [
		{ name: 'home', link: '/' },
		{ name: 'service', link: '#service' },
		{ name: 'about me', link: '#about' },
		{ name: 'portfolio', link: '#portfolio' }
	];

	let isOpen = false;
	function menuToggle() {
		isOpen != isOpen;
	}
	const closeMenu = () => {
		isOpen = false;
	};
</script>

<header class="section-header fixed top-14 z-[9] w-full">
	<div class="section-container">
		<div class="scroll-t-8 flex items-center justify-between gap-7">
			<!-- Header Logo -->
			<a
				href="/"
				class="from-primary to-primary-dark bg-linear-to-r bg-clip-text text-3xl font-bold text-transparent uppercase"
				>Logo</a
			>
			<!-- Header Logo -->
			<!-- Header Menu -->
			<div
				class="bg-dark fixed top-0 left-0 z-10 flex min-h-svh w-72 flex-1 justify-start px-6 py-10 shadow shadow-white/5 lg:static lg:z-0 lg:min-h-auto lg:w-auto lg:justify-center lg:bg-transparent lg:p-0 lg:shadow-none"
				id="menu"
			>
				<nav>
					<ul class="flex flex-col gap-x-[60px] gap-y-4 font-medium uppercase lg:flex-row">
						{#each menus as menuItem}
							<li>
								<a href={menuItem.link} class=" hover:text-primary transition-all duration-300">
									{menuItem.name}
								</a>
							</li>
						{/each}
					</ul>
				</nav>
			</div>
			<!-- Header Menu -->

			<!-- Header Event Button -->
			<div class="flex gap-5">
				<button class="cursor-pointer lg:hidden" on:click={menuToggle}> Menu </button>
				<Button buttonText={'Hire Me'} buttonLink={'#contact'} />
			</div>
			<!-- Header Event Button -->
		</div>
	</div>
</header>
