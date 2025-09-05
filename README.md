<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rodrigo Bina - Designer Multimídia</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Sidebar -->
  <aside class="sidebar">
    <div class="logo">R</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#projetos">Projetos</a>
      <a href="#contato">Contato</a>
    </nav>
  </aside>

  <!-- Hero -->
  <header id="home" class="hero">
    <div class="hero-content">
      <img src="sua-foto.jpg" alt="Rodrigo Bina" class="perfil">
      <div>
        <h1>Olá, sou o<br><span>Rodrigo Bina</span><br>Designer Multimídia</h1>
        <a href="#contato" class="btn">Solicitar Orçamento</a>
        <div class="socials">
          <a href="#">Instagram</a>
          <a href="#">LinkedIn</a>
        </div>
      </div>
    </div>
  </header>

  <!-- Missão -->
  <section class="missao">
    <h2>Nossa missão</h2>
    <div class="cards">
      <article class="card">
        <h3>Design com resultado</h3>
        <p>Crio soluções visuais pensadas para atrair atenção, gerar desejo e mover seu público à ação.</p>
      </article>
      <article class="card">
        <h3>Nosso Propósito Central</h3>
        <p>Elevar a experiência digital através de design estratégico que destaca sua marca.</p>
      </article>
      <article class="card">
        <h3>Acompanhamento estratégico</h3>
        <p>Trabalho lado a lado com você para ajustar e evoluir o design conforme o mercado.</p>
      </article>
    </div>
  </section>

  <!-- Projetos -->
  <section id="projetos" class="projetos">
    <div class="projeto">
      <img src="projeto1.jpg" alt="Projeto Cibersegurança">
      <p>Implementação de soluções de cibersegurança para uma rede social.</p>
    </div>
    <div class="projeto">
      <img src="projeto2.jpg" alt="App de recarga elétrica">
      <p>1º aplicativo de recarga para carros elétricos.</p>
    </div>
    <div class="projeto">
      <img src="projeto3.jpg" alt="Plataforma de moda ESG">
      <p>Desenvolvimento de uma plataforma de vendas online para moda ESG.</p>
    </div>
  </section>

  <!-- Premiações -->
  <section class="premiacoes">
    <h2>Premiações</h2>
    <p>
      Sou Rodrigo Bina, designer multimídia apaixonado por criar experiências visuais que conectam pessoas e marcas.
      Transformo ideias em soluções estratégicas de design, combinando criatividade, atenção aos detalhes e foco em resultados.
      Meu objetivo é ajudar marcas a se destacarem, conquistarem o público e atingirem seus objetivos de forma única e memorável.
    </p>
  </section>

  <!-- Contato -->
  <section id="contato" class="contato">
    <h2>Se interessou?</h2>
    <a href="mailto:seuemail@email.com" class="btn">Entre em contato</a>
  </section>

  <!-- Rodapé -->
  <footer>
    <div class="logo-footer">spiral tech.</div>
    <nav>
      <a href="#">Home</a>
      <a href="#">Serviços</a>
      <a href="#">Contato</a>
    </nav>
    <div class="socials">
      <a href="#">LinkedIn</a>
      <a href="#">Instagram</a>
    </div>
  </footer>
</body>
</html>
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Inter", Arial, sans-serif;
  background: #fdfdfd;
  color: #333;
  line-height: 1.6;
}

/* Sidebar */
.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 80px;
  height: 100%;
  background: #1a1a1a;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}

.sidebar .logo {
  font-size: 2rem;
  font-weight: bold;
  margin-bottom: 30px;
}

.sidebar nav {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.sidebar nav a {
  color: white;
  text-decoration: none;
  font-size: 0.9rem;
  transition: 0.3s;
}

.sidebar nav a:hover {
  color: #19d3a0;
}

/* Hero */
.hero {
  margin-left: 80px;
  min-height: 100vh;
  background: linear-gradient(135deg, #19d3a0, #0a9b8d);
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 60px 20px;
  color: white;
}

.hero-content {
  display: flex;
  gap: 40px;
  align-items: center;
  flex-wrap: wrap;
  text-align: left;
}

.hero .perfil {
  width: 220px;
  border-radius: 20px;
}

.hero h1 {
  font-size: 2rem;
}

.hero h1 span {
  font-weight: bold;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 24px;
  border-radius: 25px;
  background: white;
  color: #000;
  font-weight: bold;
  text-decoration: none;
  transition: 0.3s;
}

.btn:hover {
  background: #eee;
}

/* Missão */
.missao {
  padding: 80px 20px;
  background: #111;
  color: white;
  text-align: center;
}

.missao h2 {
  margin-bottom: 40px;
  font-size: 2rem;
}

.missao .cards {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: center;
}

.missao .card {
  background: #1f1f1f;
  padding: 30px;
  border-radius: 15px;
  flex: 1;
  min-width: 250px;
  max-width: 300px;
}

/* Projetos */
.projetos {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
  padding: 80px 20px;
  background: #00a886;
  color: white;
}

.projeto img {
  width: 100%;
  border-radius: 15px;
  margin-bottom: 15px;
}

/* Premiações */
.premiacoes {
  padding: 80px 20px;
  background: #00a886;
  color: white;
  text-align: center;
  max-width: 800px;
