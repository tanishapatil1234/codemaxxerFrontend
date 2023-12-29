---
toc: true
comments: true
layout: post
title: Helper AI
author: Finn C
---


<div class="chatbox">
    <div class="chat" id="chat">
        <p class="AI">lorem</p>
        <p class="User">lorem</p>
    </div>
    <div class="question">
        <input class="AI-input" id="question">
        <button class="send" id="send" onclick="Send()">Send</button>
    </div>
</div>

<script>
    function Send() {
        var input = document.getElementById('question').value;
        //Check if there is no input
        if (!input) {
            return;
        }
        var Chat = document.getElementById("chat");
        var UserChat = `<p class="User">${input}<p>`;
        Chat.innerHTML = Chat.innerHTML + UserChat;
    }
</script>
