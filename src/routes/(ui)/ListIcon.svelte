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
	class="m-5 flex h-full flex-col items-center rounded-lg border-2 border-rhino-500 px-5 py-10 text-2xl shadow-lg md:w-125"
>
	<Icon {icon} class="h-50 w-50 text-rhino-500" />
	<p class="mt-4 flex grow items-center justify-center">
		{@render children()}
	</p>
</li>
