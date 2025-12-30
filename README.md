<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year Akka</title>

<style>
body {
    margin: 0;
    height: 100vh;
    background: linear-gradient(-45deg, #ff758c, #ff7eb3, #fad0c4, #fbc2eb);
    background-size: 400% 400%;
    animation: bg 8s ease infinite;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: 'Segoe UI', sans-serif;
}

@keyframes bg {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
}

.card {
    background: rgba(255,255,255,0.95);
    width: 90%;
    max-width: 320px;
    padding: 20px;
    border-radius: 25px;
    box-shadow: 0 20px 40px rgba(0,0,0,0.3);
    text-align: center;
    animation: pop 1.2s ease;
}

@keyframes pop {
    from {transform: scale(0.7); opacity: 0;}
    to {transform: scale(1); opacity: 1;}
}

.photo-box {
    width: 100%;
    height: 380px;
    border-radius: 20px;
    overflow: hidden;
    cursor: pointer;
}

.photo-box img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
}

.photo-box:hover img {
    transform: scale(1.05);
}

.tap {
    font-size: 12px;
    color: #777;
    margin-top: 5px;
}

h1 {
    color: #e91e63;
    margin: 15px 0 10px;
}

p {
    font-size: 15px;
    color: #444;
    line-height: 1.5;
}

h2 {
    margin-top: 10px;
}
</style>
</head>

<body>

<div class="card">

    <!-- CLICKABLE IMAGE -->
    <div class="photo-box" onclick="changePhoto()">
        <img id="photo" src=" 1736849768046.jpg" alt="Akka">
        <img id="photo" src="IMG_20251017-WA0001.jpg" alt="Akka"
        <img id="photo" src="IMG_2025518_21594.jpg"alt="Akka"
    </div>
    <div class="tap">👆 Tap / Click photo</div>

    <h1>🎉 Happy New Year Akka 🎉</h1>

    <p>
        Dear Akka 🤍<br><br>
        This New Year brings you happiness,  
        health, success, and endless smiles 💖<br><br>
        Thank you for always being my strength ❤️
    </p>

    <h2>✨ 2025 ✨</h2>

</div>

<script>
let photos = ["IMG_2025518_21594.jpg", "IMG_20251017-WA0001.jpg", "1736849768046.jpg"];
let index = 0;

function changePhoto() {
    index = (index + 1) % photos.length;
    document.getElementById("photo").src = photos[index];
}
</script>

</body>
</html>
