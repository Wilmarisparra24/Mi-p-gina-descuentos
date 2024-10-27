# Mi-p-gina-descuentos
<!DOCTYPE html >
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Generador de Descuentos</title>
</head>
<body>
    <h1>Sube tu imagen para obtener un descuento</h1>
    <input type="file" id="fileInput" accept="image/*">
    <button onclick="generarDescuento()">Generar Descuento</button>
    <p id="descuento"></p>

    <script>
        function generarDescuento() {
    const fileInput = document.getElementById('fileInput');
    if (fileInput.files.length === 0) {
        alert('Por favor, sube una imagen primero.');
        return;
    }

    const descuento = Math.floor(Math.random() * 10) + 1; // Genera un número aleatorio entre 1 y 10
    document.getElementById('descuento').innerText = `¡Has obtenido un ${descuento}% de descuento!`;
    }
</script>
</body>
</html>
