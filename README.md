# Projeto-

2026 
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Meu Site</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #0f172a;
            color: white;
        }

        header {
            width: 100%;
            padding: 20px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #020617;
            position: fixed;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #38bdf8;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 25px;
            transition: 0.3s;
        }

        nav a:hover {
            color: #38bdf8;
        }

        .hero {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 100px 20px 40px;
            background:
                radial-gradient(circle at top, #1e3a8a, transparent 40%),
                #0f172a;
        }

        .hero-content {
            max-width: 800px;
        }

        .hero h1 {
            font-size: clamp(42px, 8vw, 80px);
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #38bdf8;
        }

        .hero p {
            font-size: 20px;
            color: #cbd5e1;
            line-height: 1.6;
            margin-bottom: 35px;
        }

        .button {
            display: inline-block;
            background: #2563eb;
            color: white;
            text-decoration: none;
            padding: 15px 30px;
            border-radius: 10px;
            font-size: 18px;
            transition: 0.3s;
        }

        .button:hover {
            background: #1d4ed8;
            transform: translateY(-3px);
        }

        section {
            padding: 100px 8%;
            text-align: center;
        }

        section h2 {
            font-size: 40px;
            margin-bottom: 20px;
        }

        section > p {
            color: #94a3b8;
            font-size: 18px;
            max-width: 700px;
            margin: 0 auto 50px;
            line-height: 1.6;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 25px;
            max-width: 1000px;
            margin: auto;
        }

        .card {
            background: #1e293b;
            padding: 35px 25px;
            border-radius: 15px;
            border: 1px solid #334155;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-8px);
            border-color: #38bdf8;
        }

        .card h3 {
            color: #38bdf8;
            margin-bottom: 15px;
            font-size: 22px;
        }

        .card p {
            color: #cbd5e1;
            line-height: 1.6;
        }

        .contact {
            background: #020617;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #020617;
            color: #64748b;
        }

        @media (max-width: 700px) {
            header {
                padding: 18px 5%;
            }

            nav a {
                margin-left: 10px;
                font-size: 14px;
            }

            section {
                padding: 80px 5%;
            }

            .hero p {
                font-size: 17px;
            }
        }
    </style>
</head>

<body>

    <header>
        <div class="logo">MeuSite</div>

        <nav>
            <a href="#inicio">Início</a>
            <a href="#sobre">Sobre</a>
            <a href="#servicos">Serviços</a>
            <a href="#contato">Contato</a>
        </nav>
    </header>

    <main>

        <section class="hero" id="inicio">
            <div class="hero-content">

                <h1>
                    Olá, eu sou <span>você</span> 👋
                </h1>

                <p>
                    Bem-vindo ao meu primeiro site criado com
                    Python e Flask.
                </p>

                <a class="button" href="#sobre">
                    Conheça o projeto
                </a>

            </div>
        </section>

        <section id="sobre">

            <h2>Sobre</h2>

            <p>
                Esta é uma página criada com Python usando o framework Flask.
                O projeto pode ser colocado no GitHub e posteriormente publicado
                na internet.
            </p>

            <div class="cards">

                <div class="card">
                    <h3>🐍 Python</h3>
                    <p>
                        A aplicação utiliza Python como linguagem principal.
                    </p>
                </div>

                <div class="card">
                    <h3>🌐 Flask</h3>
                    <p>
                        Flask é utilizado para criar o servidor e as rotas
                        da aplicação.
                    </p>
                </div>

                <div class="card">
                    <h3>💻 HTML</h3>
                    <p>
                        HTML estrutura todo o conteúdo apresentado na página.
                    </p>
                </div>

            </div>

        </section>

        <section id="servicos">

            <h2>Serviços</h2>

            <p>
                Você pode modificar esta seção para apresentar seus projetos,
                serviços, produtos ou qualquer outra informação.
            </p>

            <div class="cards">

                <div class="card">
                    <h3>Projeto 1</h3>
                    <p>
                        Descrição do seu primeiro projeto.
                    </p>
                </div>

                <div class="card">
                    <h3>Projeto 2</h3>
                    <p>
                        Descrição do seu segundo projeto.
                    </p>
                </div>

                <div class="card">
                    <h3>Projeto 3</h3>
                    <p>
                        Descrição do seu terceiro projeto.
                    </p>
                </div>

            </div>

        </section>

        <section class="contact" id="contato">

            <h2>Contato</h2>

            <p>
                Quer entrar em contato? Coloque aqui seu e-mail,
                Instagram, GitHub ou outras redes sociais.
            </p>

            <a class="button" href="mailto:seuemail@email.com">
                Enviar mensagem
            </a>

        </section>

    </main>

    <footer>
        © 2026 MeuSite. Todos os direitos reservados.
    </footer>

</body>

</html>
