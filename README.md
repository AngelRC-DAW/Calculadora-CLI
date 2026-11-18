# Calculadora-CLI
Módulo y unidad: DWEC U02
Repositorio: https://github.com/AngelRC-DAW/Calculadora-CLI
Versión entregada: [enlace al commit]
Versión anterior: 
Requisitos trabajados: [qué has implementado o modificado en esta versión]
Pendiente o con errores: Completar css y js.

index.html:
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Proyecto 1 Calculadora</title>
    <link rel="stylesheet" href="estilos.css">
    <script src="app.js" defer></script>
</head>
<body>
        <h1>Calculadora</h1>

    <form id="calculadora" novalidate>
    <label for="numero1">Primer número:</label>
        <input type="number" id="numero1" step="any">

    <label for="operacion">Operación:</label>
        <select id="operacion">
            <option value="+">Sumar</option>
            <option value="-">Restar</option>
            <option value="*">Multiplicar</option>
            <option value="/">Dividir</option>
            <option value="**">Potencia</option>
            <option value="%">Resto</option>
        </select>

    <label for="numero2">Segundo número:</label>
        <input type="number" id="numero2" step="any">

        <button type="submit">Calcular</button>
        <button type="button" id="limpiar">Limpiar</button>
    </form>

    <p id="error"></p>
<p id="resultado"></p>
</body>
</html>

estilos.css:
body {
    font-family: Arial, sans-serif;
    background-color: #eeeeee;
    max-width: 350px;
    margin: 40px auto;
    padding: 15px;
}

form {
    background-color: white;
    padding: 20px;
    border: 1px solid gray;
}

app.js:
"use strict";

const formulario = document.getElementById("calculadora");
const campo1 = document.getElementById("numero1");
const campo2 = document.getElementById("numero2");
const operacion = document.getElementById("operacion");
const botonLimpiar = document.getElementById("limpiar");
const resultado = document.getElementById("resultado");
const error = document.getElementById("error");

pruebas.txt:
[Requisito | Datos o pasos | Resultado esperado | Resultado observado]