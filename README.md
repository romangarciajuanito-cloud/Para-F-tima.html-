# Para-F-tima.html-
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Para Fátima ❤️</title>

<style>
body {
    margin: 0;
    padding: 0;
    background: linear-gradient(to bottom, #ff9a9e, #fecfef);
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
    color: white;
    overflow: hidden;
}

/* Carta */
.carta {
    max-width: 90%;
    background: rgba(255,255,255,0.15);
    padding: 25px;
    border-radius: 20px;
    backdrop-filter: blur(10px);
    z-index: 1;
}

h1 {
    font-size: 42px;
    margin-bottom: 15px;
    animation: latido 1.2s infinite;
}

p {
    font-size: 20px;
    line-height: 1.6;
}

/* Latido */
@keyframes latido {
    0% { transform: scale(1); }
    50% { transform: scale(1.08); }
    100% { transform: scale(1); }
}

/* Flores */
.flor {
    position: absolute;
    font-size: 25px;
    animation: subir 3s linear forwards;
}

@keyframes subir {
    0% {
        transform: translateY(0);
        opacity: 1;
    }
    100% {
        transform: translateY(-100px);
        opacity: 0;
    }
}
</style>
</head>

<body onclick="crearFlor(event)">

<div class="carta">
    <h1>❤️ Fátima ❤️</h1>

    <p>
        Tal vez no siempre podamos vernos tanto como quisiéramos,
        pero eso no cambia lo que siento por ti ni un poquito.
    </p>

    <p>
        Porque aunque no estés cerca, siempre estás en mi mente
        y en mi corazón en cada momento 💕
    </p>

    <p>
        Quiero que sepas que pase lo que pase,
        estés donde estés, yo siempre voy a estar para ti.
    </p>

    <p>
        Porque lo que siento por ti es real,
        es bonito… y es algo que no va a cambiar ❤️
    </p>

    <p>
        Te amo hoy, mañana y todos los días,
        sin importar la distancia ni el tiempo 💖✨
    </p>

    <p style="margin-top:15px; font-size:16px;">
        (Toca la pantalla )
    </p>
</div>

<script>
function crearFlor(e) {
    const flor = document.createElement("div");
    flor.classList.add("flor");
    flor.innerHTML = "🌸";

    flor.style.left = e.clientX + "px";
    flor.style.top = e.clientY + "px";

    document.body.appendChild(flor);

    setTimeout(() => {
        flor.remove();
    }, 3000);
}
</script>

</body>
</html>
