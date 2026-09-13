# Cx
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Priya ❤️</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    min-height: 100vh;
    overflow: hidden;
}

.slide {
    display: none;
    height: 100vh;
    width: 100%;
    text-align: center;
    padding: 40px 20px;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    animation: fade 0.8s;
}

.slide.active {
    display: flex;
}

h1 {
    font-size: 42px;
    color: white;
    margin-bottom: 20px;
    text-shadow: 2px 2px 5px #777;
}

p {
    font-size: 22px;
    color: white;
    max-width: 600px;
    line-height: 1.6;
}

.heart {
    font-size: 80px;
    animation: beat 1s infinite;
}

button {
    margin-top: 35px;
    padding: 14px 30px;
    border: none;
    border-radius: 30px;
    background: white;
    color: #ff4f81;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
}

button:hover {
    transform: scale(1.05);
}

.photo {
    width: 260px;
    height: 260px;
    object-fit: cover;
    border-radius: 50%;
    border: 7px solid white;
    box-shadow: 0 5px 25px rgba(0,0,0,0.3);
    margin-bottom: 25px;
}

@keyframes beat {
    50% { transform: scale(1.2); }
}

@keyframes fade {
    from { opacity: 0; }
    to { opacity: 1; }
}

.confetti {
    font-size: 55px;
    margin: 20px;
}
</style>
</head>

<body>

<!-- Slide 1 -->
<section class="slide active">
    <div class="heart">❤️</div>
    <h1>Hey Priya!</h1>
    <p>Someone very special has a birthday today...</p>
    <button onclick="nextSlide()">Open Your Surprise 💌</button>
</section>

<!-- Slide 2 -->
<section class="slide">
    <div class="heart">🎂</div>
    <h1>Happy Birthday!</h1>
    <p>
        Wish you a very very happy birthday, Priya! 🥳❤️
    </p>
    <button onclick="nextSlide()">Next ❤️</button>
</section>

<!-- Slide 3 -->
<section class="slide">
    <div class="heart">🌸</div>
    <h1>My Favourite</h1>
    <p>
        You are not just special...<br>
        You are my favourite person. ❤️
    </p>
    <button onclick="nextSlide()">Next ✨</button>
</section>

<!-- Slide 4 -->
<section class="slide">
    <div class="confetti">🎉 🎈 🎉</div>
    <h1>Today Is Your Day!</h1>
    <p>
        May your smile always stay this beautiful,<br>
        and may every dream of yours come true. ✨
    </p>
    <button onclick="nextSlide()">Next 💖</button>
</section>

<!-- Slide 5 -->
<section class="slide">
    <div class="heart">💖</div>
    <h1>For You, Priya</h1>
    <p>
        Keep smiling, keep shining,<br>
        and always remember how special you are. 🌷
    </p>
    <button onclick="nextSlide()">One More ❤️</button>
</section>

<!-- Slide 6 -->
<section class="slide">
    <div class="confetti">🎂 🎉 💕 🎉 🎂</div>
    <h1>Happy Birthday Priya! ❤️</h1>
    <p>
        Wish you a very very happy birthday! 🥳<br><br>
        Stay happy. Stay beautiful. Stay amazing. ❤️
    </p>
    <div class="heart">💝</div>
</section>

<script>
let currentSlide = 0;
const slides = document.querySelectorAll(".slide");

function nextSlide() {
    slides[currentSlide].classList.remove("active");

    currentSlide++;

    if (currentSlide >= slides.length) {
        currentSlide = 0;
    }

    slides[currentSlide].classList.add("active");
}
</script>

</body>
</html>
