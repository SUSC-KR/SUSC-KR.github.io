<script>
	import Countdown from '$lib/components/Countdown.svelte';
</script>
<div class="bg-base-100 sticky top-0 shadow-lg z-40 p-3">
	<div class="flex items-center justify-between p-2 lg:container lg:mx-auto">
		<div class="">
			<a href="/" class="font-bold text-primary text-2xl">SUSC</a>
		</div>
	</div>
</div>
<div
	class="hero h-[100vh] lg:h-[45rem] shadow-lg"
	style="background-image: url('/banner.png');"
>
	<div class="hero-overlay bg-opacity-70" />
	<div class="hero-content text-neutral-content">
		<div class="z-60 drop-shadow-lg text-center">
			<div class="mb-5 text-8xl font-semibold">SUSC</div>
			<div class="mb-10 text-xl">
				Seasonal University study & communication
			</div>

			<!-- <Countdown /> -->
			<br>
			<div class="flex gap-4 justify-center">
				<a href="https://forms.gle/tPQ9oBb8oTsQh9jT8" target="_blank"><button class="btn btn-primary transition-color duration-300 text-lg">신청하기</button></a>
				<button class="btn transition-color duration-300 text-lg">동아리 문의하기</button>
			</div>
		</div>
	</div>
</div>
