<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Currículo</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --cor-primaria: #2c3e50;
            --cor-secundaria: #ecf0f1;
            --cor-destaque: #3498db;
            --fonte-titulos: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            --fonte-texto: 'Helvetica Neue', Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--fonte-texto);
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
            padding-top: 70px; /* Espaço para o menu fixo */
        }

        h1, h2, h3, h4 {
            font-family: var(--fonte-titulos);
            color: var(--cor-primaria);
            margin-bottom: 15px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        section {
            padding: 40px 0;
        }
        nav {
            background-color: var(--cor-primaria);
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            padding: 15px 0;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: var(--cor-secundaria);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--cor-destaque);
        }
        header {
            background-color: var(--cor-secundaria);
            padding: 60px 0;
            text-align: center;
        }

        .perfil {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .perfil-nome {
            font-size: 2.5rem;
            margin-bottom: 20px;
            order: 1;
        }

        .perfil-foto {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid var(--cor-destaque);
            margin-bottom: 20px;
            order: 2;
        }

        .perfil-texto {
            max-width: 800px;
            margin: 0 auto 20px;
            font-size: 1.1rem;
            order: 3;
        }

        .perfil-contato {
            order: 4;
            margin-top: 20px;
        }

        /* Seções comuns */
        .secao-titulo {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        .secao-titulo::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: var(--cor-destaque);
            margin: 10px auto 0;
        }
        .registro {
            background-color: white;
            padding: 25px;
            margin-bottom: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .registro-titulo {
            color: var(--cor-destaque);
            margin-bottom: 10px;
        }

        .registro-subtitulo {
            font-weight: bold;
            margin-bottom: 10px;
            color: var(--cor-primaria);
        }

        .registro-data {
            color: #777;
            font-style: italic;
            margin-bottom: 15px;
        }
        .certificacao {
            background-color: white;
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .certificacao-titulo {
            font-weight: bold;
            color: var(--cor-destaque);
            margin-bottom: 10px;
        }
        #habilidades ul {
            display: flex;
            flex-wrap: wrap;
            list-style: none;
            justify-content: center;
        }

        #habilidades ul li {
            background-color: var(--cor-destaque);
            color: white;
            padding: 10px 20px;
            margin: 10px;
            border-radius: 30px;
            font-weight: 500;
        }

        /* Rodapé */
        footer {
            background-color: var(--cor-primaria);
            color: var(--cor-secundaria);
            padding: 40px 0;
            text-align: center;
        }

        .redes-sociais {
            margin-bottom: 20px;
        }

        .redes-sociais ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }

        .redes-sociais ul li {
            margin: 0 15px;
        }

        .redes-sociais ul li a {
            color: var(--cor-secundaria);
            font-size: 1.5rem;
            transition: color 0.3s;
        }

        .redes-sociais ul li a:hover {
            color: var(--cor-destaque);
        }

        .copyright {
            margin-top: 20px;
            font-size: 0.9rem;
        }
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
                padding: 10px 0;
            }

            nav ul li {
                margin: 5px 0;
            }

            .perfil-nome {
                font-size: 2rem;
            }

            .perfil-foto {
                width: 150px;
                height: 150px;
            }

            #habilidades ul {
                justify-content: flex-start;
            }
        }
    </style>
</head>
<body>
    <!-- Menu de Navegação -->
    <nav>
        <ul>
            <li><a href="#apresentacao">Início</a></li>
            <li><a href="#educacao">Educação</a></li>
            <li><a href="#certificacoes">Certificações</a></li>
            <li><a href="#experiencia">Experiência</a></li>
            <li><a href="#habilidades">Habilidades</a></li>
            <li><a href="#contato">Contato</a></li>
        </ul>
    </nav>

    <!-- Cabeçalho/Apresentação -->
    <header id="apresentacao">
        <div class="container">
            <div class="perfil">
                <h1 class="perfil-nome">Gabriel Macieira</h1>
                <img class="perfil-foto" src="https://placehold.co/300x300/3498db/FFFFFF?text=JS" alt="Foto de João da Silva">
                <p class="perfil-texto">
                    Formando bacharelado em Engenharia Mecanica
                </p>
                <div class="perfil-contato">
                    <p><i class="fas fa-envelope"></i>gabrielmms321@gmail.com</p>
                    <p><i class="fas fa-map-marker-alt"></i> Itabira, MG</p>
                </div>
            </div>
        </div>
    </header>

    <main class="container">
        <!-- Seção Educação -->
        <section id="educacao">
            <h2 class="secao-titulo">Educação</h2>
            
            <div class="registro">
                <h3 class="registro-titulo">Ensino medio completo/h3>
            <ul>
                <li>HTML5</li>
                <li>CSS3</li>
                <li>JavaScript</li>
                <li>React.js</li>
                <li>Vue.js</li>
                <li>Git</li>
                <li>Responsive Design</li>
                <li>UI/UX Design</li>
                <li>Web Accessibility</li>
                <li>API Integration</li>
            </ul>
        </section>
    </main>

    <!-- Rodapé -->
    <footer id="contato">
        <div class="container">
            <div class="redes-sociais">
                <ul>
                    <li><a href="#"><i class="fab fa-linkedin"></i></a></li>
                    <li><a href="#"><i class="fab fa-github"></i></a></li>
                    <li><a href="#"><i class="fab fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                </ul>
            </div>
            <p class="copyright">© 2025 Gabriel Macieira</p>
        </div>
    </footer>
</body>
</html>
