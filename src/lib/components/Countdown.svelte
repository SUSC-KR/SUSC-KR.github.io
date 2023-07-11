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
	  padding: 15px;
	  /* color: #333; */
	}
  
	.countdown-value {
	  font-size: 28px;
	  font-weight: bold;
	}
  
	.countdown-label {
	  font-size: 12px;
	}
  </style>

<div class="countdown-container">
	<div class="countdown-item bg-neutral font-mono">
	  <span class="countdown-value"><span style="--value: {days};">{days}</span></span>
	  <span class="countdown-label">days</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value"><span style="--value: {hours};">{hours}</span></span>
	  <span class="countdown-label">hours</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value"><span style="--value: {minutes};">{minutes}</span></span>
	  <span class="countdown-label">min</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value"><span style="--value: {seconds};">{seconds}</span></span>
	  <span class="countdown-label">sec</span>
	</div>
  </div>