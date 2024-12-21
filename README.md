<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="calculadora">
        <input type="text" id="visor" disabled>
        <div class="botoes">
            <button onclick="adicionarNumero('7')">7</button>
            <button onclick="adicionarNumero('8')">8</button>
            <button onclick="adicionarNumero('9')">9</button>
            <button onclick="adicionarOperacao('/')">/</button>
            <button onclick="adicionarNumero('4')">4</button>
            <button onclick="adicionarNumero('5')">5</button>
            <button onclick="adicionarNumero('6')">6</button>
            <button onclick="adicionarOperacao('*')">*</button>
            <button onclick="adicionarNumero('1')">1</button>
            <button onclick="adicionarNumero('2')">2</button>
            <button onclick="adicionarNumero('3')">3</button>
            <button onclick="adicionarOperacao('-')">-</button>
            <button onclick="adicionarNumero('0')">0</button>
            <button onclick="calcular()">=</button>
            <button onclick="limpar()">C</button>
            <button onclick="adicionarOperacao('+')">+</button>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>


style.css

body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}

.calculadora {
    width: 300px;
    margin: 50px auto;
    padding: 20px;
    background-color: #fff;
    border: 1px solid #ddd;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.botoes {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

button {
    width: 100%;
    height: 50px;
    font-size: 24px;
    border: none;
    border-radius: 5px;
    background-color: #4CAF50;
    color: #fff;
    cursor: pointer;
}

button:hover {
    background-color: #3e8e41;
}

#visor {
    width: 100%;
    height: 50px;
    font-size: 24px;
    padding: 10px;
    border: none;
    border-radius: 5px;
    background-color: #f0f0f0;
}

