<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Día del Padre</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f2f2f2;
            margin: 0;
            padding: 20px;
        }
        h1 {
            color: #333;
        }
        .option {
            display: inline-block;
            margin: 20px;
            cursor: pointer;
            border: 2px solid transparent;
            transition: border-color 0.3s;
        }
        .option img {
            width: 150px;
            height: 150px;
        }
        .option:hover {
            border-color: #333;
        }
        .message {
            display: none;
            margin-top: 20px;
            color: #333;
            font-size: 1.2em;
        }
    </style>
</head>
<body>
    <h1>Feliz Día del Padre</h1>
    <p>Esta página vale por:</p>
    <div class="option" onclick="showMessage('Baklava')">
        <img src="ruta-a-la-imagen-de-baklava.jpg" alt="Baklava">
        <p>Baklava</p>
    </div>
    <div class="option" onclick="showMessage('Guinness Stout')">
        <img src="ruta-a-la-imagen-de-guinness-stout.jpg" alt="Guinness Stout">
        <p>Guinness Stout</p>
    </div>
    <div class="option" onclick="showMessage('una Polo')">
        <img src="ruta-a-la-imagen-de-polo.jpg" alt="Polo">
        <p>Una Polo</p>
    </div>
    <div class="message" id="message"></div>

    <script>
        function showMessage(option) {
            const messageDiv = document.getElementById('message');
            messageDiv.innerHTML = `Has seleccionado ${option}. <br> Válido en Nogales.`;
            messageDiv.style.display = 'block';
        }
    </script>
</body>
</html>
