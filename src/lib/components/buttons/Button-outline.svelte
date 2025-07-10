<script>
	let { buttonText, buttonLink } = $props();
</script>

<a
	href={buttonLink}
	class="group border-white-dark relative inline-flex items-center justify-center overflow-hidden rounded-lg border bg-transparent px-10 py-3 text-base font-bold text-white"
>
	<span
		class="translate-y-0 opacity-100 transition-all duration-300 group-hover:-translate-y-full group-hover:opacity-0"
		>{buttonText}</span
	>
	<span
		class="absolute translate-y-full opacity-0 transition-all duration-300 group-hover:translate-y-0 group-hover:opacity-100"
		>{buttonText}</span
	>
</a>
