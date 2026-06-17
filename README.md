# Site-do-bts
Criação para falar sobre os meninos do BTS.
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo BTS - Curiosidades e Linha do Tempo</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Mundo BTS 💜</h1>
        <p>Tudo sobre o dia a dia e curiosidades dos sete membros</p>
    </header>

    <main>
        <section class="membros">
            <h2>Os Sete Membros</h2>
            <div class="grid-membros">
                <div class="card"><strong>RM</strong> (Líder)</div>
                <div class="card"><strong>Jin</strong></div>
                <div class="card"><strong>Suga</strong></div>
                <div class="card"><strong>J-Hope</strong></div>
                <div class="card"><strong>Jimin</strong></div>
                <div class="card"><strong>V</strong></div>
                <div class="card"><strong>Jungkook</strong></div>
            </div>
        </section>

        <section class="curiosidades">
            <h2>Curiosidades Rápidas</h2>
            <ul>
                <li>O grupo debutou oficialmente em 13 de junho de 2013.</li>
                <li>O nome do fandom, ARMY, significa "Adorable Representative M.C. for Youth".</li>
                <li>Eles são conhecidos por produzirem e escreverem a grande maioria de suas próprias músicas.</li>
            </ul>
            <button id="botao-diario">Ver atualização do dia</button>
        </section>
    </main>

    <footer>
        <p>Feito por um ARMY para ARMYs | 2026</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f3f0f7;
    color: #333;
    margin: 0;
    padding: 0;
}

header {
    background-color: #512da8; /* Roxo BTS */
    color: white;
    text-align: center;
    padding: 40px 20px;
}

main {
    max-width: 900px;
    margin: 30px auto;
    padding: 0 20px;
}

h2 {
    color: #512da8;
    border-bottom: 2px solid #d1c4e9;
    padding-bottom: 10px;
}

/* Organização dos cards dos membros */
.grid-membros {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
    gap: 15px;
    margin-bottom: 40px;
}

.card {
    background-color: white;
    padding: 20px;
    text-align: center;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    border-top: 4px solid #7e57c2;
}

ul {
    padding-left: 20px;
    line-height: 1.8;
}

button {
    background-color: #7e57c2;
    color: white;
    border: none;
    padding: 12px 24px;
    font-size: 16px;
    border-radius: 25px;
    cursor: pointer;
    display: block;
    margin: 20px auto 0;
    transition: 0.3s;
}

button:hover {
    background-color: #512da8;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #212121;
    color: #b0bec5;
    margin-top: 50px;
}const botao = document.getElementById('botao-diario');

const atualizacoes = [
    "Hoje os meninos estão focados em projetos de estúdio!",
    "Lembrança do dia: O discurso emocionante do BTS na ONU.",
    "Dica de hoje: Que tal rever o último episódio de Run BTS?",
    "Fato do dia: O roxo se tornou o símbolo do grupo graças ao termo 'I Purple You' criado pelo V."
];

botao.addEventListener('click', () => {
    // Escolhe uma frase aleatória da lista acima
    const fraseAleatoria = atualizacoes[Math.floor(Math.random() * atualizacoes.length)];
    alert(fraseAleatoria);
});

