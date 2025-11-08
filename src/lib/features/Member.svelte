<script>
  const { name, github, description } = $props()
</script>

<div class="flex flex-col justify-center rounded-xl shadow-xl bg-olive-haze-700 my-4">
  <p class="text-center">{name}</p>
  <a href="https://github.com/{github}" class="text-olive-haze-200 underline text-center">@{github}</a>
  <p class="text-center">{description}</p>
</div>