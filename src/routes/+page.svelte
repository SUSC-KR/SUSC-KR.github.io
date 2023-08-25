<script lang="ts">
	import Carousel from '$lib/components/Carousel.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Stats from '$lib/components/Stats.svelte';
	import HeroCards from '$lib/components/HeroCards.svelte';
	// import Links from '$lib/components/Links.svelte';
	// import Drawer from '$lib/components/Drawer.svelte';
	// import Card from '$lib/components/Card.svelte';
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
