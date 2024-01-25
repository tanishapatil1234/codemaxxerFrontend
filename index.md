---
layout: index
search_exclude: true
--- 
<div class="card">
    <h1>Rift</h1>
    <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
</div>
<br>
<div class="card">
    <h3>Explain</h3>
    <p>lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem ipsum</p>
</div>
<br>
<div class="card">
    <h3>Login</h3>
    <h5>Username</h5>
    <input>
    <br>    
    <h5>Password</h5>
    <input>
    <br>
    <br>
    <button>Login</button>
    <button id="transfer">Sign Up</button>
</div>

<script>
    document.addEventListener("DOMContentLoaded", function() {

    var transferButton = document.getElementById("transfer");

    transferButton.addEventListener("click", function() {
        window.location.href = "{{site.baseurl}}/signup";
    });
});
</script>