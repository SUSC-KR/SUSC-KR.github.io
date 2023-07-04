<script>
	import Test from './Test.svelte';
</script>

<div class=" bg-base-300 p-4 xl:p-10 rounded-lg">
	<div class="max-w-lg mx-auto pb-10">
		<div class="text-3xl font-bold text-center my-5">운영진 소개</div>
		<!-- <div class="text-lg text-center my-5">
			Voluptate eiusmod quis do aliquip labore esse pariatur excepteur dolore do fugiat sint
			officia. Commodo non est ullamco consectetur dolore excepteur.
		</div> -->
	</div>
	

	<div class="bg-color:gray flex flex-col lg:flex-row justify-center gap-5 xl:gap-10">
		<div class="flex flex-col justify-between bg-base-100 rounded-lg w-[60%] shadow-lg">
			<div class="flex items-center justify-center p-2 lg:container lg:mx-auto">
				<div class="">
					<a href="#" class="font-bold text-primary text-2xl">Github Chat</a>
				</div>
			</div>
			<hr>
			<div class="p-4 xl:p-10">
				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/63298243?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						이준원
						<time class="text-xs opacity-50">12:45</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/cpprhtn" class="underline" target="_blank">@cpprhtn</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/54111883?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						추영욱
						<time class="text-xs opacity-50">12:48</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/choo121600" class="underline" target="_blank">@choo121600</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/25046121?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						김현우
						<time class="text-xs opacity-50">12:48</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/Coalery" class="underline" target="_blank">@Coalery</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/52674782?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						이지성
						<time class="text-xs opacity-50">12:48</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/easycastle" class="underline" target="_blank">@easycastle</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/65693861?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						박정식
						<time class="text-xs opacity-50">12:48</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/sat0317" class="underline" target="_blank">@sat0317</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://avatars.githubusercontent.com/u/79389316?v=4"
							/>
						</div>
					</div>
					<div class="chat-header">
						정재현
						<time class="text-xs opacity-50">12:48</time>
					</div>
					<div class="chat-bubble"><a href="https://github.com/SeoLanee" class="underline" target="_blank">@SeoLanee</a></div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<Test/>

			</div>
		</div>
		<!-- <div class="flex flex-col justify-between bg-base-100 rounded-lg w-full shadow-lg">
			<div class="p-4 xl:p-10">
				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1550525811-e5869dd03032?ixlib=rb-1.2.1&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Ada Lovelace
						<time class="text-xs opacity-50">12:45</time>
					</div>
					<div class="chat-bubble">Hello world</div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-end">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Anakin
						<time class="text-xs opacity-50">12:46</time>
					</div>
					<div class="chat-bubble bg-primary">I hate you!</div>
					<div class="chat-footer opacity-50">Seen at 12:46</div>
				</div>

				<div class="chat chat-end">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Anakin
						<time class="text-xs opacity-50">12:46</time>
					</div>
					<div class="chat-bubble bg-primary">I hate you!</div>
					<div class="chat-footer opacity-50">Seen at 12:46</div>
				</div>
			</div>
		</div>
		<div class="flex flex-col justify-between bg-base-100 rounded-lg w-full shadow-lg">
			<div class="p-4 xl:p-10">
				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Obi-Wan Kenobi
						<time class="text-xs opacity-50">12:45</time>
					</div>
					<div class="chat-bubble">Anakin</div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-start">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Obi-Wan Kenobi
						<time class="text-xs opacity-50">12:45</time>
					</div>
					<div class="chat-bubble">You were the Chosen One!</div>
					<div class="chat-footer opacity-50">Delivered</div>
				</div>

				<div class="chat chat-end">
					<div class="chat-image avatar">
						<div class="w-10 rounded-full">
							<img
								alt="avatar"
								src="https://images.unsplash.com/photo-1517365830460-955ce3ccd263?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
							/>
						</div>
					</div>
					<div class="chat-header">
						Anakin
						<time class="text-xs opacity-50">12:46</time>
					</div>
					<div class="chat-bubble bg-primary">I hate you!</div>
					<div class="chat-footer opacity-50">Seen at 12:46</div>
				</div>
			</div>
		</div> -->
	</div>
</div>
