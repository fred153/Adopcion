# Adopcion
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Diccionario de Imágenes</title>
    <style>
        /* Estilos básicos */
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

        .dictionary {
            display: flex;
            flex-wrap: wrap;
            max-width: 1000px;
            gap: 20px;
        }

        .dictionary-item {
            width: 200px;
            text-align: center;
            background-color: #fff;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .dictionary-item img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }

        .dictionary-item h3 {
            font-size: 1.1em;
            margin: 10px 0 5px;
            color: #333;
        }

        .dictionary-item p {
            font-size: 0.9em;
            color: #777;
        }
    </style>
</head>
<body>

    <h1>Diccionario de Imágenes</h1>

    <div class="dictionary">
        <!-- Primera imagen -->
        <div class="dictionary-item">
            <img src="ruta-a-tu-imagen1.jpg" alt="Descripción de la Imagen 1">
            <h3>Nombre de la Imagen 1</h3>
            <p>Descripción breve de la imagen 1.</p>
        </div>

        <!-- Segunda imagen -->
        <div class="dictionary-item">
            <img src="ruta-a-tu-imagen2.jpg" alt="Descripción de la Imagen 2">
            <h3>Nombre de la Imagen 2</h3>
            <p>Descripción breve de la imagen 2.</p>
        </div>

        <!-- Agrega más imágenes según sea necesario -->
        <!-- Tercer imagen -->
        <div class="dictionary-item">
            <img src="ruta-a-tu-imagen3.jpg" alt="Descripción de la Imagen 3">
            <h3>Nombre de la Imagen 3</h3>
            <p>Descripción breve de la imagen 3.</p>
        </div>
    </div>

</body>
</html>
