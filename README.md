<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agrinho 2026</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="main-header">
        <div class="logo">Agrinho <span>2026</span></div>
        <nav class="nav-links">
            <a href="#sobre">Sobre</a>
            <a href="#projetos">Projetos</a>
            <a href="#contato" class="btn-primary">Participar</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Inovação e Sustentabilidade no Campo</h1>
            <p>Conectando a educação, a tecnologia e o futuro da agricultura sustentável.</p>
            <a href="#sobre" class="btn-secondary">Saiba Mais</a>
        </div>
    </section>

    <section id="sobre" class="content-section">
        <h2>Sobre o Agrinho 2026</h2>
        <p>O Agrinho 2026 traz como foco a transformação digital no campo aliada à preservação ambiental. Nosso objetivo é incentivar soluções inovadoras que tornem a agricultura mais inteligente, eficiente e acessível para as próximas gerações.</p>
    </section>

    <footer class="main-footer">
        <p>&copy; 2026 Agrinho - Desenvolvido com foco no futuro do Agro.</p>
    </footer>

</body>
</html>/* Reset básico e variáveis de cor */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

:root {
    --primary-color: #2e7d32; /* Verde Agro */
    --secondary-color: #f9a825; /* Amarelo Sol/Colheita */
    --dark-color: #1b5e20;
    --light-color: #f1f8e9;
    --text-color: #333;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: #ffffff;
    color: var(--text-color);
    line-height: 1.6;
}

/* Cabeçalho */
.main-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 10%;
    background-color: #ffffff;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: var(--primary-color);
}

.logo span {
    color: var(--secondary-color);
}

.nav-links a {
    text-decoration: none;
    color: var(--text-color);
    margin-left: 20px;
    font-weight: 500;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: var(--primary-color);
}

/* Botões */
.btn-primary {
    background-color: var(--primary-color);
    color: white !important;
    padding: 8px 20px;
    border-radius: 5px;
    transition: background 0.3s !important;
}

.btn-primary:hover {
    background-color: var(--dark-color);
}

.btn-secondary {
    display: inline-block;
    background-color: var(--secondary-color);
    color: white;
    text-decoration: none;
    padding: 12px 30px;
    border-radius: 5px;
    font-weight: bold;
    margin-top: 20px;
    transition: transform 0.2s;
}

.btn-secondary:hover {
    transform: scale(1.05);
}

/* Seção Hero */
.hero {
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.3)), 
                url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1470') no-repeat center center/cover;
    height: 70vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    padding: 0 20px;
}

.hero-content h1 {
    font-size: 48px;
    margin-bottom: 15px;
}

.hero-content p {
    font-size: 20px;
    max-width: 600px;
    margin: 0 auto;
}

/* Seção de Conteúdo Geral */
.content-section {
    padding: 80px 10%;
    text-align: center;
    background-color: var(--light-color);
}

.content-section h2 {
    color: var(--dark-color);
    font-size: 32px;
    margin-bottom: 20px;
}

.content-section p {
    max-width: 800px;
    margin: 0 auto;
    font-size: 18px;
}

/* Rodapé */
.main-footer {
    background-color: var(--dark-color);
    color: white;
    text-align: center;
    padding: 20px;
    font-size: 14px;
}

/* Responsividade Básica */
@media (max-width: 768px) {
    .main-header {
        flex-direction: column;
        gap: 15px;
    }
    .hero-content h1 {
        font-size: 32px;
    }
    .hero-content p {
        font-size: 16px;
    }
}
