<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Salão de Beleza Luxo & Elegância</title>
<style>
* {
  margin:0;
  padding:0;
  box-sizing:border-box;
  scroll-behavior:smooth;
  font-family: Arial, sans-serif;
}

body {
  background:#111;
  color:#fff;
}

nav {
  position: fixed;
  width: 100%;
  background:#000;
  padding: 15px;
  text-align:center;
  z-index:1000;
}

nav a {
  color: gold;
  margin:0 15px;
  text-decoration:none;
  font-weight:bold;
  transition:0.3s;
}

nav a:hover {
  color: white;
}

section {
  padding:100px 20px;
  min-height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  background-size:cover;
  background-position:center;
  background-repeat:no-repeat;
  position:relative;
}

section::before {
  content:"";
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:rgba(0,0,0,0.75);
  z-index:0;
}

section > * {
  position:relative;
  z-index:1;
}

/* FUNDOS */
#home { background:url('https://images.unsplash.com/photo-1560066984-138dadb4c035') no-repeat center/cover; }
#servicos { background:url('https://images.unsplash.com/photo-1595476108010-b4d1f102b1b1') no-repeat center/cover; }
#sobre { background:url('https://images.unsplash.com/photo-1512496015851-a90fb38ba796?w=1600&q=80') no-repeat center/cover; }
#galeria { background:url('https://images.unsplash.com/photo-1604654894610-df63bc536371?w=1600&q=80') no-repeat center/cover; }
#contacto { background:url('https://images.unsplash.com/photo-1519415510236-718bdfcd89c8?w=1600&q=80') no-repeat center/cover; }

.overlay {
  background:rgba(0,0,0,0.7);
  padding:40px;
  border-radius:20px;
  max-width:950px;
  width:90%;
}

h1 { font-size:50px; margin-bottom:20px; color:gold; }
h2 { margin-bottom:20px; color:gold; }
p { max-width:600px; margin-bottom:20px; }

button {
  padding:15px 30px;
  background:gold;
  border:none;
  border-radius:10px;
  cursor:pointer;
  font-weight:bold;
  transition:0.3s;
}

button:hover { transform:scale(1.1); box-shadow:0 0 20px gold; }

.cards {
  display:flex;
  flex-wrap:wrap;
  gap:20px;
  justify-content:center;
}

.card {
  background:#222;
  padding:20px;
  border-radius:15px;
  width:250px;
  transition:0.3s;
}

.card:hover { transform:translateY(-10px); }

.gallery {
  display:flex;
  flex-wrap:wrap;
  gap:15px;
  justify-content:center;
}

.gallery img {
  width:250px;
  border-radius:15px;
  transition:0.3s;
}

.gallery img:hover { transform:scale(1.1); }

/* TODOS OS VÍDEOS MESMO TAMANHO (igual ao 2º que gostaste) */
video, iframe {
  width:100%;
  max-width:800px;
  height:400px;  /* define altura igual para todos */
  border-radius:40px;
  margin-top:40px;
}

footer {
  background:#000;
  padding:20px;
  text-align:center;
}
</style>
</head>

<body>

<nav>
<a href="#home">🌸 Início</a>
<a href="#servicos">💅 Serviços</a>
<a href="#sobre">💄 Sobre</a>
<a href="#galeria">📸 Galeria</a>
<a href="#contacto">💗 Contato</a>
</nav>

<section id="home">
<div class="overlay">
<h1>💖✨ Salão de Beleza Luxo & Elegância</h1>
<p>🌸 Sofisticação, delicadeza e poder feminino em cada detalhe.</p>
<button onclick="window.location.href='#servicos'">Conhecer Serviços</button>
</div>
</section>

<section id="servicos">
<h2>💅👑 Nossos Serviços</h2>
<div class="cards">
<div class="card">
<h3>💇‍♀️ Tranças & Cabelo</h3>
<p>Estilos modernos e elegantes.</p>
</div>
<div class="card">
<h3>💅 Manicure & Pedicure</h3>
<p>Unhas delicadas e irresistíveis.</p>
</div>
<div class="card">
<h3>💄 Maquilhagem Profissional</h3>
<p>Realce sua beleza natural.</p>
</div>
<div class="card">
<h3>🌷 Tratamentos Faciais</h3>
<p>Pele radiante e iluminada.</p>
</div>
<div class="card">
<h3>👰‍♀️ Dia da Noiva</h3>
<p>Experiência exclusiva e luxuosa.</p>
</div>
</div>
</section>

<section id="sobre">
<h2>💄🌷 Sobre Nós</h2>
<p>Um espaço criado especialmente para valorizar a beleza feminina.</p>
<h3>🎥✨ Conheça o nosso ambiente:</h3>

<iframe 
  src="https://drive.google.com/file/d/1_hl5HcAZvMRpfvuay62quNkgV2gURrJ0/preview" 
  width="100%" 
  height="300" 
  allowfullscreen
  allow="autoplay"
  style="border-radius:10px; margin-top:10px; border:none;">
</iframe>

<iframe 
  src="https://drive.google.com/file/d/1yMQjxRlKgXYub3ptVfgBtW2cj25XO0rN/preview?autoplay=1" 
  width="100%" 
  height="300" 
  allowfullscreen
  allow="autoplay"
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>

<iframe 
  src="https://drive.google.com/file/d/1TyndF6fYd8GSKm25suzlkX5pTgisKnE6/preview?autoplay=1" 
  width="100%" 
  height="300" 
  allowfullscreen
  allow="autoplay"
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>

<iframe 
  src="https://drive.google.com/file/d/19RtNaGCNJMR244cmgasN-yru5QtNmCDV/preview?autoplay=1" 
  width="100%" 
  height="300" 
  allowfullscreen
  allow="autoplay"
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>

<iframe 
  src="https://drive.google.com/file/d/1VvbXWYb3Ca3-3jREMz5EaNaGIe_qRJpo/preview?autoplay=1" 
  width="100%" 
  height="300" 
  allow="autoplay"
  allowfullscreen
  style="border-radius:20px; margin-top:20px; border:none;">
</iframe>
</section>

<section id="galeria">
<h2>📸💖 Galeria Feminina</h2>
<div class="gallery">

  <img src="https://images.unsplash.com/photo-1633681926022-84c23e8cb2d6?w=600&q=80" alt="Salão de Beleza">
  <img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?w=600&q=80" alt="Cabelo e Tranças">
  <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?w=600&q=80" alt="Kit de Maquilhagem">
  <img src="https://images.unsplash.com/photo-1519014816548-bf5fe059798b?w=600&q=80" alt="Unhas das mãos">
  <img src="https://images.unsplash.com/photo-1519415510236-718bdfcd89c8?w=600&q=80" alt="Unhas dos Pés">

</div>
</section>

<section id="contacto">
<h2>📍💗 Contato & Localização</h2>
<p>🌸 Agende o seu momento de beleza connosco.</p>

<a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Gostaria%20de%20marcar%20um%20horário." target="_blank">
<button>📲 Agendar via WhatsApp</button>
</a>

<iframe
src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3153.019600374382!2d-9.139337384681203!3d38.72225217957039!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xd19331f1f1c9af5%3A0xa1b7e4a69e2c1e3f!2sLisboa!5e0!3m2!1spt-PT!2spt!4v1672800000000"
width="600" height="450"
style="border:0; border-radius:20px; margin-top:20px;"
allowfullscreen=""
loading="lazy">
</iframe>

</section>

<footer>
<p>© 2026 Salão de Beleza Luxo & Elegância – Beleza é Poder 💕✨</p>
</footer>

</body>
</html>
