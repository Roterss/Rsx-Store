<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RSX STORE - Loja de Discord</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #1e1e2f;
            color: #ffffff;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #2c2c54;
            padding: 20px;
            text-align: center;
            border-bottom: 2px solid #9d4edd;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav {
            margin-top: 20px;
            text-align: center;
        }
        nav a {
            color: #ffffff;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.2em;
        }
        nav a:hover {
            color: #9d4edd;
        }
        .banner {
            text-align: center;
            margin: 20px 0;
        }
        .banner img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            text-align: center;
        }
        .products {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        .product {
            background-color: #2c2c54;
            padding: 20px;
            border-radius: 10px;
            width: 300px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            position: relative;
        }
        .product img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }
        .product h2 {
            margin-top: 0;
            color: #9d4edd;
        }
        .btn-buy {
            background-color: #9d4edd;
            color: #ffffff;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
            margin-top: 10px;
            transition: background-color 0.3s;
        }
        .btn-buy:hover {
            background-color: #7a34c5;
        }
        .btn-info {
            background-color: transparent;
            color: #9d4edd;
            border: 1px solid #9d4edd;
            padding: 5px 10px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.9em;
            margin-top: 5px;
        }
        .btn-info:hover {
            background-color: #9d4edd;
            color: #ffffff;
        }
        .discord-btn {
            display: inline-block;
            background-color: #7289da;
            color: #ffffff;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-size: 1.2em;
            margin-top: 20px;
        }
        .discord-btn:hover {
            background-color: #5a6fb7;
        }
        .gif {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 10;
        }
        footer {
            background-color: #2c2c54;
            padding: 20px;
            text-align: center;
            margin-top: 40px;
        }
        footer p {
            margin: 0;
            font-size: 0.9em;
        }
    </style>
</head>
<body>

<header>
    <h1>RSX STORE</h1>
    <nav>
        <a href="#">Início</a>
        <a href="#">Produtos</a>
        <a href="#">Contato</a>
    </nav>
</header>

<div class="banner">
    <img src="https://cdn.discordapp.com/attachments/1227270610238046239/1275657625064837182/Banner_rsxstore.jpg?ex=66c6b03e&is=66c55ebe&hm=7c63d0b40035d9cc5af1361c2d69ce3049ea5ba7c84f6de0da8469251d26385a" alt="Banner RSX STORE">
</div>

<div class="container">
    <a class="discord-btn" href="https://discord.gg/rsxstore" target="_blank">Entre no nosso Discord</a>
    
    <div class="products">
        <div class="product">
            <img src="https://via.placeholder.com/300x150.png?text=Nitro+Mensal" alt="Nitro Mensal">
            <h2>Nitro Mensal</h2>
            <button class="btn-info" onclick="toggleDescription('desc1')">Descrição</button>
            <div id="desc1" style="display:none;">
                <p>Obtenha 1 mês de Discord Nitro com todos os benefícios incríveis, incluindo aumento de servidores, emojis animados e muito mais.</p>
            </div>
            <button class="btn-buy">Comprar Agora</button>
        </div>

        <div class="product">
            <img src="https://via.placeholder.com/300x150.png?text=Nitro+Trimestral" alt="Nitro Trimestral">
            <h2>Nitro Trimestral</h2>
            <button class="btn-info" onclick="toggleDescription('desc2')">Descrição</button>
            <div id="desc2" style="display:none;">
                <p>Aproveite 3 meses de Discord Nitro e economize. Perfeito para quem quer prolongar a diversão no Discord.</p>
            </div>
            <button class="btn-buy">Comprar Agora</button>
        </div>
    </div>
    
    <div class="gif">
        <a href="https://discord.gg/rsxstore" target="_blank">
            <img src="https://cdn.discordapp.com/attachments/1227270610238046239/1275657604898619465/GIF_rsxstore.gif?ex=66c6b039&is=66c55eb9&hm=4160d692711d8f791f86648da6126da029d509fb2d4238d655b86b6a53fb6520" alt="GIF RSX STORE" style="max-width: 150px; height: auto;">
        </a>
    </div>
</div>

<footer>
    <p>&copy; 2024 RSX STORE - Todos os direitos reservados.</p>
</footer>

<script>
    function toggleDescription(descId) {
        const desc = document.getElementById(descId);
        if (desc.style.display === "none") {
            desc.style.display = "block";
        } else {
            desc.style.display = "none";
        }
    }
</script>

</body>
</html>
