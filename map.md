---
toc: true
comments: true
layout: base
title: map
author: luna
permalink: /map
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>codemaxxers Map</title>
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
            background-image: url('ocean.jpg'); /* Replace 'ocean.jpg' with your map background */
            background-size: cover;
            cursor: pointer;
        }

        .island {
            position: absolute;
            width: 100px; /* Adjust the size of the islands */
            height: 100px;
            background-color: #8B4513; /* Brown color for islands */
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            font-weight: bold;
            font-size: 12px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .island:hover {
            background-color: #CD853F; /* Lighter brown color on hover */
        }
    </style>
</head>
<body>
    <div class="map">
        <div class="island" style="top: 100px; left: 150px;">Chemistry Island</div>
        <div class="island" style="top: 250px; left: 400px;">Calculus Island</div>
        <div class="island" style="top: 400px; left: 250px;">CSA Island</div>
        <div class="island" style="top: 600px; left: 500px;">Physics Island</div>
    </div>
</body>
</html>
