<script>
	import favicon from '$lib/assets/favicon.svg';
	import Header from '$lib/assets/components/Header.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<Header />

<main>
	{@render children()}
</main>
