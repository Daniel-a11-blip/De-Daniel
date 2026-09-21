<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Flores amarillas 🌻</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    overflow: hidden;
    font-family: Arial, sans-serif;
    background: linear-gradient(#87CEEB 0%, #dff6ff 70%);
}

/* Mensaje */
h1 {
    text-align: center;
    margin-top: 60px;
    color: #6b4500;
    font-size: 28px;
}

/* Jardín */
.jardin {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 70%;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    gap: 35px;
}

/* Flor */
.flor {
    position: relative;
    width: 100px;
    height: 300px;
    animation: balanceo 3s ease-in-out infinite;
}

.flor:nth-child(2) {
    animation-delay: .5s;
}

.flor:nth-child(3) {
    animation-delay: 1s;
}

/* Cabeza */
.cabeza {
    position: absolute;
    top: 0;
    left: 10px;
    width: 80px;
    height: 80px;
}

/* Pétalos */
.petalo {
    position: absolute;
    width: 32px;
    height: 48px;
    background: #FFD21F;
    border-radius: 50%;
    left: 24px;
    top: 15px;
    transform-origin: 50% 100%;
}

.p1 { transform: rotate(0deg); }
.p2 { transform: rotate(60deg); }
.p3 { transform: rotate(120deg); }
.p4 { transform: rotate(180deg); }
.p5 { transform: rotate(240deg); }
.p6 { transform: rotate(300deg); }

/* Centro */
.centro {
    position: absolute;
    width: 32px;
    height: 32px;
    background: #8B5A00;
    border-radius: 50%;
    left: 24px;
    top: 25px;
    z-index: 5;
}

/* Tallo */
.tallo {
    position: absolute;
    width: 8px;
    height: 220px;
    background: #3b8c32;
    left: 46px;
    top: 70px;
    border-radius: 10px;
}

/* Hoja */
.hoja {
    position: absolute;
    width: 55px;
    height: 25px;
    background: #3b8c32;
    border-radius: 100% 0;
    left: 5px;
    top: 180px;
    transform: rotate(-25deg);
}

/* Suelo */
.suelo {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 100px;
    background: #5ca642;
}

/* Animación */
@keyframes balanceo {
    0%, 100% {
        transform: rotate(-2deg);
    }

    50% {
        transform: rotate(2deg);
    }
}

/* Celulares pequeños */
@media (max-width: 500px) {

    h1 {
        font-size: 23px;
        margin-top: 45px;
    }

    .jardin {
        gap: 5px;
        height: 65%;
    }

    .flor {
        transform: scale(.75);
        transform-origin: bottom center;
        margin: 0 -10px;
    }

    .suelo {
        height: 80px;
    }
}
</style>
</head>

<body>

<h1>🌻 Flores amarillas para ti 🌻</h1>

<div class="jardin">

    <div class="flor">
        <div class="cabeza">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

    <div class="flor">
        <div class="cabeza">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

    <div class="flor">
        <div class="cabeza">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

</div>

<div class="suelo"></div>

</body>
</html>       top: 12%;
        width: 100%;
        text-align: center;
        color: #5c3b00;
        font-size: 28px;
        font-weight: bold;
        z-index: 10;
    }

    .flor {
        position: absolute;
        bottom: 20%;
        width: 120px;
        height: 180px;
        animation: mover 3s ease-in-out infinite;
    }

    .flor1 {
        left: 15%;
    }

    .flor2 {
        left: 42%;
        animation-delay: .5s;
    }

    .flor3 {
        left: 69%;
        animation-delay: 1s;
    }

    .petalos {
        position: absolute;
        top: 0;
        left: 25px;
        width: 70px;
        height: 70px;
    }

    .petalo {
        position: absolute;
        width: 35px;
        height: 55px;
        background: #ffd21f;
        border-radius: 50%;
        left: 18px;
        top: 8px;
        transform-origin: 50% 100%;
    }

    .p1 { transform: rotate(0deg); }
    .p2 { transform: rotate(60deg); }
    .p3 { transform: rotate(120deg); }
    .p4 { transform: rotate(180deg); }
    .p5 { transform: rotate(240deg); }
    .p6 { transform: rotate(300deg); }

    .centro {
        position: absolute;
        width: 35px;
        height: 35px;
        background: #8b5a00;
        border-radius: 50%;
        top: 26px;
        left: 43px;
        z-index: 2;
    }

    .tallo {
        position: absolute;
        width: 8px;
        height: 130px;
        background: #3b8c32;
        left: 56px;
        top: 65px;
        border-radius: 10px;
    }

    .hoja {
        position: absolute;
        width: 45px;
        height: 20px;
        background: #3b8c32;
        border-radius: 100% 0;
        top: 120px;
        left: 15px;
        transform: rotate(-25deg);
    }

    .suelo {
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 22%;
        background: #5da344;
        border-radius: 50% 50% 0 0;
    }

    @keyframes mover {
        0%, 100% {
            transform: rotate(-2deg);
        }

        50% {
            transform: rotate(2deg);
        }
    }

    @media (max-width: 500px) {
        .mensaje {
            font-size: 23px;
        }

        .flor {
            transform: scale(.8);
        }
    }
</style>
</head>

<body>

<div class="jardin">

    <div class="mensaje">
        🌻 Flores amarillas para ti 🌻
    </div>

    <div class="flor flor1">
        <div class="petalos">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

    <div class="flor flor2">
        <div class="petalos">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

    <div class="flor flor3">
        <div class="petalos">
            <div class="petalo p1"></div>
            <div class="petalo p2"></div>
            <div class="petalo p3"></div>
            <div class="petalo p4"></div>
            <div class="petalo p5"></div>
            <div class="petalo p6"></div>
            <div class="centro"></div>
        </div>
        <div class="tallo"></div>
        <div class="hoja"></div>
    </div>

    <div class="suelo"></div>

</div>

</body>
</html>
