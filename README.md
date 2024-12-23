<html><head><base href="https://example.com">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DigiSocial Marketing | Marketing Digital &amp; Gest&#xe3;o de Redes Sociais</title>
<style>
:root {
  --primary: #FF3366;
  --secondary: #6C63FF;
  --dark: #2A2A2A;
  --light: #FFFFFF;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  overflow-x: hidden;
}

.navbar {
  padding: 20px 50px;
  background: var(--light);
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  position: fixed;
  width: 100%;
  z-index: 1000;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navbar .logo {
  color: var(--primary);
  font-size: 24px;
  font-weight: 700;
  text-decoration: none;
}

.nav-links {
  display: flex;
  gap: 30px;
}

.nav-links a {
  color: var(--dark);
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
  position: relative;
}

.nav-links a::after {
  content: '';
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--primary);
  transition: width 0.3s ease;
}

.nav-links a:hover::after {
  width: 100%;
}

.nav-links a:hover {
  color: var(--primary);
}

.hero {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(45deg, var(--primary), var(--secondary));
  padding: 0 50px;
}

.hero-content {
  text-align: center;
  color: var(--light);
}

.hero h1 {
  font-size: 48px;
  margin-bottom: 20px;
  animation: fadeInUp 1s ease;
}

.hero p {
  font-size: 20px;
  margin-bottom: 30px;
  animation: fadeInUp 1s ease 0.3s;
}

.cta-button {
  padding: 15px 30px;
  background: var(--light);
  color: var(--primary);
  text-decoration: none;
  border-radius: 30px;
  font-weight: 600;
  transition: transform 0.3s ease;
  display: inline-block;
  animation: fadeInUp 1s ease 0.6s;
}

.cta-button:hover {
  transform: translateY(-5px);
}

.services {
  padding: 100px 50px;
  background: var(--light);
}

.services h2 {
  text-align: center;
  color: var(--dark);
  margin-bottom: 50px;
}

.service-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
}

.service-card {
  padding: 30px;
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.service-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(45deg, var(--primary), var(--secondary));
  opacity: 0;
  transition: opacity 0.3s ease;
  z-index: 0;
}

.service-card:hover::before {
  opacity: 0.1;
}

.service-card:hover {
  transform: translateY(-10px);
}

.service-card svg {
  width: 50px;
  height: 50px;
  margin-bottom: 20px;
  fill: var(--primary);
}

.service-card h3 {
  color: var(--dark);
  margin-bottom: 15px;
}

.service-card p {
  color: #666;
  line-height: 1.6;
}

.testimonials {
  padding: 100px 50px;
  background: #f9f9f9;
}

.testimonials h2 {
  text-align: center;
  color: var(--dark);
  margin-bottom: 50px;
}

.testimonial-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin-bottom: 50px;
}

.testimonial-card {
  display: grid;
  grid-template-columns: 100px 1fr;
  gap: 20px;
  align-items: center;
  background: var(--light);
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  cursor: pointer;
  transition: all 0.3s ease;
}

.testimonial-image {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  overflow: hidden;
  position: relative;
}

.testimonial-content {
  text-align: left;
}

.client-name {
  font-weight: bold;
  color: var(--dark);
}

.client-company {
  color: var(--primary);
  font-size: 0.9em;
  margin-top: 5px;
}

.testimonial-rating {
  color: #FFD700;
  font-size: 20px;
  margin: 10px 0;
}

.stats {
  padding: 50px;
  background: var(--primary);
  color: var(--light);
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 30px;
  text-align: center;
}

.stat-item {
  cursor: pointer;
  transition: transform 0.3s ease;
}

.stat-item:hover {
  transform: scale(1.1);
}

.stat-item h3 {
  font-size: 40px;
  margin-bottom: 10px;
}

.contact {
  padding: 100px 50px;
  background: var(--light);
}

.contact h2 {
  text-align: center;
  color: var(--dark);
  margin-bottom: 50px;
}

.contact-form {
  max-width: 600px;
  margin: 0 auto;
}

.form-group {
  margin-bottom: 20px;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 15px;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 16px;
}

.form-group textarea {
  height: 150px;
  resize: vertical;
}

.submit-btn {
  background: var(--primary);
  color: var(--light);
  padding: 15px 30px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  font-size: 16px;
  font-weight: 600;
  transition: transform 0.3s ease;
}

.submit-btn:hover {
  transform: translateY(-3px);
}

footer {
  background: var(--dark);
  color: var(--light);
  padding: 50px;
  text-align: center;
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin-bottom: 30px;
}

.social-links a {
  color: var(--light);
  font-size: 24px;
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: var(--primary);
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@media (max-width: 768px) {
  .navbar {
    padding: 20px;
  }
  
  .nav-links {
    display: none;
  }
  
  .hero h1 {
    font-size: 36px;
  }
  
  .hero p {
    font-size: 18px;
  }
  
  .services {
    padding: 50px 20px;
  }
}

.service-modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.8);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1000;
  opacity: 0;
  animation: fadeIn 0.3s ease forwards;
}

.modal-content {
  background: white;
  padding: 40px;
  border-radius: 15px;
  max-width: 500px;
  width: 90%;
  position: relative;
  transform: translateY(20px);
  animation: slideUp 0.3s ease forwards;
}

.modal-content h3 {
  color: var(--primary);
  margin-bottom: 20px;
}

.modal-content h4 {
  color: var(--dark);
  margin-bottom: 15px;
}

.modal-content ul {
  list-style: none;
  margin-bottom: 20px;
}

.modal-content li {
  padding: 10px 0;
  border-bottom: 1px solid #eee;
  color: #666;
}

.modal-content li:before {
  content: "✓";
  color: var(--primary);
  margin-right: 10px;
}

.price {
  font-size: 1.2em;
  color: var(--primary);
  font-weight: bold;
  margin: 20px 0;
}

.close-modal {
  background: var(--primary);
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 25px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.close-modal:hover {
  transform: translateY(-2px);
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideUp {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.domain-suggestion {
  background: linear-gradient(45deg, var(--primary), var(--secondary));
  color: white;
  padding: 15px 30px;
  border-radius: 8px;
  margin: 30px auto;
  max-width: 600px;
  text-align: center;
}

.domain-suggestion p {
  font-size: 1.2em;
  margin-bottom: 10px;
}

.domain-name {
  font-size: 1.5em;
  font-weight: bold;
  color: #fff;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
}
</style>
</head>
<body>
  <nav class="navbar">
    <a href="https://example.com" class="logo">DigiSocial Marketing</a>
    <div class="nav-links">
      <a href="https://example.com/servicos">Servi&#xe7;os</a>
      <a href="https://example.com/portfolio">Portf&#xf3;lio</a>
      <a href="https://example.com/sobre">Sobre</a>
      <a href="https://example.com/contato">Contato</a>
    </div>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Transforme sua Presen&#xe7;a Digital</h1>
      <p>Gest&#xe3;o profissional de redes sociais para impulsionar seu neg&#xf3;cio</p>
      <a href="https://example.com/contato" class="cta-button">Comece Agora</a>
    </div>
  </section>

  <section class="services">
    <h2>Nossos Servi&#xe7;os</h2>
    <div class="service-grid">
      <div class="service-card" data-service="instagram">
        <svg viewBox="0 0 24 24">
          <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
        </svg>
        <h3>Gest&#xe3;o de Instagram</h3>
        <p>Cria&#xe7;&#xe3;o de conte&#xfa;do estrat&#xe9;gico, design de posts, stories e reels para engajar seu p&#xfa;blico.</p>
      </div>

      <div class="service-card" data-service="content">
        <svg viewBox="0 0 24 24">
          <path d="M20 2H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h14l4 4V4c0-1.1-.9-2-2-2zm-2 12H6v-2h12v2zm0-3H6V9h12v2zm0-3H6V6h12v2z"/>
        </svg>
        <h3>Marketing de Conte&#xfa;do</h3>
        <p>Desenvolvimento de estrat&#xe9;gias de conte&#xfa;do alinhadas com seus objetivos de neg&#xf3;cio.</p>
      </div>

      <div class="service-card" data-service="analytics">
        <svg viewBox="0 0 24 24">
          <path d="M16 6l2.29 2.29-4.88 4.88-4-4L2 16.59 3.41 18l6-6 4 4 6.3-6.29L22 12V6z"/>
        </svg>
        <h3>An&#xe1;lise de M&#xe9;tricas</h3>
        <p>Monitoramento e an&#xe1;lise de resultados para otimizar sua estrat&#xe9;gia digital.</p>
      </div>
    </div>
  </section>

  <section class="testimonials">
    <h2>O Que Nossos Clientes Dizem</h2>
    <div class="testimonial-grid">
      <div class="testimonial-card">
        <div class="testimonial-image">
          <svg viewBox="0 0 24 24" style="width: 100%; height: 100%; fill: var(--primary);">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 3c1.66 0 3 1.34 3 3s-1.34 3-3 3-3-1.34-3-3 1.34-3 3-3z M12 20.5c-2.33 0-4.32-1.45-5.12-3.5h10.24c-.8 2.05-2.79 3.5-5.12 3.5z"/>
          </svg>
        </div>
        <div class="testimonial-content">
          <div class="testimonial-rating">★★★★★</div>
          <p>"A DigiSocial revolucionou nossa presença online! Em apenas 3 meses, nosso engajamento cresceu 300% e as vendas pelo Instagram aumentaram significativamente."</p>
          <div class="client-name">Maria Silva</div>
          <div class="client-company">Boutique Elegance - @boutiqueelegance</div>
        </div>
      </div>
      
      <div class="testimonial-card">
        <div class="testimonial-image">
          <svg viewBox="0 0 24 24" style="width: 100%; height: 100%; fill: var(--primary);">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 3c1.66 0 3 1.34 3 3s-1.34 3-3 3-3-1.34-3-3 1.34-3 3-3z M12 20.5c-2.33 0-4.32-1.45-5.12-3.5h10.24c-.8 2.05-2.79 3.5-5.12 3.5z"/>
          </svg>
        </div>
        <div class="testimonial-content">
          <div class="testimonial-rating">★★★★★</div>
          <p>"Equipe extremamente profissional e criativa. Nossa presença digital mudou completamente e os resultados são impressionantes!"</p>
          <div class="client-name">João Santos</div>
          <div class="client-company">Tech Solutions - @techsolutionsbr</div>
        </div>
      </div>

      <div class="testimonial-card">
        <div class="testimonial-image">
          <svg viewBox="0 0 24 24" style="width: 100%; height: 100%; fill: var(--primary);">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 3c1.66 0 3 1.34 3 3s-1.34 3-3 3-3-1.34-3-3 1.34-3 3-3z M12 20.5c-2.33 0-4.32-1.45-5.12-3.5h10.24c-.8 2.05-2.79 3.5-5.12 3.5z"/>
          </svg>
        </div>
        <div class="testimonial-content">
          <div class="testimonial-rating">★★★★★</div>
          <p>"Nosso ROI em marketing digital triplicou desde que começamos a trabalhar com a DigiSocial. Eles realmente entendem o que funciona!"</p>
          <div class="client-name">Ana Oliveira</div>
          <div class="client-company">Café & Cia - @cafeciabrasil</div>
        </div>
      </div>
    </div>

    <div class="domain-suggestion">
      <p>Visite nosso site:</p>
      <div class="domain-name">www.digisocial.com.br</div>
      <p>Siga-nos no Instagram: @digisocial.br</p>
    </div>
  </section>

  <section class="stats">
    <div class="stats-grid">
      <div class="stat-item">
        <h3>0</h3>
        <p>Clientes Satisfeitos</p>
      </div>
      <div class="stat-item">
        <h3>0</h3>
        <p>Seguidores Alcan&#xe7;ados</p>
      </div>
      <div class="stat-item">
        <h3>0</h3>
        <p>Posts Criados</p>
      </div>
      <div class="stat-item">
        <h3>0</h3>
        <p>Taxa de Reten&#xe7;&#xe3;o</p>
      </div>
    </div>
  </section>

  <section class="contact">
    <h2>Entre em Contato</h2>
    <form class="contact-form">
      <div class="form-group">
        <input type="text" placeholder="Nome" required>
      </div>
      <div class="form-group">
        <input type="email" placeholder="Email" required>
      </div>
      <div class="form-group">
        <textarea placeholder="Sua mensagem" required></textarea>
      </div>
      <button type="submit" class="submit-btn">Enviar Mensagem</button>
    </form>
  </section>

  <footer>
    <div class="social-links">
      <a href="https://instagram.com/digisocial"><svg viewBox="0 0 24 24" width="24" height="24" style="fill: currentColor;">
        <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
      </svg></a>
    </div>
    <p>&#xa9; 2024 DigiSocial Marketing. Todos os direitos reservados.</p>
  </footer>

  <script>document.addEventListener('DOMContentLoaded', function () {
  const observerOptions = {
    threshold: 0.1
  };
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.opacity = '1';
        entry.target.style.transform = 'translateY(0)';
      }
    });
  }, observerOptions);
  document.querySelectorAll('.service-card').forEach(card => {
    card.style.opacity = '0';
    card.style.transform = 'translateY(30px)';
    card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
    observer.observe(card);
  });
  let animated = false;
  window.addEventListener('scroll', () => {
    if (!animated) {
      const statsSection = document.querySelector('.stats');
      if (isElementInViewport(statsSection)) {
        animated = true;
        const statElements = {
          clients: {
            el: document.querySelector('.stat-item:nth-child(1) h3'),
            end: 500
          },
          followers: {
            el: document.querySelector('.stat-item:nth-child(2) h3'),
            end: 1000000
          },
          posts: {
            el: document.querySelector('.stat-item:nth-child(3) h3'),
            end: 5000
          },
          retention: {
            el: document.querySelector('.stat-item:nth-child(4) h3'),
            end: 98
          }
        };
        Object.values(statElements).forEach(({
          el,
          end
        }) => {
          animateValue(el, 0, end, 2000);
        });
      }
    }
  });
  document.querySelectorAll('.service-card').forEach(card => {
    card.addEventListener('mousemove', e => {
      const rect = card.getBoundingClientRect();
      const x = e.clientX - rect.left;
      const y = e.clientY - rect.top;
      card.style.transform = `
        perspective(1000px) 
        rotateX(${(y - rect.height / 2) / 20}deg) 
        rotateY(${-(x - rect.width / 2) / 20}deg)
      `;
    });
    card.addEventListener('mouseleave', () => {
      card.style.transform = 'perspective(1000px) rotateX(0) rotateY(0)';
    });
  });
  const form = document.querySelector('.contact-form');
  form.addEventListener('submit', e => {
    e.preventDefault();
    const button = form.querySelector('.submit-btn');
    button.innerHTML = 'Enviando...';
    button.disabled = true;
    setTimeout(() => {
      button.innerHTML = 'Mensagem Enviada!';
      button.style.background = '#4CAF50';
      form.reset();
      setTimeout(() => {
        button.innerHTML = 'Enviar Mensagem';
        button.style.background = '';
        button.disabled = false;
      }, 2000);
    }, 1500);
  });

  function expandServiceDetails(serviceCard) {
    const serviceDetails = {
      'instagram': {
        title: 'Gestão de Instagram',
        examples: [
          'Stories diários com conteúdo exclusivo',
          'Posts estratégicos 5x por semana',
          'Reels semanais para aumentar alcance',
          'Gestão de comentários e DMs',
          'Relatórios mensais de desempenho'
        ],
        price: 'A partir de R$997/mês'
      },
      'content': {
        title: 'Marketing de Conteúdo',
        examples: [
          'Planejamento editorial mensal',
          'Copywriting especializado',
          'Calendário de postagens',
          'Pesquisa de palavras-chave',
          'Análise de concorrência'
        ],
        price: 'A partir de R$1297/mês'
      },
      'analytics': {
        title: 'Análise de Métricas',
        examples: [
          'Relatórios semanais de performance',
          'Análise de engajamento',
          'Métricas de crescimento',
          'ROI de campanhas',
          'Insights estratégicos'
        ],
        price: 'A partir de R$797/mês'
      }
    };

    const serviceType = serviceCard.getAttribute('data-service');
    const details = serviceDetails[serviceType];

    const modal = document.createElement('div');
    modal.className = 'service-modal';
    modal.innerHTML = `
      <div class="modal-content">
        <h3>${details.title}</h3>
        <h4>Inclui:</h4>
        <ul>
          ${details.examples.map(example => `<li>${example}</li>`).join('')}
        </ul>
        <p class="price">${details.price}</p>
        <button class="close-modal">Fechar</button>
      </div>
    `;

    document.body.appendChild(modal);

    modal.querySelector('.close-modal').onclick = () => {
      modal.remove();
    };

    modal.onclick = (e) => {
      if (e.target === modal) {
        modal.remove();
      }
    };
  }

  document.querySelectorAll('.service-card').forEach(card => {
    card.style.cursor = 'pointer';
    card.onclick = () => expandServiceDetails(card);
  });

  document.querySelectorAll('.testimonial-card').forEach(card => {
    card.addEventListener('mouseenter', () => {
      card.style.transform = 'scale(1.02)';
      card.style.transition = 'transform 0.3s ease';
    });
    
    card.addEventListener('mouseleave', () => {
      card.style.transform = 'scale(1)';
    });
  });

  function isElementInViewport(element) {
    const rect = element.getBoundingClientRect();
    return rect.top >= 0 && rect.left >= 0 && rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) && rect.right <= (window.innerWidth || document.documentElement.clientWidth);
  }

  function animateValue(obj, start, end, duration) {
    let startTimestamp = null;
    const step = timestamp => {
      if (!startTimestamp) startTimestamp = timestamp;
      const progress = (timestamp - startTimestamp) / duration;
      obj.innerHTML = Math.floor(progress * (end - start) + start);
      if (progress < 1) {
        window.requestAnimationFrame(step);
      }
    };
    window.requestAnimationFrame(step);
  }
});
</script>
</body>
</html>
