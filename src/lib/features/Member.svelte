<script>
	const { name, github, description } = $props();
</script>

<div class="my-4 flex flex-col justify-center rounded-xl bg-olive-haze-700 shadow-xl">
	<p class="text-center">{name}</p>
	<a href="https://github.com/{github}" class="text-center text-olive-haze-200 underline"
		>@{github}</a
	>
	<p class="text-center">{description}</p>
</div>
