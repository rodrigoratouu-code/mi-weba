<!DOCTYPE html>
<html lang="es">
<head>
  <!-- Open Graph -->
<meta property="og:title" content="Mi Web Dans" />
<meta property="og:description" content="Bienvenidos a mi sitio web" />
<meta property="og:image" content="https://rodrigoratouu-code.github.io/mi-weba/radioRD.webp" />
<meta property="og:url" content="https://rodrigoratouu-code.github.io/mi-weba" />
<meta property="og:type" content="website" />

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:title" content="Mi Web Dans" />
<meta name="twitter:description" content="Bienvenido a mi sitio web" />
<meta name="twitter:image" content="https://rodrigoratouu-code.github.io/mi-weba/imagen.jpg" />

      <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emisoras de Radio Latinas</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            width: 100%;
        }

        h1 {
            text-align: center;
            color: #fff;
            font-size: 2.5rem;
            margin-bottom: 50px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            letter-spacing: 1px;
        }

        .radio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 20px;
        }

        .radio-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
        }

        .radio-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 40px rgba(233, 69, 96, 0.3);
            border-color: rgba(233, 69, 96, 0.5);
        }

        .radio-image {
            width: 250px;
            height: 150px;
            border-radius: 10%;
            margin: 0 auto 25px;
            object-fit: cover;
            border: 4px solid rgba(233, 69, 96, 0.6);
            box-shadow: 0 4px 15px rgba(233, 69, 96, 0.4);
        }

        .radio-button {
            display: inline-block;
            padding: 15px 40px;
            background: linear-gradient(135deg, #45e989 0%, #f11c5c 100%);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(233, 69, 96, 0.4);
            border: 2px solid transparent;
        }

        .radio-button:hover {
            background: linear-gradient(135deg, #0bffae 0%, #ffffff 100%);
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(255, 253, 254, 0.6);
            border-color: rgba(255, 255, 255, 0.89);
        }

        .radio-button:active {
            transform: scale(0.98);
        }

        .radio-name {
            color: #fff;
            font-size: 1.3rem;
            margin-bottom: 20px;
            font-weight: 600;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
                margin-bottom: 30px;
            }

            .radio-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }

            .radio-card {
                padding: 25px;
            }
        }

        /* Efecto de onda al hacer clic */
        @keyframes ripple {
            0% {
                transform: scale(0);
                opacity: 1;
            }
            100% {
                transform: scale(4);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🎵Radio Latinas iBE </h1>
        
        <div class="radio-grid">
            <!-- Radio 1: Olímpica Stereo -->
            <div class="radio-card">
                <img src="radiocol.webp" alt="Olímpica Stereo Medellín" class="radio-image">
                <div class="radio-name">Olímpica Stereo Medellín</div>
                <a href="https://www.emisorascolombianas.co/olimpica-stereo-medellin"  
                class="radio-button">
                    ▶ Escuchar Ahora
                </a>
            </div>

            <!-- Radio 2: Alofoke -->
            <div class="radio-card">
                <img src="alofoke.webp" alt="Alofoke Radio" class="radio-image">
                <div class="radio-name">Alofoke Radio</div>
                <a href="https://rdomiplayer.com/landing/radio/1596/1" 
                class="radio-button">
                    ▶ Escuchar Ahora
                </a>
            </div>
        </div>
    </div>
</body>
</html>
