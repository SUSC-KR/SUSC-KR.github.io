<script>
	import { base } from "$app/paths";
</script>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row xl:gap-32">
		<div class="text-lg text-center my-5 border-b-2">
			<table class="table-auto text-xl mx-auto bg-gray-100">
				<thead>
				  <tr>
					<th class="px-4 py-2">연사자</th>
					<th class="px-4 py-2">분야</th>
					<th class="px-4 py-2">내용</th>
				  </tr>
				</thead>
				<tbody>
				  <tr>
					<td class="border px-4 py-2">정상수</td>
					<td class="border px-4 py-2">보안</td>
					<td class="border px-4 py-2">보안에 입문한 이야기 및 각 보안분야별 공부 방법론</td>
				  </tr>
				  <tr>
					<td class="border px-4 py-2">임재혁</td>
					<td class="border px-4 py-2">보안/블록체인</td>
					<td class="border px-4 py-2">블록체인이 해킹되는 과정을 다룬 이야기</td>
				  </tr>
				  <tr>
					<td class="border px-4 py-2">옥찬호</td>
					<td class="border px-4 py-2">C++/Rust</td>
					<td class="border px-4 py-2">대학생때 알았다면 좋았을것들</td>
				  </tr>
				</tbody>
			  </table>
		</div>
		
		<div class="text-center max-w-lg">
			<h1 class="text-3xl font-bold">전문 분야별 세미나</h1>
			<br>
			<a href="https://www.youtube.com/@SUSCkr">
				<button class="btn btn-primary w-60">
					<div>다시보기</div>
				</button>
			</a>
		</div>
	</div>
</div>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row-reverse xl:gap-32">
		<img
			alt="hero"
			src="/mentor1.png"
			class="h-80 w-[100%] object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-full">
			<h1 class="text-3xl font-bold w-full">현업 전문가<br> 멘토링</h1>
			<br>
			<a href="{base}/mentoring">
				<button class="btn btn-primary w-60">
					<div>TimeTable</div>
				</button>
			</a>
		</div>
	</div>
</div>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row xl:gap-32">
		<img
			alt="hero"
			src="/suscnet.png"
			class="h-80 w-full object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-auto">
			<h1 class="text-3xl font-bold">프로젝트 및 공모전</h1>
		</div>
	</div>
</div>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row-reverse">
		<img
			alt="hero"
			src="papers.jpg"
			class="h-80 w-full object-cover rounded-lg shadow-lg"
		/>
		<img
			alt="hero"
			src="papers2.png"
			class="h-80 w-full object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-full">
			<h1 class="text-3xl font-bold m-auto">연구 활동 및 주제 탐구</h1>
		</div>
	</div>
</div>
