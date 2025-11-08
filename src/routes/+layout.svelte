<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	import background from '$lib/assets/flood.jpg';

	const { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<img src={background} alt="" class="absolute top-0 -z-100 w-full" />

<main class="bg-linear-to-b from-0% via-olive-haze-500 via-10% to-olive-haze-950 text-foreground">
	<div class="mx-10 pt-150 pb-4">
		{@render children?.()}
	</div>
</main>
