<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Нажимай клавиши</title>
</head>
<body>
    <h1>Нажимай клавиши R, G, B</h1>
    <p id="output">Нажмите клавишу для изменения цвета текста.</p>
    <script 
        src="script.js">
            document.addEventListener('keydown', function(event) {
    const output = document.getElementById('output');
    const key = event.key.toUpperCase();

    if (key === 'R') {
        output.style.color = 'red';
        output.textContent = 'Вы нажали клавишу R. Цвет текста изменился на красный.';
    } else if (key === 'G') {
        output.style.color = 'green';
        output.textContent = 'Вы нажали клавишу G. Цвет текста изменился на зелёный.';
    } else if (key === 'B') {
        output.style.color = 'blue';
        output.textContent = 'Вы нажали клавишу B. Цвет текста изменился на синий.';
    } else {
        output.style.color = 'black';
        output.textContent = 'Цвет не изменился. Нажмите \'R\', \'G\' или \'B\' для изменения цвета текста.';
    }
});
        </script>

</body>
</html>
