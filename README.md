<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Simelwe ❤️</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    width: 100%;
    min-height: 100vh;
    background: #050008;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    font-family: Arial, sans-serif;
}

.scene {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    perspective: 1000px;
}

.heart-container {
    width: min(90vw, 390px);
    aspect-ratio: 1;
    position: relative;
    animation: float 4s ease-in-out infinite;
}

.heart-svg {
    width: 100%;
    height: 100%;
    overflow: visible;
    animation: turn 12s ease-in-out infinite;
    transform-style: preserve-3d;
}

.heart-words {
    fill: #ffacd5;
    font-family: Arial, sans-serif;
    font-size: 12px;
    font-weight: bold;
    letter-spacing: 1.4px;
    filter: drop-shadow(0 0 4px #ff1493);
}

.heart-words.inner {
    fill: #ff69b4;
    font-size: 10px;
    letter-spacing: 1px;
    opacity: 0.9;
}

.center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 75%;
    text-align: center;
    pointer-events: none;
}

.center h1 {
    color: #ffacd5;
    font-family: cursive;
    font-size: clamp(25px, 7vw, 35px);
    text-shadow:
        0 0 8px #ff1493,
        0 0 20px #ff1493;
    animation: pulse 2s infinite;
}

.center p {
    color: #fff0f7;
    font-size: 10px;
    letter-spacing: 2px;
    line-height: 2;
    margin-top: 8px;
    text-shadow: 0 0 8px #ff69b4;
}

.bottom-message {
    color: #ffacd5;
    font-family: cursive;
    font-size: 17px;
    text-align: center;
    margin-top: 5px;
    text-shadow: 0 0 12px #ff1493;
}

@keyframes turn {
    0%, 100% {
        transform: rotateY(-12deg) rotateX(5deg);
    }
    50% {
        transform: rotateY(12deg) rotateX(-5deg);
    }
}

@keyframes float {
    0%, 100% {
        translate: 0 0;
    }
    50% {
        translate: 0 -8px;
    }
}

@keyframes pulse {
    0%, 100% {
        scale: 1;
    }
    50% {
        scale: 1.06;
    }
}

@media (prefers-reduced-motion: reduce) {
    .heart-svg,
    .heart-container,
    .center h1 {
        animation: none;
    }
}
</style>
</head>

<body>

<div class="scene">

    <div class="heart-container">

        <svg class="heart-svg"
             viewBox="0 0 400 400"
             xmlns="http://www.w3.org/2000/svg">

            <defs>
                <!-- Outer heart path -->
                <path id="outerHeart"
                    d="M200 340
                       C170 310 40 225 40 130
                       C40 45 145 25 200 105
                       C255 25 360 45 360 130
                       C360 225 230 310 200 340 Z" />

                <!-- Inner heart path -->
                <path id="innerHeart"
                    d="M200 285
                       C175 260 85 200 85 140
                       C85 85 150 75 200 125
                       C250 75 315 85 315 140
                       C315 200 225 260 200 285 Z" />
            </defs>

            <!-- Soft heart outline -->
            <use href="#outerHeart"
                 fill="none"
                 stroke="#ff1493"
                 stroke-width="1"
                 opacity="0.45" />

            <!-- Clear words around the outside -->
            <text class="heart-words">
                <textPath href="#outerHeart"
                          startOffset="0%">
                    I LOVE YOU SIMELWE ♥ I LOVE YOU SIMELWE ♥
                </textPath>
            </text>

            <!-- Smaller heart with fewer words -->
            <text class="heart-words inner">
                <textPath href="#innerHeart"
                          startOffset="0%">
                    I LOVE YOU ♥ I LOVE YOU ♥
                </textPath>
            </text>

        </svg>

        <!-- Message in the center -->
        <div class="center">
            <h1>Simelwe ❤️</h1>
            <p>YOU ARE SPECIAL TO ME</p>
            <p>FOREVER & ALWAYS</p>
        </div>

    </div>

    <div class="bottom-message">
        Made with love, just for you 💗
    </div>

</div>

</body>
</html># Simelwe
