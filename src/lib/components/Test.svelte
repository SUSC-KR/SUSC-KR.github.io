<script>
    import { onMount } from 'svelte';
  
    let message = '';
    let chatMessages = [];
  
    function sendMessage() {
      if (message.trim() === '') {
        return; // 입력 텍스트가 비어 있으면 전송하지 않음
      }
  
      chatMessages = [...chatMessages, message];
      message = '';
    }
  
    function handleKeyDown(event) {
      if (event.key === 'Enter') {
        event.preventDefault(); // 기본 동작 막기
  
        sendMessage();
      }
    }
  
    function handleInput(event) {
      const inputValue = event.target.value;
      const lastCharacter = inputValue.charAt(inputValue.length - 1);
  
      // 한글 입력을 막음
      if (/[ㄱ-ㅎㅏ-ㅣ가-힣]/.test(lastCharacter)) {
        message = inputValue.slice(0, -1);
      } else {
        message = inputValue;
      }
    }
  
    onMount(() => {
      const chatContainer = document.getElementById('chat-container');
      chatContainer.scrollTop = chatContainer.scrollHeight;
    });
  </script>
  
  <div class="chat-container" id="chat-container">
    {#each chatMessages as chatMessage, i}
    <div class="chat chat-end">
      <div class="chat-image avatar">
        <div class="w-10 rounded-full">
          <img
            alt="avatar"
            src="https://daisyui.com/images/stock/photo-1534528741775-53994a69daeb.jpg"
          />
        </div>
      </div>
      <div class="chat-header">
        you
        <time class="text-xs opacity-50">Now</time>
      </div>
      <div class="chat-bubble bg-primary"><a href="https://github.com/{chatMessage}" class="underline" target="_blank">{chatMessage}</a></div>
      </div>
    {/each}
  </div>
  
  <div>
    <input type="text" bind:value="{message}" placeholder="Github name" on:keydown="{handleKeyDown}" on:input="{handleInput}"/>
    <button on:click="{sendMessage}">Send</button>
  </div>