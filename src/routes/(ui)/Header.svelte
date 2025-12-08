<script>
	import { asset } from '$app/paths';

	import flood from '$lib/assets/flood.jpg';
</script>

<header
	class="relative h-screen w-full bg-linear-to-b from-0% via-olive-haze-500 via-65% to-olive-haze-500 text-foreground lg:bg-linear-to-l"
>
	<div
		class="absolute bottom-0 left-0 z-100 flex h-full w-full flex-col justify-center py-10 pr-10 pl-10 *:text-center *:*:text-shadow-olive-haze-800 lg:top-0 lg:w-5/10 lg:py-30 lg:pr-0 *:lg:text-left"
	>
		<div class="mb-4 font-specialelite">
			<p class="mb-2 text-2xl text-shadow-sm lg:text-3xl">Drowning in Budget:</p>
			<h1 class="text-4xl text-shadow-lg lg:text-6xl">
				How Flood Control Budget Correlates to Damage Caused by Flooding
			</h1>
		</div>
		<div>
			<p class="text-shadow-sm">
				<b>Sustainable Development Goal</b>: (11) Sustainable Cities and Communities: Urban
				Planning, Infrastructure Resilience, Environmental Sustainability
			</p>
		</div>
		<div class="mt-10 text-center text-xl *:text-shadow-sm">
			<p>A special report on flood control projects</p>
			<p>by <b>CS 132 25.1 WFV Group 1</b></p>
		</div>
	</div>

	<div class="absolute top-0 right-0 -z-100 flex h-full items-center justify-end">
		<img
			src={flood}
			alt="child swimming in floodwaters"
			class="h-full object-cover object-center"
		/>
	</div>
</header>
