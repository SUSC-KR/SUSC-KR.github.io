<style>
@import 'https://fonts.googleapis.com/css?family=Open+Sans:600,700';

* {font-family: 'Open Sans', sans-serif;}

.rwd-table {
  margin: auto;
  min-width: 300px;
  max-width: 100%;
  border-collapse: collapse;
}

.rwd-table tr:first-child {
  border-top: none;
  background: #428bca;
  color: #fff;
}

.rwd-table tr {
  border-top: 1px solid #ddd;
  border-bottom: 1px solid #ddd;
  background-color: #f5f9fc;
}

.rwd-table tr:nth-child(odd):not(:first-child) {
  background-color: #ebf3f9;
}

.rwd-table th {
  display: none;
}

.rwd-table td {
  display: block;
}

.rwd-table td:first-child {
  margin-top: .5em;
}

.rwd-table td:last-child {
  margin-bottom: .5em;
}

.rwd-table td:before {
  content: attr(data-th) ": ";
  font-weight: bold;
  width: 120px;
  display: inline-block;
  color: #000;
}

.rwd-table th,
.rwd-table td {
  text-align: left;
}

.rwd-table {
  color: #333;
  border-radius: .4em;
  overflow: hidden;
}

.rwd-table tr {
  border-color: #bfbfbf;
}

.rwd-table th,
.rwd-table td {
  padding: .5em 1em;
}
@media screen and (max-width: 601px) {
  .rwd-table tr:nth-child(2) {
    border-top: none;
  }
}
@media screen and (min-width: 600px) {
  .rwd-table tr:hover:not(:first-child) {
    background-color: #d8e7f3;
  }
  .rwd-table td:before {
    display: none;
  }
  .rwd-table th,
  .rwd-table td {
    display: table-cell;
    padding: .25em .5em;
  }
  .rwd-table th:first-child,
  .rwd-table td:first-child {
    padding-left: 0;
  }
  .rwd-table th:last-child,
  .rwd-table td:last-child {
    padding-right: 0;
  }
  .rwd-table th,
  .rwd-table td {
    padding: 1em !important;
  }
}


/* THE END OF THE IMPORTANT STUFF */

/* Basic Styling */
body {
background: #4B79A1;
background: -webkit-linear-gradient(to left, #4B79A1 , #283E51);
background: linear-gradient(to left, #4B79A1 , #283E51);        
}

.container {
  display: block;
  text-align: center;
}

@-webkit-keyframes leftRight {
  0%    { -webkit-transform: translateX(0)}
  25%   { -webkit-transform: translateX(-10px)}
  75%   { -webkit-transform: translateX(10px)}
  100%  { -webkit-transform: translateX(0)}
}
@keyframes leftRight {
  0%    { transform: translateX(0)}
  25%   { transform: translateX(-10px)}
  75%   { transform: translateX(10px)}
  100%  { transform: translateX(0)}
}
</style>
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
			<!-- <p class="py-6">
				Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem
				quasi. In deleniti eaque aut repudiandae et a id nisi.
			</p> -->
			<!-- <button class="btn btn-primary w-full">Get Started</button> -->
		</div>
	</div>
</div>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row-reverse xl:gap-32">
		<img
			alt="hero"
			src="/mentors.png"
			class="h-80 w-[80%] object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-full">
			<h1 class="text-3xl font-bold">현업 전문가<br> 멘토링</h1>
			<!-- <p class="py-6">
				Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem
				quasi. In deleniti eaque aut repudiandae et a id nisi.
			</p> -->
			<br>
			<a href="{base}/mentoring">
				<button class="btn btn-primary w-full">
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
			src="/proj.jpg"
			class="h-80 w-full object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-auto">
			<h1 class="text-3xl font-bold">프로젝트 및 공모전</h1>
			<!-- <p class="py-6">
				Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem
				quasi. In deleniti eaque aut repudiandae et a id nisi.
			</p> -->
			<!-- <button class="btn btn-primary w-full">Get Started</button> -->
		</div>
	</div>
</div>

<div class="hero min-h-full bg-base-200 rounded-lg">
	<div class="hero-content flex-col lg:flex-row-reverse xl:gap-32">
		<img
			alt="hero"
			src="papers.jpg"
			class="h-80 w-full object-cover rounded-lg shadow-lg"
		/>
		<div class="text-center w-full">
			<h1 class="text-3xl font-bold">연구 활동 및 주제 탐구</h1>
			<!-- <p class="py-6">
				Provident cupiditate voluptatem et in. Quaerat fugiat ut assumenda excepturi exercitationem
				quasi. In deleniti eaque aut repudiandae et a id nisi.
			</p> -->
			<!-- <button class="btn btn-primary w-full">Get Started</button> -->
		</div>
	</div>
</div>
