<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Just a Normal Page 😇</title>
    <style>
        body { 
            background-color: white; 
            text-align: center; 
            font-size: 24px;
        }
        #scary-img {
            display: none; 
            width: 100%; 
            height: 100vh;
            position: fixed;
            top: 0;
            left: 0;
        }
    </style>
</head>
<body>
    <p>Loading... please wait 😊</p>
    
    <img id="scary-img" src="https://i.imgur.com/QKb4aTh.jpg"> <!-- Scary Image -->
    <audio id="scream-sound" src="https://www.fesliyanstudios.com/play-mp3/4387" preload="auto"></audio> <!-- Loud Scream -->

    <script>
        setTimeout(() => {
            document.body.style.backgroundColor = "black"; 
            document.getElementById("scary-img").style.display = "block";
            document.getElementById("scream-sound").play();
        }, 3000); // 3-second delay before jumpscare
    </script>
</body>
</html>
