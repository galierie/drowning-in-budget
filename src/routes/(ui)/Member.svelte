<script>
	import Icon from "@iconify/svelte";
	const { name, github, description } = $props();
</script>

<div class="m-5 px-5 py-10 w-300 flex flex-col justify-center rounded-lg border-2 border-rhino-500 shadow-lg">
	<p class="text-center">{name}</p>
	<div class="flex items-center justify-center">
		<Icon icon="mdi:github" class="m-1"></Icon>
		<a href="https://github.com/{github}" class="text-center text-rhino-500 underline"
			>@{github}</a
		>
	</div>
	<p class="text-center">{description}</p>
</div>
