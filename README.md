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
      <ul>
        <li><a href="#home">🏠 Home</a></li>
        <li><a href="#projetos">📍 Projetos</a></li>
        <li><a href="#contato">✉️ Contato</a></li>
      </ul>
    </nav>
  </aside>

  <!-- Hero -->
  <section id="home" class="hero">
    <div class="perfil">
      <img src="sua-foto.jpg" alt="Rodrigo Bina">
    </div>
    <div class="intro">
      <h1>Olá, sou o<br><span>Rodrigo Bina</span><br>Designer Multimídia</h1>
      <a href="#contato" class="btn">Solicitar Orçamento</a>
      <div class="socials">
        <a href="#">Instagram</a>
        <a href="#">LinkedIn</a>
      </div>
    </div>
  </section>

  <!-- Missão -->
  <section id="missao" class="missao">
    <h2>Nossa missão</h2>
    <div class="cards">
      <div class="card">
        <h3>Design com resultado</h3>
        <p>Crio soluções visuais pensadas para atrair atenção, gerar desejo e mover seu público à ação.</p>
      </div>
      <div class="card">
        <h3>Nosso Propósito Central</h3>
        <p>Elevar a experiência digital através de design estratégico que destaca sua marca.</p>
      </div>
      <div class="card">
        <h3>Acompanhamento estratégico</h3>
        <p>Trabalho lado a lado com você para ajustar e evoluir o design conforme o mercado.</p>
      </div>
    </div>
  </section>

  <!-- Projetos -->
  <section id="projetos" class="projetos">
    <div class="projeto">
      <img src="projeto1.jpg" alt="">
      <p>Implementação de soluções de cibersegurança para uma rede social.</p>
    </div>
    <div class="projeto">
      <img src="projeto2.jpg" alt="">
      <p>1º aplicativo de recarga para carros elétricos.</p>
    </div>
    <div class="projeto">
      <img src="projeto3.jpg" alt="">
      <p>Desenvolvimento de uma plataforma de vendas online para moda ESG.</p>
    </div>
  </section>

  <!-- Premiações -->
  <section class="premiacoes">
    <h2>Premiações</h2>
    <p>Sou Rodrigo Bina, designer multimídia apaixonado por criar experiências visuais que conectam pessoas e marcas...</p>
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

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f5f5f5;
  color: #333;
}

/* Sidebar */
.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 80px;
  height: 100%;
  background: #1d1d1d;
  color: #fff;
  padding: 20px;
}

.sidebar .logo {
  font-size: 2rem;
  text-align: center;
  margin-bottom: 20px;
}

.sidebar nav ul {
  list-style: none;
  padding: 0;
}

.sidebar nav ul li {
  margin: 20px 0;
}

.sidebar nav ul li a {
  color: white;
  text-decoration: none;
}

/* Hero */
.hero {
  margin-left: 100px;
  height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #19d3a0, #0a9b8d);
  color: white;
  text-align: center;
}

.hero img {
  border-radius: 20px;
  max-width: 250px;
}

.hero h1 span {
  color: #fff;
  font-weight: bold;
}

.btn {
  display: inline-block;
  margin-top: 15px;
  padding: 10px 20px;
  border-radius: 25px;
  background: white;
  color: #000;
  text-decoration: none;
}

/* Missão */
.missao {
  padding: 50px;
  background: #1d1d1d;
  color: white;
  text-align: center;
}

.missao .cards {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-top: 30px;
}

.missao .card {
  background: #2a2a2a;
  padding: 20px;
  border-radius: 15px;
  width: 30%;
}

/* Projetos */
.projetos {
  display: flex;
  justify-content: center;
  gap: 20px;
  padding: 50px;
  background: #00a886;
}

.projeto img {
  width: 100%;
  border-radius: 15px;
}

/* Premiações */
.premiacoes {
  padding: 50px;
  background: #00a886;
  color: white;
  text-align: left;
  max-width: 700px;
  margin: auto;
}

/* Contato */
.contato {
  padding: 50px;
  text-align: center;
  background: #00a886;
}

footer {
  background: #f0f0f0;
  padding: 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
