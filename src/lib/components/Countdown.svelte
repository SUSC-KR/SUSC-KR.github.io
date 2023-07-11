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
  
  <style>
	.countdown-container {
	  display: flex;
	  justify-content: center;
	  align-items: center;
	  gap: 10px;
	}
  
	.countdown-item {
	  display: flex;
	  flex-direction: column;
	  align-items: center;
	  /* background-color: #f0f0f0; */
	  border-radius: 10px;
	  padding: 10px;
	  /* color: #333; */
	}
  
	.countdown-value {
	  font-size: 30px;
	  font-weight: bold;
	}
  
	.countdown-label {
	  font-size: 12px;
	}
  </style>

  
  <div class="grid grid-flow-col gap-5 text-center auto-cols-max countdown-container">
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content countdown-item">
	  <span class="countdown font-mono text-5xl countdown-value">
		<span style="--value: {days};">{days}</span>
	  </span>
	  days
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content countdown-item">
	  <span class="countdown font-mono text-5xl countdown-value">
		<span style="--value: {hours};">{hours}</span>
	  </span>
	  hours
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content countdown-item">
	  <span class="countdown font-mono text-5xl countdown-value">
		<span style="--value: {minutes};">{minutes}</span>
	  </span>
	  min
	</div>
	<div class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content countdown-item">
	  <span class="countdown font-mono text-5xl countdown-value">
		<span style="--value: {seconds};">{seconds}</span>
	  </span>
	  sec
	</div>
  </div>
  