<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A.L Marketing - Landing Pages e Gestão de Tráfego</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Estilos gerais */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            color: #333;
        }

        /* Cabeçalho Fixo */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
            background-color: #fff;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            z-index: 1000;
        }
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #333;
        }
        .buttons a {
            text-decoration: none;
            color: white;
            background-color: #666;
            padding: 10px 15px;
            border-radius: 5px;
            margin: 0 5px;
            font-size: 14px;
            transition: background-color 0.3s ease;
        }
        .buttons a:hover {
            background-color: #444;
        }

        /* Seção Hero */
        .hero {
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 100px 20px;
            background-color: #e9e9e9;
            text-align: center;
            margin-top: 60px; /* Compensa o cabeçalho fixo */
        }
        .hero-content {
            max-width: 800px;
        }
        .hero h1 {
            font-size: 36px;
            font-weight: bold;
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
        }

        /* Benefícios */
        .benefits {
            padding: 40px 20px;
            background-color: #fff;
            text-align: center;
        }
        .benefits h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        .benefits ul {
            list-style: none;
            padding: 0;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .benefits li {
            background-color: #f8f8f8;
            padding: 20px;
            border-radius: 10px;
            width: 300px;
            text-align: left;
        }

        /* Prova Social */
        .testimonials {
            padding: 40px 20px;
            background-color: #e9e9e9;
            text-align: center;
        }
        .testimonials h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        .testimonial-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .testimonial {
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            width: 300px;
            text-align: left;
        }

        /* Ferramentas e Tecnologias */
        .tools {
            padding: 40px 20px;
            background-color: #fff;
            text-align: center;
        }
        .tools h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        .tools-logos {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        .tools-logos img {
            width: 100px;
            height: auto;
        }

        /* Carrossel de Portfólio */
        .portfolio {
            padding: 40px 20px;
            background-color: #e9e9e9;
            text-align: center;
        }
        .portfolio h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        .carousel {
            display: flex;
            overflow: hidden;
            width: 80%;
            margin: 0 auto;
            position: relative;
        }
        .carousel img {
            width: 33.33%;
            flex-shrink: 0;
            transition: transform 0.5s ease-in-out;
        }

        /* CTA Final */
        .cta-final {
            padding: 40px 20px;
            background-color: #fff;
            text-align: center;
        }
        .cta-final h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        .cta-final a {
            background-color: #666;
            color: white;
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-size: 18px;
            transition: background-color 0.3s ease;
        }
        .cta-final a:hover {
            background-color: #444;
        }

        /* Rodapé */
        footer {
            background-color: #e0e0e0;
            padding: 20px;
            text-align: left;
            font-size: 14px;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        .footer-logo {
            font-weight: bold;
            font-size: 24px;
        }
        .footer-columns {
            display: flex;
            gap: 50px;
            flex-wrap: wrap;
        }
        .footer-column {
            list-style: none;
            padding: 0;
        }
        .footer-column li {
            margin: 5px 0;
        }

        /* Botão de WhatsApp Fixo */
        .whatsapp-button {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #25d366;
            color: white;
            padding: 15px;
            border-radius: 50%;
            text-decoration: none;
            font-size: 24px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 28px;
            }
            .hero p {
                font-size: 16px;
            }
            .benefits li, .testimonial {
                width: 100%;
            }
            .carousel img {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <!-- Cabeçalho Fixo -->
    <header>
        <div class="logo">A.L Marketing</div>
        <nav class="buttons">
            <a href="https://www.linkedin.com/in/allefy-vidal-2125368b/">Portfólio</a>
            <a href="https://wa.me/5527996619274">Contato</a>
            <a href="https://wa.me/5527996619274" target="_blank" style="background-color: #25d366;">Solicitar Orçamento</a>
        </nav>
    </header>

    <!-- Seção Hero -->
    <section class="hero">
        <div class="hero-content">
            <h1>Landing Pages e Gestão de Tráfego Pago que Convertem!</h1>
            <p>Criamos sites e campanhas que transformam visitantes em clientes de verdade.</p>
            <a href="https://wa.me/5527996619274" target="_blank" class="cta-button">Solicite um Orçamento Agora</a>
        </div>
    </section>

    <!-- Benefícios -->
    <section class="benefits" id="benefits">
        <h2>Por que Escolher a A.L Marketing?</h2>
        <ul>
            <li>✅ Landing Pages Estratégicas: Feitas para aumentar conversões.</li>
            <li>✅ Gestão de Tráfego Pago: Atraímos o público certo no Meta Ads.</li>
            <li>✅ Sites Rápidos e Responsivos: Perfeitos para mobile e desktop.</li>
            <li>✅ Integrações Avançadas: Conectamos seu site ao WhatsApp, Email, etc.</li>
            
        </ul>
    </section>

        <!-- Ferramentas e Tecnologias -->
    <section class="tools">
        <h2>Diversas opções para seu negócio</h2>
        <div class="tools-logos">
            <img src="https://cdn.worldvectorlogo.com/logos/wordpress-icon.svg" alt="WordPress">
            <img src="https://cdn.worldvectorlogo.com/logos/meta-3.svg" alt="Elementor">
            <img src="https://cdn.worldvectorlogo.com/logos/mailchimp-freddie-icon-wink.svg" alt="Mailchimp">
            <img src="https://cdn.worldvectorlogo.com/logos/github-icon-1.svg" alt="GitHub">
            <img src="https://cdn.worldvectorlogo.com/logos/hostinger.svg" alt="Hostinger">
        </div>
    </section>

    <!-- Carrossel de Portfólio -->
    <section class="portfolio" id="portfolio">
        <h2>Alguns clientes:</h2>
        <div class="carousel">
            <img src="case1.jpg" alt="Projeto 1">
            <img src="case2.jpg" alt="Projeto 2">
            <img src="case3.jpg" alt="Projeto 3">
        </div>
    </section>

    <!-- CTA Final -->
    <section class="cta-final">
        <h2>Fale Conosco Agora e Aumente Suas Vendas!</h2>
        <a href="https://wa.me/5527996619274" target="_blank">WhatsApp</a>
    </section>

    <!-- Rodapé -->
    <footer>
        <div class="footer-logo">A.L Marketing</div>
        <div class="footer-columns">
            <ul class="footer-column">
                <li>Política de Privacidade</li>
                <li>Contato</li>
                <li>Termos de Uso</li>
            </ul>
            <ul class="footer-column">
                <li>Email: Allefyvidal@gmail.com</li>
                <li>WhatsApp: (27) 99661-9274</li>
            </ul>
        </div>
    </footer>

    <!-- Botão de WhatsApp Fixo -->
    <a href="https://wa.me/5527996619274" target="_blank" class="whatsapp-button">&#128172;</a>
</body>
</html>
