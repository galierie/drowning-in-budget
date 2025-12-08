<script lang="ts">
  import Icon from '@iconify/svelte';
	import type { Snippet } from 'svelte';

  interface Props {
    icon: string;
    children: Snippet;
  }

  const { icon, children }: Props = $props();
</script>

<li class="w-175 h-full rounded-lg border-2 border-olive-haze-500 py-10 px-5 flex flex-col items-center font-specialelite text-xl mx-5 my-5">
  <Icon {icon} class="text-olive-haze-500 rounded-full border-2 border-olive-haze-500 w-50 h-50" />
  <p class="mt-4 grow flex justify-center items-center text-shadow-sm">
    {@render children()}
  </p>
</li>