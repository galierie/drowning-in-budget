<script lang="ts">
	import Icon from '@iconify/svelte';
	import type { Snippet } from 'svelte';

	interface Props {
		icon: string;
		children: Snippet;
	}

	const { icon, children }: Props = $props();
</script>

<li
	class="mx-5 my-5 flex h-full w-175 flex-col items-center rounded-lg border-2 border-olive-haze-500 px-5 py-10 font-specialelite text-xl"
>
	<Icon {icon} class="h-50 w-50 rounded-full border-2 border-olive-haze-500 text-olive-haze-500" />
	<p class="mt-4 flex grow items-center justify-center text-shadow-sm">
		{@render children()}
	</p>
</li>
