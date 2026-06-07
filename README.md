<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>English & Digital Culture</title>

<style>
body{
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #1e3c72, #2a5298);
    color: white;
    margin: 0;
}

header{
    background: #0f172a;
    text-align: center;
    padding: 20px;
}

section{
    background: rgba(255,255,255,0.1);
    margin: 20px;
    padding: 20px;
    border-radius: 15px;
}

input{
    padding: 10px;
    border-radius: 8px;
    border: none;
}

button{
    padding: 10px 15px;
    border: none;
    border-radius: 8px;
    background: #38bdf8;
    cursor: pointer;
    margin-top: 10px;
}

button:hover{
    background: #0ea5e9;
}

footer{
    background: #0f172a;
    text-align: center;
    padding: 15px;
}

ul{
    line-height: 1.8;
}
</style>
</head>
<body>

<header>
    <h1>🌎 English & Digital Culture</h1>
    <p>Learning English and Technology</p>
</header>

<section>
    <h2>📖 English Vocabulary</h2>
    <ul>
        <li>Computer = Computadora</li>
        <li>Keyboard = Teclado</li>
        <li>Mouse = Ratón</li>
        <li>Internet = Internet</li>
        <li>Screen = Pantalla</li>
    </ul>
</section>

<section>
    <h2>💻 Digital Culture</h2>
    <p>
        Digital culture includes the technologies and tools that people use
        to communicate, learn and work in everyday life.
    </p>
</section>

<section>
    <h2>🔎 Translator</h2>
    <input type="text" id="word" placeholder="Write a word">
    <button onclick="translateWord()">Translate</button>
    <p id="result"></p>
</section>

<section>
    <h2>📝 Quiz</h2>
    <p>What is the translation of "Keyboard"?</p>

    <button onclick="checkAnswer('Teclado')">Teclado</button>
    <button onclick="checkAnswer('Pantalla')">Pantalla</button>

    <p id="answer"></p>
</section>

<footer>
    Created by Student ✨
</footer>

<script>
function translateWord() {
    let word = document.getElementById("word").value.toLowerCase();
    let translation = "";

    if (word === "computer") {
        translation = "Computadora";
    } else if (word === "keyboard") {
        translation = "Teclado";
    } else if (word === "mouse") {
        translation = "Ratón";
    } else if (word === "screen") {
        translation = "Pantalla";
    } else if (word === "internet") {
        translation = "Internet";
    } else {
        translation = "Word not found";
    }

    document.getElementById("result").textContent = translation;
}

function checkAnswer(option) {
    if (option === "Teclado") {
        document.getElementById("answer").textContent = "✅ Correct!";
    } else {
        document.getElementById("answer").textContent = "❌ Incorrect!";
    }
}
</script>

</body>
</html>
