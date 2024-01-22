---
toc: true
comments: true
layout: base
title: map
author: luna and tanisha 
permalink: /map
---
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Game Map</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
        }

        .map {
            position: relative;
            width: 100vw;
            height: 100vh;
            background-color: #87CEEB; /* Blue color for the ocean background */
            cursor: pointer;
        }

        .island {
            position: absolute;
            width: 150px;
            height: 150px;
            background-image: url('images/island.png'); /* Path to your island image */
            background-size: cover;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .island-name {
            color: #fff;
            font-weight: bold;
            font-size: 12px;
            font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
            text-align: center;
            position: absolute;
            bottom: -20px; /* Adjust the distance between the island and the name */
            width: 100%; /* Ensure full width */
            transition: color 0.3s;
        }

        .island:hover {
            font-family: 'Courier New', Courier, monospace;
        }

        .island:hover .island-name {
            color: #CD853F; 
        }
    </style>
</head>
<body>
    <div class="map">
        <div class="island" style="top: 100px; left: 150px;">
            <div class="island-name">Chemistry Island</div>
        </div>
        <div class="island" style="top: 220px; left: 450px;">
            <div class="island-name">Calculus Island</div>
        </div>
        <div class="island" style="top: 400px; left: 250px;">
            <div class="island-name">CSA Island</div>
        </div>
        <div class="island" style="top: 500px; left: 550px;">
            <div class="island-name">Physics Island</div>
        </div>
    </div>
</body>
</html>
