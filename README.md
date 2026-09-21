<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Para Sarita 🌻</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Pacifico&display=swap" rel="stylesheet">

<style>

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    overflow: hidden;

    font-family: "DM Sans", sans-serif;

    background:
        radial-gradient(circle at 20% 20%, #fff6b8 0%, transparent 25%),
        radial-gradient(circle at 80% 80%, #ffe58a 0%, transparent 25%),
        linear-gradient(135deg, #fffdf0, #fff4c7);

    display: flex;
    justify-content: center;
    align-items: center;
}

/* FONDO */

.luz {
    position: fixed;
    width: 300px;
    height: 300px;
    border-radius: 50%;

    background: rgba(255, 218, 70, .15);

    filter: blur(40px);

    animation: mover 7s ease-in-out infinite alternate;
}

.luz1 {
    top: -100px;
    left: -100px;
}

.luz2 {
    bottom: -120px;
    right: -100px;
    animation-delay: 2s;
}

@keyframes mover {
    from {
        transform: translate(0,0);
    }

    to {
        transform: translate(50px,30px);
    }
}

/* TARJETA */

.card {

    width: min(90%, 420px);

    padding: 42px 25px 35px;

    text-align: center;

    background: rgba(255,255,255,.72);

    backdrop-filter: blur(15px);

    border: 1px solid rgba(255,255,255,.9);

    border-radius: 32px;

    box-shadow:
        0 20px 60px rgba(160,120,20,.15);

    position: relative;

    z-index: 2;

    animation: aparecer .9s ease;
}

@keyframes aparecer {

    from {
        opacity: 0;
        transform: translateY(25px) scale(.96);
    }

    to {
        opacity: 1;
        transform: translateY(0) scale(1);
    }
}

/* NOMBRE */

.nombre {

    margin: 0;

    font-family: "Pacifico", cursive;

    font-size: clamp(45px, 13vw, 65px);

    font-weight: normal;

    color: #d99a00;

    text-shadow:
        2px 3px 0 #ffe9a0;

    line-height: 1.2;
}

/* TEXTO */

.subtitulo {

    margin-top: 8px;

    font-size: 15px;

    color: #77705e;

    letter-spacing: .3px;
}

/* FLOR */

.flor {

    width: 210px;
    height: 210px;

    margin: 25px auto 20px;

    position: relative;

    animation: flotar 4s ease-in-out infinite;
}

@keyframes flotar {

    0%,100% {
        transform: translateY(0) rotate(-2deg);
    }

    50% {
        transform: translateY(-8px) rotate(2deg);
    }
}

/* PÉTALOS */

.petalo {

    position: absolute;

    width: 48px;
    height: 88px;

    left: 81px;
    top: 8px;

    border-radius: 50%;

    background: linear-gradient(
        180deg,
        #ffe96a,
        #f5b900
    );

    transform-origin: center 97px;

    box-shadow:
        0 4px 10px rgba(200,140,0,.12);
}

.p1  { transform: rotate(0deg); }
.p2  { transform: rotate(30deg); }
.p3  { transform: rotate(60deg); }
.p4  { transform: rotate(90deg); }
.p5  { transform: rotate(120deg); }
.p6  { transform: rotate(150deg); }
.p7  { transform: rotate(180deg); }
.p8  { transform: rotate(210deg); }
.p9  { transform: rotate(240deg); }
.p10 { transform: rotate(270deg); }
.p11 { transform: rotate(300deg); }
.p12 { transform: rotate(330deg); }

/* CENTRO */

.centro {

    position: absolute;

    width: 82px;
    height: 82px;

    left: 64px;
    top: 64px;

    border-radius: 50%;

    background:
        radial-gradient(
            circle at 35% 30%,
            #9c661e,
            #5e350b
        );

    box-shadow:
        inset 0 0 0 5px rgba(50,25,0,.15),
        0 5px 15px rgba(80,40,0,.2);

    z-index: 2;
}

/* TALLO */

.tallo {

    position: absolute;

    width: 11px;
    height: 100px;

    left: 99px;
    top: 135px;

    background: #4f963e;

    border-radius: 20px;

    z-index: -1;
}

/* HOJAS */

.hoja {

    position: absolute;

    width: 65px;
    height: 30px;

    background: #65a94b;

    border-radius: 100% 0 100% 0;

    top: 175px;
}

.izq {
    left: 35px;
    transform: rotate(25deg);
}

.der {
    right: 35px;
    transform: scaleX(-1) rotate(25deg);
}

/* BOTÓN */

button {

    border: none;

    padding: 14px 28px;

    border-radius: 50px;

    background: linear-gradient(
        135deg,
        #ffd83d,
        #f5b900
    );

    color: #684900;

    font-family: "DM Sans", sans-serif;

    font-size: 16px;

    font-weight: 700;

    cursor: pointer;

    box-shadow:
        0 8px 20px rgba(220,160,0,.25);

    transition: .25s;
}

button:hover {

    transform: translateY(-3px);

    box-shadow:
        0 12px 25px rgba(220,160,0,.32);
}

button:active {

    transform: scale(.94);
}

/* MENSAJE */

.mensaje {

    max-height: 0;

    overflow: hidden;

    opacity: 0;

    margin-top: 0;

    color: #665c48;

    font-size: 16px;

    line-height: 1.6;

    transition:
