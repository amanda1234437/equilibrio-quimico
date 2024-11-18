/seu_projeto
├── index.html
├── style.css
├── script.js
└── imagens
    ├── equilibrio-agua.png
    ├── sintese-amonia.png
    └── acido-base.png
    <body>
    <!-- Banner da página -->
    <div class="banner">
        <img src="imagens/banner.png" alt="Banner sobre Equilíbrio Químico">
        <div class="titulo-banner">
        /* Estilos para o banner */
.banner {
    position: relative;
    width: 100%;
    height: 300px;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
}

.banner img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.titulo-banner {
    position: absolute;
    text-align: center;
    color: #fff;
    background-color: rgba(0, 0, 0, 0.5);
    padding: 20px;
    border-radius: 10px;
}

.titulo-banner h1 {
    font-size: 2.5em;
    margin: 0;
}

.titulo-banner p {
    font-size: 1.2em;
    margin-top: 10px;
}
            <h1>Equilíbrio Químico</h1>
            <p>Explorando os conceitos de equilíbrio nas reações químicas</p>
        </div>
    </div>
    <!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Equilíbrio Químico</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Equilíbrio Químico</h1>
        <nav>
            <ul>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#exemplos">Exemplos</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <section id="sobre">
        <h2>O que é Equilíbrio Químico?</h2>
        <p>O equilíbrio químico é o estado onde as concentrações dos reagentes e produtos permanecem constantes em um sistema fechado, porque as velocidades das reações direta e reversa são iguais.</p>
        <img src="imagens/equilibrio-agua.png" alt="Equilíbrio da água" class="imagem">
    </section>

    <section id="exemplos">
        <h2>Exemplos de Reações em Equilíbrio</h2>
        <div class="exemplo">
            <h3>Equilíbrio da água (H<sub>2</sub>O ⇌ H<sup>+</sup> + OH<sup>-</sup>)</h3>
            <img src="imagens/equilibrio-agua.png" alt="Equilíbrio da água" class="imagem">
        </div>
        <div class="exemplo">
            <h3>Processo de Haber (N<sub>2</sub> + 3H<sub>2</sub> ⇌ 2NH<sub>3</sub>)</h3>
            <img src="imagens/sintese-amonia.png" alt="Síntese da amônia" class="imagem">
        </div>
        <div class="exemplo">
            <h3>Equilíbrio ácido-base (CH<sub>3</sub>COOH ⇌ CH<sub>3</sub>COO<sup>-</sup> + H<sup>+</sup>)</h3>
            <img src="imagens/acido-base.png" alt="Equilíbrio ácido-base" class="imagem">
        </div>
        <button id="ver-exemplo">Mostrar Reação Interativa</button>
        <div id="resultado"></div>
    </section>

    <section id="contato">
        <h2>Entre em Contato</h2>
        <form id="form-contato">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" required>
            <label for="email">Email:</label>
            <input type="email" id="email" required>
            <button type="submit">Enviar</button>
        </form>
    </section>

    <footer>
        <p>© 2024 Equilíbrio Químico. Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    color: #333;
    margin: 0;
    padding: 0;
}

header {
    background-color: #0077b6;
    color: #fff;
    text-align: center;
    padding: 1em;
}

nav ul {
    list-style: none;
    padding: 0;
    text-align: center;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
}

section {
    padding: 2em;
    margin: 1em auto;
    max-width: 800px;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.imagem {
    width: 100%;
    max-width: 400px;
    display: block;
    margin: 20px auto;
    border-radius: 8px;
}

button {
    background-color: #0077b6;
    color: #fff;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    border-radius: 5px;
    display: block;
    margin: 20px auto;
}

button:hover {
    background-color: #005f7f;
}

footer {
    background-color: #0077b6;
    color: #fff;
    text-align: center;
    padding: 1em;
}
document.getElementById('ver-exemplo').addEventListener('click', function() {
    const resultado = document.getElementById('resultado');
    resultado.innerHTML = `
        <p><strong>Equilíbrio dinâmico:</strong> Ao adicionar mais reagente ou produto, o sistema se ajusta para restabelecer o equilíbrio, seguindo o princípio de Le Chatelier.</p>
        <img src="imagens/equilibrio-agua.png" alt="Exemplo de Equilíbrio" class="imagem">
    `;
});

document.getElementById('form-contato').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Formulário enviado com sucesso! Obrigado pelo contato.');
});
