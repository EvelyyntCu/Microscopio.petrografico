# Microscopio.petrografico
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Microscopio Petrográfico MEIJI</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .container {
            position: relative;
            display: inline-block;
        }
        .part {
            position: absolute;
            background: rgba(255, 255, 255, 0.8);
            padding: 5px;
            border-radius: 5px;
            cursor: pointer;
        }
        .tooltip {
            display: none;
            position: absolute;
            background: black;
            color: white;
            padding: 5px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <h1>Microscopio Petrográfico MEIJI</h1>
    <div class="container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/5/50/Petrographic_Microscope.jpg" alt="Microscopio MEIJI" width="500">
        
        <div class="part" style="top: 10px; left: 200px;" onclick="showInfo('Ocular: Permite observar la imagen ampliada.')">🔍</div>
        <div class="part" style="top: 100px; left: 150px;" onclick="showInfo('Objetivos: Lentes que amplían la imagen de la muestra.')">🔍</div>
        <div class="part" style="top: 200px; left: 180px;" onclick="showInfo('Platina: Plataforma donde se coloca la muestra.')">🔍</div>
        <div class="part" style="top: 300px; left: 220px;" onclick="showInfo('Fuente de luz: Ilumina la muestra para su observación.')">🔍</div>
    </div>
    
    <div id="info" class="tooltip"></div>
    
    <script>
        function showInfo(text) {
            let infoBox = document.getElementById("info");
            infoBox.textContent = text;
            infoBox.style.display = "block";
            setTimeout(() => infoBox.style.display = "none", 3000);
        }
    </script>
</body>
</html>"}
