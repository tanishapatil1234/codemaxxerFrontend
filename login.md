---
layout: star
search_exclude: true
permalink: login
---
<body>
    <div class="banner">
        <div class="navbar">
            <img src="images/RIFTlogo.png" class="logo">
            <ul>
                <li><a href="{{site.baseurl}}/">Home</a></li>
                <li><a href="">Info</a></li>
                <li><a href="">Player Search</a></li>
                <li><a href="">About Us</a></li>
            </ul>
        </div>
    </div>
</body>

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

<style>
    .page-content {
        padding: 0px !important;
    }

    * {
        margin: 0;
        padding: 0;
        font-family: sans-serif;
    }


    .navbar {
        width: 85%;
        margin: auto;
        padding: 35px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .logo {
        width: 120px !important;
        height: auto !important;
    }

    .navbar ul li{
        list-style: none;
        display: inline-block;
        margin: 0 20px;
        position: relative;
    }

    .navbar ul li a{
        font-size: 16px;
        text-decoration: none;
        color: #fff;
        text-transform: uppercase;
    }

    .navbar ul li::after{
        content: '';
        height: 3px;
        width: 0;
        background: #2f80d0;
        position: absolute;
        left: 0;
        bottom: -10px;
        transition: ease-out .5s;
    }

    .navbar ul li:hover::after{
        width: 100%;
    }

    .content {
        width: 100%;
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        text-align: center;
        color: #fff;
    }

    .content h1{
        font-size: 120px;
        margin-top: 80px;
    }


    button{
        width: 200px;
        padding: 15px 0;
        text-align: center;
        margin: 20px 10px;
        font-weight: bold;
        border: 2px solid #2f80d0;
        background: transparent;
        color: #fff;
        cursor: pointer;
        position: relative;
        overflow: hidden;
        border-radius: 25px;
    }

    span{
        background-color: #2f80d0;
        height: 100%;
        width: 0;
        position: absolute;
        left: 0;
        bottom: 0;
        z-index: -1;
        border-radius: 0px;
    }

    button:hover span{
        width: 100%;
    }

    @keyframes transitionIn {
        from {
            opacity: 0;
        }

        to {
            opacity: 1;
        }
    }

    .content {
        animation: transitionIn 2s;
    }
</style>