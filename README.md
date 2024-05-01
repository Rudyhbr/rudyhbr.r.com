#<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aritmética Elemental - Quiz</title>
</head>
<body>
    <h1>Aritmética Elemental - Quiz</h1>

    <p>Probar tus conocimientos en aritmética respondiendo las siguientes preguntas:</p>

    <form id="quizForm">
        <h3>Pregunta 1: ¿Cuánto es 5 + 3?</h3>
        <input type="radio" name="pregunta1" value="8"> 8<br>
        <input type="radio" name="pregunta1" value="7"> 7<br>
        <input type="radio" name="pregunta1" value="6"> 6<br><br>

        <h3>Pregunta 2: ¿Cuánto es 12 - 4?</h3>
        <input type="radio" name="pregunta2" value="8"> 8<br>
        <input type="radio" name="pregunta2" value="6"> 6<br>
        <input type="radio" name="pregunta2" value="5"> 5<br><br>

        <h3>Pregunta 3: ¿Cuánto es 3 * 4?</h3>
        <input type="radio" name="pregunta3" value="10"> 10<br>
        <input type="radio" name="pregunta3" value="12"> 12<br>
        <input type="radio" name="pregunta3" value="9"> 9<br><br>

        <button type="button" onclick="calificar()">Calificar</button>
    </form>

    <div id="resultado"></div>

    <script>
        function calificar() {
            var respuestas = document.getElementById("quizForm").elements;
            var correctas = 0;

            for (var i = 0; i < respuestas.length; i++) {
                if (respuestas[i].checked && respuestas[i].value === "8") {
                    correctas++;
                }
            }

            document.getElementById("resultado").innerHTML = "Has acertado " + correctas + " de 3 preguntas.";
        }
    </script>
</body>
</html> rudyhbr.r.com
Matemáticas e Informática 
