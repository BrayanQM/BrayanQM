<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animación ASCII Estilo Omarchy</title>
    <style>
        /* Fondo negro estilo hacker/terminal */
        body {
            background-color: #0a0a0a;
            color: #00ff00;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: monospace;
            overflow: hidden;
        }

        /* Contenedor del logo ASCII */
        .ascii-logo {
            font-family: monospace;
            white-space: pre; /* Mantiene los espacios y saltos de línea */
            font-size: 14px;
            font-weight: bold;
            line-height: 1.2;
            text-align: left;
            
            /* Aplicamos las animaciones: pulso de color y vibración */
            animation: cambiodecolor 4s infinite alternate, glitch 0.3s infinite;
            
            /* Sombra de neón */
            text-shadow: 0 0 8px rgba(0, 255, 0, 0.8);
        }

        /* Animación 1: Efecto de luces psicodélicas / cambio de color */
        @keyframes cambiodecolor {
            0% { color: #00ff00; text-shadow: 0 0 10px #00ff00; }
            33% { color: #00ffff; text-shadow: 0 0 10px #00ffff; }
            66% { color: #ff00ff; text-shadow: 0 0 10px #ff00ff; }
            100% { color: #ffff00; text-shadow: 0 0 10px #ffff00; }
        }

        /* Animación 2: Efecto Glitch / Pequeña vibración de distorsión */
        @keyframes glitch {
            0% { transform: translate(0); }
            20% { transform: translate(-1px, 1px); }
            40% { transform: translate(-1px, -1px); }
            60% { transform: translate(1px, 1px); }
            80% { transform: translate(1px, -1px); }
            100% { transform: translate(0); }
        }
    </style>
</head>
<body>

    <!-- Tu arte ASCII dentro de la etiqueta <pre> -->
    <pre class="ascii-logo">
██████╗ ██████╗  █████╗ ██╗   ██╗  █████╗     ███╗   ██╗     ██████╗ ███╗   ███╗
██╔══██╗██╔══██╗██╔══██╗╚██╗ ██╔╝██╔══██╗   ████╗  ██║    ██╔═══██╗████╗ ████║
██████╔╝██████╔╝███████║ ╚████╔╝ ███████║   ██╔██╗ ██║    ██║   ██║██╔████╔██║
██╔══██╗██╔══██╗██╔══██║  ╚██╔╝   ██╔══██║  ██║╚██╗██║    ██║▄▄ ██║██║╚██╔╝██║
██████╔╝██║  ██║██║  ██║    ██║    ██║   ██║ ██║ ╚████║    ╚██████╔╝██║ ╚═╝ ██║
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝    ╚═╝    ╚═╝   ╚═╝ ╚═╝  ╚═══╝     ╚══▀▀═╝ ╚═╝     ╚═╝
                                                                           
    </pre>

</body>
</html>
