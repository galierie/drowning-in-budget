<script>
  import { asset } from '$app/paths';

  import flood from '$lib/assets/flood.jpg';
</script>

<header class="relative w-full h-screen lg:bg-linear-to-l bg-linear-to-b from-0% via-olive-haze-500 via-65% to-olive-haze-500 text-foreground">
  <div class="lg:w-5/10 w-full lg:h-full h-1/2 absolute lg:top-0 bottom-0 z-100 left-0 lg:py-30 py-10 pl-10 lg:pr-0 flex flex-col justify-center pr-10 *:lg:text-left *:text-center *:*:text-shadow-olive-haze-800">
    <div class="mb-4 font-specialelite">
      <p class="lg:text-3xl text-2xl mb-2 text-shadow-sm">Drowning in Budget:</p>
      <h1 class="lg:text-6xl text-4xl text-shadow-lg">How Flood Control Budget Correlates to Damage Caused by Flooding</h1>
    </div>
    <div>
      <p class="text-shadow-sm">
        <b>Sustainable Development Goal</b>: (11) Sustainable Cities and Communities: Urban Planning,
        Infrastructure Resilience, Environmental Sustainability
      </p>
    </div>
    <div class="*:text-shadow-sm mt-10 text-center text-xl">
      <p>A special report on flood control projects</p>
      <p>by <b>CS 132 25.1 WFV Group 1</b></p>
    </div>
  </div>

  <div class="flex h-full justify-end items-center absolute top-0 -z-100 right-0">
    <img src={asset(flood)} alt="child swimming in floodwaters" class="h-full object-cover object-center" />
  </div>
</header>