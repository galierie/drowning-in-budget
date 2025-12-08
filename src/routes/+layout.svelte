<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	import Header from './(ui)/Header.svelte';

	const { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<Header />

<main class="py-10">
	{@render children?.()}
</main>
