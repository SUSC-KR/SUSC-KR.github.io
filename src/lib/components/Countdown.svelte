<script>
  import { onMount } from 'svelte';

let days = "00";
let hours = "00";
let minutes = "00";
let seconds = "00";

onMount(() => {
  const targetDate = new Date(2023, 6, 15, 13, 30); // 2023년 7월 15일 오후 1시 30분
  const countdownInterval = setInterval(() => {
	const now = new Date();
	const timeDifference = targetDate - now;

	if (timeDifference > 0) {
	  days = String(Math.floor(timeDifference / (1000 * 60 * 60 * 24))).padStart(2, '0');
	  hours = String(Math.floor((timeDifference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))).padStart(2, '0');
	  minutes = String(Math.floor((timeDifference % (1000 * 60 * 60)) / (1000 * 60))).padStart(2, '0');
	  seconds = String(Math.floor((timeDifference % (1000 * 60)) / 1000)).padStart(2, '0');
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
	  border-radius: 10px;
	  padding: 15px;
	  min-width: 72px;
	}
  
	.countdown-value {
	  font-size: 28px;
	  font-weight: bold;
	}
  
	.countdown-label {
	  font-size: 12px;
	}
  </style>

<div class="countdown-container flex center">
	<div class="countdown-item bg-neutral font-mono">
	  <span class="countdown-value">{days}</span>
	  <span class="countdown-label">days</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value">{hours}</span>
	  <span class="countdown-label">hours</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value">{minutes}</span>
	  <span class="countdown-label">min</span>
	</div>
	<div class="countdown-item bg-neutral">
	  <span class="countdown-value">{seconds}</span>
	  <span class="countdown-label">sec</span>
	</div>
</div>