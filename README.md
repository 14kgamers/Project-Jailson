
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        header {
            background-color: #333;
            color: white;
            padding: 1em;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            cursor: pointer;
        }

        nav a:hover {
            text-decoration: underline;
        }

        .page {
            display: none;
            padding: 20px;
        }

        .active {
            display: block;
        }

        footer {
            background-color: #333;
            color: white;
            padding: 1em;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <header>
        <nav>
            <a onclick="showPage('home')">Inicio</a>
            <a onclick="showPage('about')">Sobre</a>
            <a onclick="showPage('contact')">Notas</a>
        </nav>
    </header>

    <main>
        <!-- Home Page -->
        <div id="home" class="page active">
            <h1>O Inicio de Tudo</h1>
            <p>Jailson Mendes, nascido Valdemar Gonçalves, ficou conhecido na internet brasileira como um ícone de memes e da cultura pop underground.
                 Originalmente motoboy, onde ele ganhou fama ao atuar em filmes onde se tornou viral, consolidando sua imagem como uma figura humorística.
                  Mesmo após sua morte em 2018, Jailson continua a ser reverenciado na internet, especialmente em memes, figurinhas e montagens,  que celebram seu carisma e bordões icônicos.</p>
            <img src="https://th.bing.com/th/id/OIP.uFzIz9lvWz3B_zNW513PrgHaHa?rs=1&pid=ImgDetMain" alt="Placeholder Image">
        </div>

        <!-- About Page -->
        <div id="about" class="page">
            <h1>Seu Legado</h1>
            <img src="https://i.ytimg.com/vi/_2Pc9Uv7TY0/maxresdefault.jpg" alt="Placeholder Image" height="300px"> 
            <p style="text-align: left;">Nos filmes de Jailson Mendes, ele interpretou uma variedade de profissões, muitas vezes de forma caricata e humorística, o que contribuiu para o tom exagerado dos vídeos. Alguns dos "papéis" que ele desempenhou incluem:</p>

<p style="text-align: left;"><strong>Motoboy</strong> - Uma das profissões mais associadas à imagem de Jailson, já que ele trabalhou como motoboy antes de entrar para os filmes adultos.</p>

<p style="text-align: left;"><strong>Mecânico</strong> - Em um dos vídeos mais famosos, ele aparece como um mecânico, reforçando o estereótipo de trabalhador manual.</p>

<p style="text-align: left;"><strong>Entregador de gás</strong> - Outro papel que ele interpretou, envolvendo uma interação cômica com os clientes.</p>

<p style="text-align: left;"><strong>Pedreiro</strong> - Uma profissão frequentemente retratada em filmes com um viés mais fantasioso e estereotipado.</p>

<p style="text-align: left;">Esses papéis faziam parte da estética dos filmes, misturando o humor com situações cotidianas.</p>

        </div>

        <!-- Contact Page -->
        <div id="contact" class="page">
            <h1>Aqui jas "Ai que delicia"</h1>
            <img src="https://th.bing.com/th/id/OIP.fg3NATJTE_z7UG8ltWLfygHaFj?w=259&h=194&c=7&r=0&o=5&pid=1.7" alt="Placeholder Image" height="300px">
            <p><strong>Nota de Falecimento</strong>

                É com pesar que informamos o falecimento de Jailson Mendes, um ícone da cultura pop brasileira e figura marcante na internet. Jailson, conhecido por seu carisma e humor irreverente, conquistou a simpatia de muitos com seus papéis cômicos e bordões inesquecíveis. Sua contribuição para o entretenimento e a cultura de memes deixou uma marca indelével em diversos fãs e seguidores.
                
                Jailson Mendes faleceu no dia 29 de Junho de 2018, aos 48 anos. Sua presença na mídia e na vida de muitos será sempre lembrada com carinho e saudade.
                
                Nossos sentimentos à família, amigos e a todos que foram tocados pela sua energia e alegria.</p>
        </div>
    </main>

    <footer>
        <p>&copy; 2024 Vitor e o cara</p>
    </footer>

    <script>
        function showPage(pageId) {
            // Hide all pages
            var pages = document.querySelectorAll('.page');
            pages.forEach(function(page) {
                page.classList.remove('active');
            });

            // Show the selected page
            var selectedPage = document.getElementById(pageId);
            selectedPage.classList.add('active');
        }
    </script>

</body>
</html>
