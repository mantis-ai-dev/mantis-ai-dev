<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Just a Normal Page 😊</title>
    <style>
        body {
            background-color: white;
            text-align: center;
            font-size: 24px;
            padding: 20px;
            transition: background-color 0.5s ease-in-out;
        }
        #scary-img {
            display: none;
            width: 100vw;
            height: 100vh;
            position: fixed;
            top: 0;
            left: 0;
            object-fit: cover;
            z-index: 9999;
        }
    </style>
</head>
<body>
    <p>Loading... please wait 😊</p>
    
    <img id="scary-img" src="https://www.google.com/imgres?q=scary%20images&imgurl=https%3A%2F%2Fm.media-amazon.com%2Fimages%2FI%2F71u2nbcRpyS._AC_UY1100_.jpg&imgrefurl=https%3A%2F%2Fwww.amazon.in%2FHalloween-Smiling-Demons-Horrible-Cosume%2Fdp%2FB09B34HYXM&docid=M3M6BnZxbdAT1M&tbnid=GpmWc_aeLFxXKM&vet=12ahUKEwit9NTxw6yMAxW-sVYBHY-MMCcQM3oFCIIBEAA..i&w=1100&h=1100&hcb=2&ved=2ahUKEwit9NTxw6yMAxW-sVYBHY-MMCcQM3oFCIIBEAA"> <!-- Scary Image -->
    <audio id="scream-sound" src="https://www.fesliyanstudios.com/play-mp3/6666" preload="auto"></audio> <!-- Loud Scream -->

    <script>
        setTimeout(() => {
            document.body.style.backgroundColor = "black";
            document.getElementById("scary-img").style.display = "block";
            let audio = document.getElementById("scream-sound");
            audio.volume = 1.0;
            audio.play().catch(error => console.log("Autoplay failed: ", error));
        }, 3000); // Jumpscare triggers after 3 seconds
    </script>
</body>
</html>
