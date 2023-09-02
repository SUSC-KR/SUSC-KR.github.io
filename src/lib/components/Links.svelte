<script lang="ts">
	import { base } from "$app/paths";
</script>
<style>
	@media screen and (max-width: 768px) {
	a {
		/* 모바일 환경에서 너비를 80%로 설정 */
		width: 60%;
	}
	}
</style>

<div class="flex flex-col md:flex-row gap-2 xl:gap-5 justify-center items-center">
	<a
		class="w-[30%] bg-base-100 rounded-lg shadow-lg p-4 text-xl font-bold text-center hover:bg-base-300 transition-all duration-300"
		href="https://www.linkedin.com/company/susc-kr/posts/?feedView=all"
		target="_blank"
	>
		<div>Linkedin</div>
	</a>

	<a
		class="w-[30%] bg-base-100 rounded-lg shadow-lg p-4 text-xl font-bold text-center hover:bg-base-300 transition-all duration-300"
		href="https://github.com/SUSC-KR"
		target="_blank"
	>
		<div>Github</div>
	</a>

	<!-- <a
		class="w-full bg-base-100 rounded-lg shadow-lg p-4 text-xl font-bold text-center hover:bg-base-300 transition-all duration-300"
		href="{base}/"
	>
		<div>Contribute</div>
	</a>

	<a
		class="w-full bg-base-100 rounded-lg shadow-lg p-4 text-xl font-bold text-center hover:bg-base-300 transition-all duration-300"
		href="{base}/"
	>
		<div>Contact</div>
	</a> -->
</div>
