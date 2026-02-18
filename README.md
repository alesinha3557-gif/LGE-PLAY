<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>LGE PLAY</title>

<style>
body{
margin:0;
font-family:Arial;
background:#0b1020;
color:white;
}

header{
text-align:center;
padding:30px;
background:linear-gradient(90deg,#0c1445,#09122e);
}

.logo{
width:160px;
}

.container{
max-width:1100px;
margin:auto;
padding:20px;
}

.box{
background:#111a33;
padding:20px;
border-radius:12px;
margin:15px 0;
}

.planos{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.plano{
background:#141f3d;
padding:25px;
border-radius:12px;
text-align:center;
}

.preco{
font-size:28px;
color:#4da6ff;
}

.btn{
background:#4da6ff;
padding:12px 18px;
border-radius:8px;
color:white;
text-decoration:none;
display:inline-block;
margin-top:10px;
cursor:pointer;
border:none;
}

input{
width:100%;
padding:12px;
margin:8px 0;
border-radius:6px;
border:none;
}

footer{
text-align:center;
padding:20px;
background:#0a0f22;
}
</style>
</head>

<body>

<header>
<img src="logo.png" class="logo">
<h1>LGE PLAY</h1>
<p>Canais • Filmes • Séries • Esportes</p>
</header>

<div class="container">

<div class="box">
<h2>📺 Vantagens</h2>
<ul>
<li>HD e Full HD</li>
<li>Smart TV, TV Box e celular</li>
<li>Suporte rápido</li>
<li>Atualizações diárias</li>
</ul>
</div>

<h2>💰 Planos</h2>

<div class="planos">

<div class="plano">
<h3>Básico</h3>
<p class="preco">R$25</p>
<button class="btn" onclick="copiarPix()">Pagar com Pix</button>
</div>

<div class="plano">
<h3>Padrão</h3>
<p class="preco">R$30</p>
<button class="btn" onclick="copiarPix()">Pagar com Pix</button>
</div>

<div class="plano">
<h3>Premium</h3>
<p class="preco">R$35</p>
<button class="btn" onclick="copiarPix()">Pagar com Pix</button>
</div>

</div>

<div class="box">
<h2>💳 Pagamento Pix</h2>
<p>Chave Pix:</p>
<p id="pix">SUA-CHAVE-PIX-AQUI</p>
<button class="btn" onclick="copiarPix()">Copiar Chave Pix</button>
</div>

<div class="box">
<h2>🧪 Teste Grátis</h2>
<input placeholder="LGE PLAY<img width="1024" height="1024" alt="1000052446" src="https://github.com/user-attachments/assets/8e5d719f-98ec-4f94-8274-b9b3a7f7cf5b" />
">
<input placeholder="27992238857">
<a class="btn" href="https://wa.me/5527992238857">Solicitar Teste</a>
</div>

</div>

<footer>
<p>LGE PLAY © 2026</p>
</footer>

<script>
function copiarPix(){
var chave = document.getElementById("pix").innerText;
navigator.clipboard.writeText(chave);
alert("Chave Pix copiada!");
}
</script>

</body>
</html>
