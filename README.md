<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>🌻 Para ti</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    overflow: hidden;
    font-family: Georgia, serif;
    background: linear-gradient(
        180deg,
        #bde9ff 0%,
        #eaf8ff 65%,
        #b7d98a 65%,
        #82b45c 100%
    );
}

/* Mensaje */

.mensaje {
    position: absolute;
    top: 45px;
    left: 0;
    width: 100%;
    text-align: center;
    color: #72501c;
    font-size: clamp(24px, 6vw, 38px);
    font-weight: bold;
    z-index: 10;
    text-shadow: 0 2px 4px rgba(255,255,255,.7);
}

/* Jardín */

.jardin {
    position: absolute;
    inset: 0;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    padding-bottom: 3vh;
}

/* SVG */

svg {
    width: min(700px, 100vw);
    height: min(650px, 78vh);
}

/* Movimiento suave */

.girasol {
    transform-box: fill-box;
    transform-origin: bottom center;
    animation: viento 5s ease-in-out infinite;
}

.girasol:nth-of-type(2) {
    animation-delay: .8s;
}

.girasol:nth-of-type(3) {
    animation-delay: 1.5s;
}

@keyframes viento {

    0%, 100% {
        transform: rotate(-1deg);
    }

    50% {
        transform: rotate(1deg);
    }
}
</style>
</head>

<body>

<div class="mensaje">
    🌻 Para ti 🌻
</div>

<div class="jardin">

<svg viewBox="0 0 700 650"
     xmlns="http://www.w3.org/2000/svg">

<!-- SUELO -->

<path
    d="M0 590 Q175 555 350 590 T700 590 V650 H0Z"
    fill="#78a94f"/>

<path
    d="M0 615 Q180 580 350 615 T700 615 V650 H0Z"
    fill="#699745"/>


<!-- GIRASOL IZQUIERDO -->

<g class="girasol">

    <!-- tallo -->
    <path
        d="M170 620
           C168 500 170 390 190 275"
        fill="none"
        stroke="#43843a"
        stroke-width="11"
        stroke-linecap="round"/>

    <!-- hoja -->
    <path
        d="M170 490
           C115 450 82 475 100 505
           C120 535 160 525 180 500Z"
        fill="#4d963f"/>

    <path
        d="M145 492 Q130 490 110 492"
        fill="none"
        stroke="#367a32"
        stroke-width="3"/>


    <!-- flor -->

    <g transform="translate(190 250)">

        <!-- pétalos traseros -->
        <g fill="#f7c928">

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(30)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(60)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(90)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(120)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(150)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(180)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(210)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(240)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(270)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(300)"/>

            <ellipse cx="0" cy="-72"
                     rx="25" ry="72"
                     transform="rotate(330)"/>

        </g>

        <!-- pétalos delanteros -->
        <g fill="#ffd83d">

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"/>

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"
                     transform="rotate(60)"/>

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"
                     transform="rotate(120)"/>

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"
                     transform="rotate(180)"/>

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"
                     transform="rotate(240)"/>

            <ellipse cx="0" cy="-55"
                     rx="20" ry="58"
                     transform="rotate(300)"/>

        </g>

        <!-- centro -->
        <circle r="48" fill="#75420d"/>

        <circle r="38" fill="#8d5313"/>

        <!-- semillas -->
        <g fill="#55300b">

            <circle cx="-18" cy="-15" r="3"/>
            <circle cx="0" cy="-21" r="3"/>
            <circle cx="18" cy="-13" r="3"/>

            <circle cx="-25" cy="4" r="3"/>
            <circle cx="-8" cy="3" r="3"/>
            <circle cx="10" cy="4" r="3"/>
            <circle cx="26" cy="5" r="3"/>

            <circle cx="-17" cy="22" r="3"/>
            <circle cx="2" cy="21" r="3"/>
            <circle cx="20" cy="21" r="3"/>

        </g>

    </g>

</g>


<!-- GIRASOL CENTRAL -->

<g class="girasol">

    <!-- tallo -->
    <path
        d="M350 630
           C350 500 350 365 350 220"
        fill="none"
        stroke="#43843a"
        stroke-width="13"
        stroke-linecap="round"/>

    <!-- hoja izquierda -->
    <path
        d="M350 485
           C285 440 250 470 270 505
           C295 535 330 520 355 495Z"
        fill="#4d963f"/>

    <!-- nervadura -->
    <path
        d="M350 490 Q305 480 275 490"
        fill="none"
        stroke="#367a32"
        stroke-width="3"/>

    <!-- hoja derecha -->
    <path
        d="M350 405
           C415 360 450 390 430 425
           C405 450 370 435 350 415Z"
        fill="#4d963f"/>


    <!-- flor -->

    <g transform="translate(350 195)">

        <!-- pétalos -->
        <g fill="#f7c928">

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(30)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(60)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(90)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(120)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(150)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(180)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(210)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(240)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(270)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(300)"/>

            <ellipse cx="0" cy="-82"
                     rx="28" ry="82"
                     transform="rotate(330)"/>

        </g>

        <!-- centro -->
        <circle r="55" fill="#70400b"/>
        <circle r="44" fill="#8c5312"/>

        <!-- semillas -->
        <g fill="#56310a">

            <circle cx="-20" cy="-20" r="3"/>
            <circle cx="0" cy="-27" r="3"/>
            <circle cx="20" cy="-18" r="3"/>

            <circle cx="-28" cy="0" r="3"/>
            <circle cx="-10" cy="0" r="3"/>
            <circle cx="10" cy="0" r="3"/>
            <circle cx="28" cy="0" r="3"/>

            <circle cx="-18" cy="21" r="3"/>
            <circle cx="0" cy="25" r="3"/>
            <circle cx="19" cy="20" r="3"/>

        </g>

    </g>

</g>


<!-- GIRASOL DERECHO -->

<g class="girasol">

    <!-- tallo -->
    <path
        d="M530 625
           C530 500 530 395 505 285"
        fill="none"
        stroke="#43843a"
        stroke-width="11"
        stroke-linecap="round"/>

    <!-- hoja -->
    <path
        d="M530 500
           C585 460 615 485 600 515
           C580 540 545 530 525 510Z"
        fill="#4d963f"/>

    <!-- flor -->

    <g transform="translate(505 260)">

        <g fill="#f7c928">

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(30)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(60)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(90)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(120)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(150)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(180)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(210)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(240)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(270)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(300)"/>

            <ellipse cx="0" cy="-70"
                     rx="24" ry="70"
                     transform="rotate(330)"/>

        </g>

        <circle r="46" fill="#75420d"/>
        <circle r="36" fill="#8d5313"/>

        <g fill="#55300b">

            <circle cx="-17" cy="-14" r="3"/>
            <circle cx="0" cy="-20" r="3"/>
            <circle cx="17" cy="-14" r="3"/>

            <circle cx="-23" cy="3" r="3"/>
            <circle cx="-7" cy="2" r="3"/>
            <circle cx="9" cy="3" r="3"/>
            <circle cx="23" cy="4" r="3"/>

            <circle cx="-15" cy="19" r="3"/>
            <circle cx="2" cy="20" r="3"/>
            <circle cx="18" cy="18" r="3"/>

        </g>

    </g>

</g>

</svg>

</div>

</body>
</html>
