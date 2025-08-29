<script>
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
	<nav class="w-full flex justify-center gap-1 h-10">
		<a href="/" class="text-xl font-bold w-30 text-center content-center">Home</a>
		<a href="/details" class="text-xl font-bold w-30 text-center content-center">Details</a>
		<a href="/gallery" class="text-xl font-bold w-30 text-center content-center">Gallery</a>
	</nav>
</header>
<main>
	{@render children?.()}
</main>
