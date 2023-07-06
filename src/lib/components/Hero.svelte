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
	style="background-image: url('https://images.unsplash.com/photo-1644325349124-d1756b79dd42?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2675&q=80');"
>
	<div class="hero-overlay bg-opacity-70" />
	<div class="hero-content text-neutral-content">
		<div class="z-60 drop-shadow-lg text-center">
			<div class="mb-5 text-8xl font-semibold">SUSC</div>
			<div class="mb-10 text-xl">
				Seasonal University study & communication
			</div>

			<Countdown />
			<br>
			<div class="flex gap-4 justify-center">
				<button class="btn btn-primary transition-color duration-300 text-lg">신청하기</button>
				<button class="btn transition-color duration-300 text-lg">동아리 신청</button>
			</div>
		</div>
	</div>
</div>
