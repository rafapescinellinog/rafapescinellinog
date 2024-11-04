<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Filmes e Séries</title>
    <style>
        /* Reset básico */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #1c1c1c;
            color: #f4f4f4;
            line-height: 1.6;
        }

        /* Cabeçalho e Menu */
        header {
            background-color: #333;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            color: #f4f4f4;
            font-size: 1.8rem;
        }

        nav {
            margin-top: 10px;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: #f4f4f4;
            text-decoration: none;
            font-weight: bold;
            padding: 8px 15px;
            transition: background 0.3s;
        }

        nav ul li a:hover {
            background-color: #555;
            border-radius: 5px;
        }

        /* Estilos das Seções */
        main {
            padding: 2rem;
        }

        section {
            margin-bottom: 3rem;
            text-align: center;
        }

        section h2 {
            color: #ff6347;
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        section p {
            color: #ddd;
            font-size: 1rem;
            margin-bottom: 20px;
        }

        /* Card de Filmes e Séries */
        .card-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .card {
            background-color: #444;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .card img {
            max-width: 100%;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .card h3 {
            font-size: 1.2rem;
            margin-bottom: 100px;
            color: #f4f4f4;
        }

        .card p {
            font-size: 0.9rem;
            color: #ccc;
        }

        /* Rodapé */
        footer {
            background-color: #333;
            color: #f4f4f4;
            text-align: center;
            padding: 1rem 0;
        }
    </style>
</head>
<body>
    <!-- Cabeçalho e Menu -->
    <header>
        <h1>Filmes e Séries</h1>
        <nav>
            <ul>
                <li><a href="#inicio">Início</a></li>
                <li><a href="#filmes">Filmes</a></li>
                <li><a href="#series">Séries</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <!-- Conteúdo Principal -->
    <main>
        <section id="inicio">
            <h2>Bem-vindo ao CineFlex</h2>
            <p>Descubra os melhores lançamentos e clássicos do cinema e da TV!</p>
        </section>
        
        <section id="filmes">
            <h2>Filmes</h2>
            <p>Confira nossos filmes em destaque!</p>
            <div class="card-container">
                <div class="card">
                    <img src="data:image/jpeg;base64,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" alt="Sorria">
                    <h3>Sorria</h3>
                    <p>Em Sorria, tudo na vida da Dra. Rose Cotter (Sosie Bacon) muda, após uma paciente morrer de forma brutal em sua frente, e ela testemunhar o incidente bizarro e traumático no consultório.</p

    
 
     <section id="animação"
            <div class="card-container">
                <div class="card">
                    <img src="data:image/jpeg;base64,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" alt="Whish">
                    <h3>Whish</h3>
                    <p>O filme se passa no reino de Rosas, onde Asha, uma garota idealista, faz um desejo tão poderoso que é atendido por uma estrela.</p
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Filmes e Séries</title>
    <style>
        /* Reset básico */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #1c1c1c;
            color: #f4f4f4;
            line-height: 1.6;
        }

        /* Cabeçalho e Menu */
        header {
            background-color: #333;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            color: #f4f4f4;
            font-size: 1.8rem;
        }

        nav {
            margin-top: 10px;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: #f4f4f4;
            text-decoration: none;
            font-weight: bold;
            padding: 8px 15px;
            transition: background 0.3s;
        }

        nav ul li a:hover {
            background-color: #555;
            border-radius: 5px;
        }

        /* Estilos das Seções */
        main {
            padding: 2rem;
        }

        section {
            margin-bottom: 3rem;
            text-align: center;
        }

        section h2 {
            color: #ff6347;
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        section p {
            color: #ddd;
            font-size: 1rem;
            margin-bottom: 20px;
        }

        /* Card de Filmes e Séries */
        .card-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .card {
            background-color: #444;
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s;
        }

        .card:hover {
            transform: scale(1.05);
        }

        .card img {
            max-width: 100%;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .card h3 {
            font-size: 1.2rem;
            margin-bottom: 8px;
            color: #f4f4f4;
        }

        .card p {
            font-size: 0.9rem;
            color: #ccc;
        }

        /* Rodapé */
        footer {
            background-color: #333;
            color: #f4f4f4;
            text-align: center;
            padding: 1rem 0;
        }
    </style>
</head>
<body>
    <!-- Cabeçalho e Menu -->
    <header>
        <h1>Filmes e Séries</h1>
        <nav>
            <ul>
                <li><a href="inicio">Inicio</a></li>
                <li><a href="filmes">Filmes</a></li>
                <li><a href="series">Séries</a></li>
                <li><a href="contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <!-- Conteúdo Principal -->
    <main>
        <section id="inicio">
            <h2>Bem-vindo ao Site de Filmes e Séries</h2>
            <p>Descubra os melhores lançamentos e clássicos do cinema e da TV!</p>
        </section>
        
        <section id="filmes">
            <h2>Filmes</h2>
            <p>Confira nossos filmes em destaque!</p>
            <div class="card-container">
                <div class="card">
                    <img src="https://via.placeholder.com/200x300" alt="Filme 1">
                    <h3>Filme 1</h3>
                    <p>Descrição breve do filme 1.</p
