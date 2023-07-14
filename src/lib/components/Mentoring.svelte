<script>
  import Card from "./Card.svelte";

</script>
<div class=" bg-base-300 p-4 xl:p-10 rounded-lg w-[100%]">
	<div class="mx-auto pb-10 w-[100%]">
		<div class="text-3xl font-bold text-center my-5">멘토링 TimeTable</div>
		<div class="text-lg text-center my-5 border-b-2 w-[100%]">
			<table class="text-xl mx-auto bg-gray-100 w-[100%]">
				<thead>
				  <tr>
					<th class="px-4 py-2">분야</th>
					<th class="px-4 py-2">멘토</th>
					<th class="px-4 py-2">방식</th>
					<th class="px-4 py-2">다루는 내용</th>
					<th class="px-4 py-2">커리큘럼</th>
					<th class="px-4 py-2">멘토링 시간</th>
				  </tr>
				</thead>
				<tbody>
				  <tr>
					<td data-th="border px-4 py-2">보안</td>
					<td data-th="border px-4 py-2">임재혁 멘토</td>
					<td data-th="border px-4 py-2">강의 + 스터디</td>
					<td data-th="border px-4 py-2">보안 기초 + 실사례 문제 분석</td>
					<td data-th="border px-4 py-2"></td>
					<td data-th="border px-4 py-2">매주 토 22~23시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">유니티</td>
					<td data-th="border px-4 py-2">강은호 & (부)박상민 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">예제를 중심으로 배우는 Unity 기초부터 실습까지</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1NC0P-FZkoe4KyZSWQhIsme1S-83ACzb2hBVVS1z1THA/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">매주 목 20~24시, 토일 10~15시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">알고리즘</td>
					<td data-th="border px-4 py-2">김민상 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">백준 그룹에서 매주 실력별 문제 제공 + 풀이</td>
					<td data-th="border px-4 py-2"><a href="https://www.acmicpc.net/group/18313" target="_blank">백준 그룹 신청 Link</a></td>
					<td data-th="border px-4 py-2">매주 일요일 22~23시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">백엔드</td>
					<td data-th="border px-4 py-2">이수영 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">Java & Spring Boot로 구현하는 웹 게시판</td>
					<td data-th="border px-4 py-2"><a href="https://piquant-increase-d76.notion.site/Spring-Boot-Study-3d499f17532142a69caf22a2a43bcfcc?pvs=4" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">화목토 21~22시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">플러터</td>
					<td data-th="border px-4 py-2">김현우 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">플러터를 활용해서 투두 앱 만들기</td>
					<td data-th="border px-4 py-2"><a href="https://coalery.notion.site/SUSC-2023S-Flutter-954a0f619ca94a68920e020461e9403f" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">토일 21~24시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">머신러닝 딥러닝 Basic</td>
					<td data-th="border px-4 py-2">데보션 박정환 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">머신러닝/딥러닝 이론 및 실습</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1_ekljyrGLFMFiGZhTnd-xd8Pf497IVvLrcBGzrIX_84/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">데보션 API (디스코드 봇)</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">NLP</td>
					<td data-th="border px-4 py-2">데보션 윤주성 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">Text preprocessing부터 GPT까지</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1q-tnYEn8MSOub7WbS99r_61x4fq-2fU5B5FBzKFdZMU/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">데보션 API (디스코드 봇)</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">CV</td>
					<td data-th="border px-4 py-2">추영욱 & 이준원 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">OpenCV를 활용한 컴퓨터비전 기초부터 활용까지</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/15OvnnvtJoMffhHH8cO83KuX_Kg3Y8OCrNN7zMRcmbMA/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">상시 (신청 형태)</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">AI 논문리딩</td>
					<td data-th="border px-4 py-2">이준원 멘토</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">효과적인 논문 읽는법, 논문탐색 방법</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1FgXdtdq1KLUUokQtxYMN3MOdAwTShl5h693Me7wiQ6A/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">화목토 15시~16시</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">C++</td>
					<td data-th="border px-4 py-2">운영진</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">C++ 기초 및 STL 기초</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1WlslcfPm5PFhMBs96AAMcU80EQQJzLq_LDnslzg8dKs/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">상시 (신청 형태)</td>
				  </tr>
				  <tr>
					<td data-th="border px-4 py-2">Python</td>
					<td data-th="border px-4 py-2">운영진</td>
					<td data-th="border px-4 py-2">스터디</td>
					<td data-th="border px-4 py-2">Python 기초 및 기본 자료구조</td>
					<td data-th="border px-4 py-2"><a href="https://docs.google.com/spreadsheets/d/1CkQqjKJ_PnUm7yMUBK2YVpRN4DgSPDdqs1NuKZ7_zr4/edit?usp=sharing" target="_blank">Link</a></td>
					<td data-th="border px-4 py-2">상시 (신청 형태)</td>
				  </tr>
				</tbody>
			  </table>
		</div>
		
	</div>
</div>
