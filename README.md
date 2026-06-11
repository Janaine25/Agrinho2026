# Agrinho2026
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agrinho 2026 - Conectando Campo e Cidade</title>
    <style>
        /* Cores e Reset Global */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --verde-escuro: #1b4d3e;
            --verde-claro: #2e7d32;
            --amarelo-sol: #fbc02d;
            --bege-fundo: #f4f6f0;
            --texto-escuro: #333;
        }

        body {
            background-color: var(--bege-fundo);
            color: var(--texto-escuro);
            line-height: 1.6;
        }

        /* Cabeçalho */
        header {
            background-color: var(--verde-escuro);
            color: white;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header h1 {
            font-size: 1.8rem;
            font-weight: bold;
        }

        header h1 span {
            color: var(--amarelo-sol);
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 1.5rem;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--amarelo-sol);
        }

        /* Banner Principal */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
            height: 60vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 0 1rem;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin-bottom: 2rem;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.7);
        }

        .btn {
            background-color: var(--amarelo-sol);
            color: var(--verde-escuro);
            padding: 0.8rem 2rem;
            text-decoration: none;
            font-weight: bold;
            border-radius: 25px;
            transition: transform 0.2s, background-color 0.3s;
        }

        .btn:hover {
            transform: scale(1.05);
            background-color: #fdd835;
        }

        /* Seções de Conteúdo */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 4rem 1rem;
        }

        .section-title {
            text-align: center;
            color: var(--verde-escuro);
            margin-bottom: 3rem;
            font-size: 2.2rem;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--amarelo-sol);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }

        /* Grid de Pilares/Temas */
        .grid-temas {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .card {
            background: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            border-top: 5px solid var(--verde-claro);
            transition: translateY 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            color: var(--verde-escuro);
            margin-bottom: 1rem;
        }

        /* Sobre / Cronograma */
        .sobre-content {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            align-items: center;
        }

        .sobre-text {
            flex: 1;
            min-width: 300px;
        }

        .sobre-text p {
            margin-bottom: 1rem;
        }

        /* Rodapé */
        footer {
            background-color: var(--verde-escuro);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        footer p {
            font-size: 0.9rem;
            opacity: 0.8;
        }

        /* Responsividade Básica */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 1rem;
            }
            nav a {
                margin: 0 0.7rem;
            }
            .hero h2 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Cabeçalho -->
    <header id="inicio">
        <h1><span>Agrinho</span> 2026</h1>
        <nav>
            <a href="#inicio">Início</a>
            <a href="#sobre">O Projeto</a>
            <a href="#temas">Eixos Temáticos</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <!-- Banner Principal -->
    <section class="hero">
        <h2>Inovação e Sustentabilidade no Campo</h2>
        <p>Cultivando o conhecimento e colhendo um futuro melhor através da educação e da tecnologia no agronegócio.</p>
        <a href="#sobre" class="btn">Saiba Mais</a>
    </section>

    <!-- Seção Sobre -->
    <section class="container" id="sobre">
        <h2 class="section-title">Sobre o Agrinho 2026</h2>
        <div class="sobre-content">
            <div class="sobre-text">
                <p>O <strong>Programa Agrinho</strong> é a maior iniciativa de responsabilidade social do Sistema FAEP/SENAR-PR. Em 2026, nosso foco está em conectar as novas tecnologias digitais à preservação ambiental e ao protagonismo jovem.</p>
                <p>Há décadas, o programa leva para as escolas públicas e particulares uma proposta pedagógica focada na pesquisa, na ética e no desenvolvimento sustentável, premiando as melhores práticas de alunos e professores.</p>
            </div>
        </div>
    </section>

    <!-- Seção Temas (Grid) -->
    <section class="container" style="background-color: #fff; max-width: 100%;" id="temas">
        <div style="max-width: 1100px; margin: 0 auto; padding: 1rem;">
            <h2 class="section-title">Eixos Temáticos deste Ano</h2>
            <div class="grid-temas">
                <div class="card">
                    <h3>🌱 Sustentabilidade</h3>
                    <p>Práticas agrícolas que protegem o solo, a água e a biodiversidade, garantindo o futuro das próximas gerações.</p>
                </div>
                <div class="card">
                    <h3>🚀 Tecnologia e IA</h3>
                    <p>Como a Inteligência Artificial, drones e a tecnologia no campo ajudam a produzir mais com menos recursos.</p>
                </div>
                <div class="card">
                    <h3>🏡 Cidadania</h3>
                    <p>A integração entre o campo e a cidade, valorizando o trabalhador rural e a segurança alimentar de todos.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Rodapé / Contato -->
    <footer id="contato">
        <p style="margin-bottom: 1rem; font-weight: bold; color: var(--amarelo-sol);">Projeto Agrinho 2026</p>
        <p>Desenvolvido para fins educativos e de engajamento escolar.</p>
        <p style="margin-top: 1.5rem; font-size: 0.8rem;">&copy; 2026 Sistema FAEP/SENAR. Imagens ilustrativas via Unsplash.</p>
    </footer>

</body>
</html>
