<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diccionario de Imágenes en Carrusel</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            margin: 0;
            padding: 20px;
            background-color: #f3f3f3;
        }

        h1 {
            margin-bottom: 20px;
            color: #333;
        }

        .slider-container {
            position: relative;
            width: 80%;
            overflow: hidden;
            max-width: 1000px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .slider {
            display: flex;
            transition: transform 0.5s ease;
            width: calc(100% * 5); /* Ajusta el valor según la cantidad de imágenes */
        }

        .slider-item {
            min-width: 100%;
            box-sizing: border-box;
            text-align: center;
            background-color: #fff;
            padding: 15px;
        }

        .slider-item img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }

        .slider-item h3 {
            font-size: 1.1em;
            margin: 10px 0 5px;
            color: #333;
        }

        .slider-item p {
            font-size: 0.9em;
            color: #777;
        }
    </style>
</head>
<body>

    <h1>Diccionario de Imágenes en Carrusel</h1>

    <div class="slider-container">
        <div class="slider" id="slider">
            <!-- Primera imagen -->
            <div class="slider-item">
                <img src="https://drive.google.com/file/d/1x5pQ3rQ263u0ocek_jKaak9pKlVPVI2s/view?usp=sharing">
                <h3>Nombre de la Imagen 1</h3>
                <p>Descripción breve de la imagen 1.</p>
            </div>

            <!-- Segunda imagen -->
            <div class="slider-item">
                <img src="https://drive.google.com/uc?export=view&id=ID_DE_LA_IMAGEN2" alt="Descripción de la Imagen 2">
                <h3>Nombre de la Imagen 2</h3>
                <p>Descripción breve de la imagen 2.</p>
            </div>

            <!-- Tercer imagen -->
            <div class="slider-item">
                <img src="https://drive.google.com/uc?export=view&id=ID_DE_LA_IMAGEN3" alt="Descripción de la Imagen 3">
                <h3>Nombre de la Imagen 3</h3>
                <p>Descripción breve de la imagen 3.</p>
            </div>

            <!-- Agrega más imágenes si es necesario -->
        </div>
    </div>

    <script>
        let slider = document.getElementById("slider");
        let slideIndex = 0;
        const slideWidth = slider.clientWidth;

        function autoSlide() {
            slideIndex++;
            if (slideIndex >= slider.children.length) {
                slideIndex = 0; // Reiniciar el carrusel al inicio
            }
            slider.style.transform = `translateX(-${slideIndex * slideWidth}px)`;
        }

        setInterval(autoSlide, 3000); // Cambia cada 3 segundos
    </script>
</body>
</html>
