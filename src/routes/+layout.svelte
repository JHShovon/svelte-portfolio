<script>
	import Footer from '$lib/components/Footer.svelte';
	import Header from '$lib/components/Header.svelte';
	import '../app.css';

	let { children } = $props();
</script>

<div class="relative z-[1] overflow-x-clip">
	<Header />
	{@render children()}
	<Footer />
</div>
