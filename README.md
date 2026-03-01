<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vyntra | Marketplace Digital Global</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Inter',sans-serif;}

body{
background:linear-gradient(180deg,#ffffff,#f2fcff);
color:#111;
}

header{
background:#00CFE8;
padding:20px 40px;
display:flex;
justify-content:space-between;
align-items:center;
color:white;
}

.logo{
font-size:24px;
font-weight:700;
}

nav a{
color:white;
text-decoration:none;
margin-left:25px;
font-weight:500;
cursor:pointer;
}

.hero{
padding:120px 20px;
text-align:center;
}

.hero h1{
font-size:48px;
margin-bottom:20px;
}

.hero p{
max-width:600px;
margin:0 auto 30px;
font-size:18px;
color:#444;
}

.btn{
background:#00CFE8;
color:white;
padding:15px 35px;
border:none;
border-radius:8px;
font-size:16px;
cursor:pointer;
transition:0.3s;
}

.btn:hover{
opacity:0.85;
}

.section{
padding:80px 20px;
text-align:center;
}

.cards{
display:flex;
justify-content:center;
gap:30px;
flex-wrap:wrap;
margin-top:40px;
}

.card{
background:white;
padding:30px;
border-radius:12px;
width:260px;
box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

footer{
background:#00CFE8;
color:white;
padding:20px;
text-align:center;
margin-top:60px;
}

.panel{
display:none;
padding:60px 20px;
text-align:center;
}

input{
padding:12px;
margin:10px;
width:220px;
border-radius:6px;
border:1px solid #ddd;
}

.dashboard-box{
background:white;
max-width:600px;
margin:30px auto;
padding:30px;
border-radius:12px;
box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

.stat{
margin:10px 0;
font-weight:600;
}
</style>

<script>
function show(page){
document.getElementById("home").style.display="none";
document.getElementById("produtor").style.display="none";
document.getElementById("aluno").style.display="none";
document.getElementById(page).style.display="block";
}
</script>

</head>
<body>

<header>
<div class="logo">Vyntra</div>
<nav>
<a onclick="show('home')">Home</a>
<a onclick="show('produtor')">Produtor</a>
<a onclick="show('aluno')">Aluno</a>
</nav>
</header>

<!-- HOME -->
<div id="home">

<section class="hero">
<h1>Venda qualquer produto digital no mundo 🌍</h1>
<p>A Vyntra é uma plataforma global para criadores venderem produtos digitais com segurança, afiliados e pagamentos integrados.</p>
<button class="btn" onclick="show('produtor')">Começar Agora</button>
</section>

<section class="section">
<h2>Por que escolher a Vyntra?</h2>

<div class="cards">
<div class="card">
<h3>7% por venda</h3>
<p>Taxa simples e transparente.</p>
</div>

<div class="card">
<h3>Afiliados</h3>
<p>Produtor define comissão personalizada.</p>
</div>

<div class="card">
<h3>Pagamentos</h3>
<p>Pix, Cartão e Boleto integrados.</p>
</div>
</div>
</section>

</div>

<!-- PRODUTOR -->
<div id="produtor" class="panel">
<h2>Painel do Produtor</h2>

<div class="dashboard-box">
<h3>Criar Produto</h3>
<input placeholder="Nome do produto">
<input placeholder="Preço (R$)">
<br>
<button class="btn">Publicar</button>
</div>

<div class="dashboard-box">
<h3>Estatísticas</h3>
<p class="stat">Vendas: 14</p>
<p class="stat">Saldo disponível: R$ 1.890</p>
<p class="stat">Taxa da Vyntra: 7%</p>
</div>

<button class="btn" onclick="show('home')">Voltar</button>
</div>

<!-- ALUNO -->
<div id="aluno" class="panel">
<h2>Área do Aluno</h2>

<div class="dashboard-box">
<h3>Seus Produtos</h3>
<p>✔ Curso Marketing Digital</p>
<p>✔ E-book Vendas Online</p>
</div>

<button class="btn" onclick="show('home')">Voltar</button>
</div>

<footer>
© 2026 Vyntra - Marketplace Digital Global
</footer>

</body>
</html>
