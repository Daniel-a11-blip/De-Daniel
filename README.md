<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Para Sarita 🌻</title>

<style>

* {
    box-sizing: border-box;
}

html, body {
    margin: 0;
    width: 100%;
    min-height: 100%;
}

body {
    overflow: hidden;
    font-family: Georgia, "Times New Roman", serif;
    background:
        radial-gradient(circle at 50% 25%, #fff8cf 0%, transparent 25%),
        linear-gradient(180deg, #8ed8f5 0%, #dff5f4 70%, #91bd63 70%, #6d9f4c 100%);
}

/* Pantalla */

.pantalla {
    width: 100%;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
}

/* Tarjeta */

.tarjeta {
    width: min(92%, 430px);
    padding: 35px 25px 30px;
    text-align: center;
    position: relative;
    z-index: 5;
}

.nombre {
    font-size: clamp(38px, 11vw, 58px);
    color: #6f4a18;
    margin: 0 0 8px;
    font-weight: normal;
    letter-spacing: 1px;
}

.subtitulo {
    color: #80632f;
    font-size: 17px;
    margin-bottom: 15px;
}

/* Girasol principal */

.girasol {
    width: 250px;
    height: 250px;
    margin: 0 auto 8px;
    position: relative;
    animation: balanceo 5s ease-in-out infinite;
}

.petalo {
    position: absolute;
    width: 43px;
    height: 100px;
    background: linear-gradient(#ffe44c, #f7bd18);
    border-radius: 50%;
    left: 104px;
    top: 20px;
    transform-origin: 21px 105px;
}

.p1 { transform: rotate(0deg); }
.p2 { transform: rotate(30deg); }
.p3 { transform: rotate(60deg); }
.p4 { transform: rotate(90deg); }
.p5 { transform: rotate(120deg); }
.p6 { transform: rotate(150deg); }
.p7 { transform: rotate(180deg); }
.p8 { transform: rotate(210deg); }
.p9 { transform: rotate(240deg); }
.p10 { transform: rotate(270deg); }
.p11 { transform: rotate(300deg); }
.p12 { transform: rotate(330deg); }

.centro {
    position: absolute;
    width: 92px;
    height: 92px;
    background:
        radial-gradient(circle at 35% 30%, #a66b1c, #70400c 70%);
    border-radius: 50%;
    left: 79px;
    top: 79px;
    box-shadow: inset 0 0 0 5px rgba(75,40,5,.18);
}

/* Semillas */

.semilla {
    position: absolute;
    width: 6px;
    height: 6px;
    background: #4e2d08;
    border-radius: 50%;
}

.s1 { left: 105px; top: 105px; }
.s2 { left: 128px; top: 98px; }
.s3 { left: 150px; top: 110px; }
.s4 { left: 100px; top: 130px; }
.s5 { left: 125px; top: 125px; }
.s6 { left: 150px; top: 135px; }
.s7 { left: 112px; top: 150px; }
.s8 { left: 138px; top: 153px; }

/* Tallo */

.tallo {
    position: absolute;
    width: 13px;
    height: 145px;
    background: linear-gradient(90deg, #3e7931, #59943e);
    left: 118px;
    top: 185px;
    border-radius: 10px;
    z-index: -1;
}

/* Hojas */

.hoja {
    position: absolute;
    width: 85px;
    height: 35px;
    background: #4d9139;
    border-radius: 100% 0 100% 0;
    top: 255px;
}

.hoja.izquierda {
    left: 50px;
    transform: rotate(25deg);
}

.hoja.derecha {
    right: 50px;
    transform: scaleX(-1) rotate(25deg);
}

/* Botón */

button {
    border: none;
    background: #f3bd24;
    color: #5c3d08;
    font-family: Georgia, serif;
    font-size: 17px;
    padding: 13px 25px;
    border-radius: 30px;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(100,70,10,.18);
    transition: transform .2s, background .2s;
}

button:active {
    transform: scale(.94);
}

button:hover {
    background: #ffd447;
}

/* Mensaje oculto */

.mensaje {
    max-height: 0;
    opacity: 0;
    overflow: hidden;
    transition: all .7s ease;
    color: #6b4b1b;
    font-size: 18px;
    line-height: 1.6;
}

.mensaje.visible {
    max-height: 180px;
    opacity: 1;
    margin-top: 20px;
}

/* Pétalos que caen */

.caido {
    position: fixed;
    top: -30px;
    font-size: 22px;
    pointer-events: none;
    animation: caer linear forwards;
    z-index: 20;
}

@keyframes caer {
    to {
        transform:
            translateY(110vh)
            rotate(360deg);
        opacity: 0;
    }
}

@keyframes balanceo {

    0%, 100% {
        transform: rotate(-2deg);
    }

    50% {
        transform: rotate(2deg);
    }
}

/* Celular */

@media (max-width: 450px) {

    .tarjeta {
        padding-top: 20px;
    }

    .nombre {
        font-size: 43px;
    }

    .subtitulo {
        font-size: 15px;
    }

    .girasol {
        transform: scale(.82);
        margin-top: -5px;
        margin-bottom: -25px;
    }

    button {
        font-size: 16px;
    }
}

</style>
</head>

<body>

<div class="pantalla">

    <div class="tarjeta">

        <h1 class="nombre">Sarita</h1>

        <div class="subtitulo">
            Una pequeña sorpresa para ti 🌻
        </div>

        <div class="girasol">

            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="petalo p7"></div>
            <div class="petalo p8"></div>
            <div class="petalo p9"></div>
            <div class="petalo p10"></div>
            <div class="petalo p11"></div>
            <div class="petalo p12"></div>

            <div class="centro"></div>

            <div class="semilla s1"></div>
            <div class="semilla s2"></div>
            <div class="semilla s3"></div>
            <div class="semilla s4"></div>
            <div class="semilla s5"></div>
            <div class="semilla s6"></div>
            <div class="semilla s7"></div>
            <div class="semilla s8"></div>

            <div class="tallo"></div>
            <div class="hoja izquierda"></div>
            <div class="hoja derecha"></div>

        </div>

        <button id="boton">
            Toca aquí 🌻
        </button>

        <div class="mensaje" id="mensaje">
            Que estas flores puedan sacarte una sonrisa
            y alegrarte un poquito el día. 💛
        </div>

    </div>

</div>

<script>

const boton = document.getElementById("boton");
const mensaje = document.getElementById("mensaje");

boton.addEventListener("click", () => {

    mensaje.classList.toggle("visible");

    if (mensaje.classList.contains("visible")) {
        boton.textContent = "🌻 Para Sarita 🌻";
        crearPetalos();
    } else {
        boton.textContent = "Toca aquí 🌻";
    }

});

function crearPetalos() {

    for (let i = 0; i < 18; i++) {

        const petalo = document.createElement("div");

        petalo.className = "caido";
        petalo.textContent = "🌻";

        petalo.style.left =
            Math.random() * 100 + "%";

        petalo.style.animationDuration =
            (3 + Math.random() * 3) + "s";

        petalo.style.animationDelay =
            Math.random() * 1.5 + "s";

        document.body.appendChild(petalo);

        setTimeout(() => {
            petalo.remove();
        }, 7000);
    }
}

</script>

</body>
</html>
