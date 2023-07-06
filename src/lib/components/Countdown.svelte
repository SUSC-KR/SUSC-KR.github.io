<!-- <div class="grid grid-flow-col gap-5 text-center auto-cols-max">
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
		<span class="countdown font-mono text-5xl">
			<span style="--value:15;" />
		</span>
		days
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
		<span class="countdown font-mono text-5xl">
			<span style="--value:10;" />
		</span>
		hours
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
		<span class="countdown font-mono text-5xl">
			<span style="--value:24;" />
		</span>
		min
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
		<span class="countdown font-mono text-5xl">
			<span style="--value:38;" />
		</span>
		sec
	</div>
</div> -->

<script>
	import { onMount } from 'svelte';
  
	let days = 0;
	let hours = 0;
	let minutes = 0;
	let seconds = 0;
  
	onMount(() => {
	  const targetDate = new Date(2023, 6, 15, 13, 30); // 2023년 7월 15일 오후 1시 30분
	  const countdownInterval = setInterval(() => {
		const now = new Date();
		const timeDifference = targetDate - now;
  
		if (timeDifference > 0) {
		  days = Math.floor(timeDifference / (1000 * 60 * 60 * 24));
		  hours = Math.floor((timeDifference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
		  minutes = Math.floor((timeDifference % (1000 * 60 * 60)) / (1000 * 60));
		  seconds = Math.floor((timeDifference % (1000 * 60)) / 1000);
		} else {
		  clearInterval(countdownInterval);
		}
	  }, 1000);
	});
  </script>
  
  <div class="grid grid-flow-col gap-5 text-center auto-cols-max">
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
	  <span class="countdown font-mono text-5xl">
		<span style="--value: {days};">{days}</span>
	  </span>
	  days
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
	  <span class="countdown font-mono text-5xl">
		<span style="--value: {hours};">{hours}</span>
	  </span>
	  hours
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
	  <span class="countdown font-mono text-5xl">
		<span style="--value: {minutes};">{minutes}</span>
	  </span>
	  min
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
	  <span class="countdown font-mono text-5xl">
		<span style="--value: {seconds};">{seconds}</span>
	  </span>
	  sec
	</div>
  </div>
  