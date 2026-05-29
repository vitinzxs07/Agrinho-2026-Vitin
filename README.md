# Agrinho-2026-Vitin
Projeto Agrinho 1° Ano 2026 Ita.
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>agrinho2026</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="main-header">
        <div class="logo">agrinho<span>2026</span></div>
        <nav class="nav-links">
            <a href="#sobre">Sobre</a>
            <a href="#agroforte">Agroforte</a>
            <a href="#tecnologias">Tecnologias</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Inovação que Transforma o Campo</h1>
            <p>Desenvolvendo soluções digitais para o agronegócio de amanhã.</p>
            <a href="#agroforte" class="btn-primary">Conhecer Visão</a>
        </div>
    </section>

    <section id="agroforte" class="manifesto-section">
        <div class="container">
            <h2>Agroforte & Futuro Sustentável</h2>
            <div class="divider"></div>
            <blockquote>
                "O conceito de um <strong>Agroforte</strong> só se consolida quando caminha lado a lado com um <strong>futuro sustentável</strong>. A verdadeira potência do campo em 2026 não é medida apenas pela quantidade da colheita, mas pela inteligência aplicada em sua preservação. Através da tecnologia no Front-End, criamos interfaces capazes de monitorar recursos, otimizar dados agrícolas e aproximar a nova geração de produtores de práticas ecologicamente viáveis. Unir a força da terra à precisão do código é o que garante a segurança alimentar do planeta com respeito à biodiversidade."
            </blockquote>
        </div>
    </section>

    <footer class="main-footer">
        <p>&copy; 2026 Repositório agrinho2026 - Código aberto para um futuro sustentável.</p>
    </footer>

</body>
</html>
/* Reset e Configurações Globais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', system-ui, sans-serif;
}

:root {
    /* Paleta selecionada: Tons de Azul Escuro e Amarelo Pontual */
    .bg-dark-blue { color: #0a192f; } /* Referência visual */
    --navy-dark: #0a192f;      /* Azul escuro profundo (predominante) */
    --navy-medium: #112240;    /* Azul escuro para blocos/cards */
    --accent-yellow: #ffcb05;  /* Amarelo vivo (contraste e destaques) */
    --text-light: #e6f1ff;     /* Texto claro para contraste */
    --text-gray: #8892b0;      /* Texto secundário */
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: var(--navy-dark);
    color: var(--text-light);
    line-height: 1.6;
}

/* Cabeçalho */
.main-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 8%;
    background-color: rgba(10, 25, 47, 0.85);
    backdrop-filter: blur(10px);
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 1px solid rgba(255, 203, 5, 0.1);
}

.logo {
    font-size: 24px;
    font-weight: 700;
    letter-spacing: 1px;
}

.logo span {
    color: var(--accent-yellow);
}

.nav-links a {
    text-decoration: none;
    color: var(--text-light);
    margin-left: 25px;
    font-size: 15px;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: var(--accent-yellow);
}

/* Banner Principal (Hero) */
.hero {
    height: 65vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
    background: radial-gradient(circle at center, #112240 0%, #0a192f 100%);
}

.hero-content h1 {
    font-size: 42px;
    color: #ffffff;
    margin-bottom: 15px;
}

.hero-content p {
    color: var(--text-gray);
    font-size: 18px;
    max-width: 600px;
    margin: 0 auto 30px auto;
}

/* Botão */
.btn-primary {
    display: inline-block;
    padding: 12px 28px;
    border: 2px solid var(--accent-yellow);
    color: var(--accent-yellow);
    text-decoration: none;
    font-weight: 600;
    border-radius: 4px;
    transition: all 0.3s ease;
}

.btn-primary:hover {
    background-color: var(--accent-yellow);
    color: var(--navy-dark);
    box-shadow: 0 4px 20px rgba(255, 203, 5, 0.3);
}

/* Seção Manifesto (Agroforte) */
.manifesto-section {
    padding: 80px 10%;
    background-color: var(--navy-medium);
}

.container {
    max-width: 900px;
    margin: 0 auto;
    text-align: center;
}

.manifesto-section h2 {
    font-size: 32px;
    color: var(--accent-yellow);
    margin-bottom: 10px;
}

.divider {
    height: 3px;
    width: 60px;
    background-color: var(--accent-yellow);
    margin: 0 auto 30px auto;
    border-radius: 2px;
}

blockquote {
    font-size: 19px;
    color: var(--text-light);
    font-style: italic;
