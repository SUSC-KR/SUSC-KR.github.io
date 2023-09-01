<script lang="ts">
	import Carousel from '$lib/components/Carousel.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Stats from '$lib/components/Stats.svelte';
	import HeroCards from '$lib/components/HeroCards.svelte';
</script>

<div>
	<div class="">
		<div class="">
			<Hero />
		</div>

		<div class="lg:container mx-auto">
			<Carousel />
		</div>
	</div>
	<div class="container mx-auto">
		<Stats />

		<div class="my-10">
			<HeroCards />
		</div>

		<!-- <div class="my-10">
			<Links />
		</div>	 -->
	</div>
</div>
