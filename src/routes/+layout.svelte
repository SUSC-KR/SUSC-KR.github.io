<script lang="ts">
	import '$lib/app.css';
	import Footer from '$lib/components/Footer.svelte';
</script>

<div class="bg-base-200">
	<div class="">
		<slot />
	</div>
	<Footer />
</div>
