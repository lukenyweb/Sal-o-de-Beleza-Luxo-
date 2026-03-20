<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Salão de Beleza Luxo & Elegância</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Bebas+Neue&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
:root {
  --rose: #C9748C;
  --rose-light: #F0A0B8;
  --rose-dim: #7a3a4a;
  --gold: #C9A84C;
  --gold-light: #F0D080;
  --black: #050303;
}

* { margin:0; padding:0; box-sizing:border-box; }

body {
  font-family: 'DM Sans', sans-serif;
  color: #fff;
  background: var(--black);
  overflow-x: hidden;
}

h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(32px, 8vw, 72px);
  font-weight: 300;
  color: var(--gold-light);
  line-height: 1.1;
  margin-bottom: 16px;
  text-shadow: 0 2px 24px rgba(0,0,0,0.8);
}
h2 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(26px, 6vw, 54px);
  font-weight: 300;
  color: var(--gold-light);
  line-height: 1.15;
  margin-bottom: 14px;
}
p {
  font-size: clamp(13px, 3vw, 16px);
  color: rgba(255,255,255,0.7);
  line-height: 1.8;
  margin: 12px 0;
  font-weight: 300;
}

.label {
  font-size: 10px;
  letter-spacing: 5px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 12px;
  display: block;
}

button {
  padding: 13px 36px;
  font-family: 'DM Sans', sans-serif;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 2.5px;
  text-transform: uppercase;
  background: var(--gold);
  color: #000;
  border: none;
  cursor: pointer;
  margin: 8px;
  transition: all 0.3s;
  clip-path: polygon(8px 0%, 100% 0%, calc(100% - 8px) 100%, 0% 100%);
}
button:hover {
  background: var(--gold-light);
  transform: translateY(-2px);
  box-shadow: 0 12px 32px rgba(201,168,76,0.3);
}
button.btn-outline {
  background: transparent;
  color: var(--gold);
  border: 1px solid var(--rose-dim);
}
button.btn-outline:hover {
  background: rgba(201,168,76,0.08);
  border-color: var(--gold);
}

.page {
  width: 100%;
  min-height: 100vh;
  display: none;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-size: cover;
  background-position: center;
  animation: fadeIn 0.8s ease;
  padding: 20px;
  position: relative;
}
.page::before {
  content: '';
  position: absolute; inset: 0;
  background: rgba(5,2,3,0.78);
}
.active { display: flex; }

.overlay {
  background: rgba(0,0,0,0.55);
  border: 1px solid rgba(201,168,76,0.15);
  padding: clamp(28px, 6vw, 60px);
  width: 100%;
  max-width: 780px;
  position: relative;
  z-index: 1;
}
.overlay::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
}

.gold-line {
  width: 48px; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 18px auto;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(12px); }
  to   { opacity: 1; transform: translateY(0); }
}

.btn-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 4px;
  margin-top: 20px;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  justify-content: center;
  margin: 20px 0;
}
.card {
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(201,168,76,0.2);
  padding: 18px 22px;
  min-width: 130px;
  max-width: 170px;
  flex: 1;
  transition: 0.3s;
}
.card:hover {
  border-color: rgba(201,168,76,0.5);
  background: rgba(201,168,76,0.07);
  transform: translateY(-4px);
}
.card h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(14px, 3vw, 18px);
  font-weight: 400;
  color: var(--gold-light);
  margin-bottom: 6px;
}
.card p { font-size: clamp(11px, 2.5vw, 13px); margin: 0; }

.video-wrap {
  width: 100%;
  margin: 14px 0;
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid rgba(201,168,76,0.2);
  background: #000;
}
.video-wrap iframe {
  width: 100%;
  height: 220px;
  border: none;
  display: block;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
  margin: 16px 0;
}
.gallery img {
  width: 100%;
  aspect-ratio: 1;
  object-fit: cover;
  border-radius: 10px;
  border: 1px solid rgba(201,168,76,0.15);
  transition: 0.3s;
}
.gallery img:hover {
  border-color: rgba(201,168,76,0.5);
  transform: scale(1.02);
}

.scroll-overlay {
  max-height: 85vh;
  overflow-y: auto;
  scrollbar-width: thin;
  scrollbar-color: var(--gold) transparent;
}
.scroll-overlay::-webkit-scrollbar { width: 4px; }
.scroll-overlay::-webkit-scrollbar-track { background: transparent; }
.scroll-overlay::-webkit-scrollbar-thumb { background: var(--gold); border-radius: 2px; }
</style>
</head>
<body>

<!-- PÁGINA 1 — INÍCIO -->
<div id="p1" class="page active" style="background-image:url('https://images.unsplash.com/photo-1560066984-138dadb4c035?w=1600&q=80');">
  <div class="overlay">
    <span class="label">°•°.Beleza Feminina de Luxo</span>
    <h1>💖 Salão de Beleza<br><em style="font-style:italic">Luxo & Elegância</em></h1>
    <div class="gold-line"></div>
    <p>Sofisticação, delicadeza e poder feminino em cada detalhe.<br>O teu espaço de transformação e confiança.</p>
    <div class="btn-group">
      <button onclick="goTo('p2')">Descobrir</button>
    </div>
  </div>
</div>

<!-- PÁGINA 2 — SERVIÇOS -->
<div id="p2" class="page" style="background-image:url('https://images.unsplash.com/photo-1595476108010-b4d1f102b1b1?w=1600&q=80');">
  <div class="overlay">
    <span class="label">O que oferecemos</span>
    <h2>💅 Serviços</h2>
    <div class="gold-line"></div>
    <div class="cards">
      <div class="card">
        <h3>💇‍♀️ Cabelo</h3>
        <p>Tranças, cortes e estilos modernos</p>
      </div>
      <div class="card">
        <h3>💅 Unhas</h3>
        <p>Manicure & Pedicure delicados</p>
      </div>
      <div class="card">
        <h3>💄 Maquilhagem</h3>
        <p>Realce a sua beleza natural</p>
      </div>
      <div class="card">
        <h3>🌷 Facial</h3>
        <p>Tratamentos para pele radiante</p>
      </div>
      <div class="card">
        <h3>👰‍♀️ Noiva</h3>
        <p>Experiência exclusiva e luxuosa</p>
      </div>
    </div>
    <div class="btn-group">
      <button onclick="goTo('p3')">Ver Ambiente</button>
      <button class="btn-outline" onclick="goTo('p1')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 3 — VÍDEOS -->
<div id="p3" class="page" style="background-image:url('https://images.unsplash.com/photo-1512496015851-a90fb38ba796?w=1600&q=80');">
  <div class="overlay scroll-overlay">
    <span class="label">O nosso espaço</span>
    <h2>🎥 Conheça o Ambiente</h2>
    <div class="gold-line"></div>
    <p>Veja de perto a nossa elegância e sofisticação.</p>

    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1_hl5HcAZvMRpfvuay62quNkgV2gURrJ0/preview" allow="autoplay" allowfullscreen></iframe>
    </div>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1yMQjxRlKgXYub3ptVfgBtW2cj25XO0rN/preview" allow="autoplay" allowfullscreen></iframe>
    </div>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1TyndF6fYd8GSKm25suzlkX5pTgisKnE6/preview" allow="autoplay" allowfullscreen></iframe>
    </div>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1sKde81XAHy_P9n5IVB7CqPTXWFu5zEye/preview" allow="autoplay" allowfullscreen></iframe>
    </div>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1VvbXWYb3Ca3-3jREMz5EaNaGIe_qRJpo/preview" allow="autoplay" allowfullscreen></iframe>
    </div>

    <div class="btn-group">
      <button onclick="goTo('p4')">Galeria</button>
      <button class="btn-outline" onclick="goTo('p2')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 4 — GALERIA -->
<div id="p4" class="page" style="background-image:url('https://images.unsplash.com/photo-1604654894610-df63bc536371?w=1600&q=80');">
  <div class="overlay scroll-overlay">
    <span class="label">Transformações reais</span>
    <h2>📸 Galeria Feminina</h2>
    <div class="gold-line"></div>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1633681926022-84c23e8cb2d6?w=600&q=80" alt="Salão de Beleza">
      <img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?w=600&q=80" alt="Cabelo e Tranças">
      <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?w=600&q=80" alt="Maquilhagem">
      <img src="https://images.unsplash.com/photo-1519014816548-bf5fe059798b?w=600&q=80" alt="Unhas das mãos">
    </div>
    <div class="btn-group">
      <button onclick="goTo('p5')">Contacto</button>
      <button class="btn-outline" onclick="goTo('p3')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 5 — CONTACTO -->
<div id="p5" class="page" style="background-image:url('https://images.unsplash.com/photo-1519415510236-718bdfcd89c8?w=1600&q=80');">
  <div class="overlay">
    <span class="label">Marcações</span>
    <h2>💗 Agendar Agora</h2>
    <div class="gold-line"></div>
    <p>O teu momento de beleza começa aqui.<br>Fala connosco agora mesmo no WhatsApp.</p>
    <div class="btn-group">
      <a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Gostaria%20de%20marcar%20um%20horário.🌸" target="_blank">
        <button>📲 WhatsApp</button>
      </a>
      <button class="btn-outline" onclick="goTo('p4')">Voltar</button>
    </div>
  </div>
</div>

<script>
function goTo(page) {
  document.querySelector('.active').classList.remove('active');
  document.getElementById(page).classList.add('active');
  window.scrollTo(0,0);
}
</script>
</body>
</html>
