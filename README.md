<!--
Project: Landing Soluciones
Structure:
  /index.html
  /css/styles.css
  /assets/  (images exported from Figma)
-->

<!-- index.html -->
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Landing Soluciones</title>
  <link rel="stylesheet" href="css/styles.css">
</head>
<body>
  <header class="header container">
    <div class="logo"> <!-- logo export -->
      <img src="assets/logo.svg" alt="Logo Landing Soluciones">
    </div>
    <nav class="nav">
      <ul>
        <li><a href="#features">Características</a></li>
        <li><a href="#testimonials">Testimonios</a></li>
        <li><a href="#contact">Contacto</a></li>
      </ul>
    </nav>
    <a href="#contact" class="btn-primary">Contáctanos</a>
  </header>

  <section id="hero" class="hero">
    <div class="hero-content container">
      <h1>Título Principal de la Landing</h1>
      <p>Descripción breve que invite a la acción.</p>
      <a href="#contact" class="btn-secondary">Empieza Ahora</a>
    </div>
    <div class="hero-image">
      <img src="assets/hero-image.png" alt="Imagen Hero">
    </div>
  </section>

  <section id="features" class="features container">
    <h2>¿Qué ofrecemos?</h2>
    <div class="feature-grid">
      <div class="feature-item">
        <img src="assets/feature1.svg" alt="Feature 1">
        <h3>Funcionalidad 1</h3>
        <p>Descripción breve de la funcionalidad.</p>
      </div>
      <div class="feature-item">
        <img src="assets/feature2.svg" alt="Feature 2">
        <h3>Funcionalidad 2</h3>
        <p>Descripción breve de la funcionalidad.</p>
      </div>
      <div class="feature-item">
        <img src="assets/feature3.svg" alt="Feature 3">
        <h3>Funcionalidad 3</h3>
        <p>Descripción breve de la funcionalidad.</p>
      </div>
    </div>
  </section>

  <section id="testimonials" class="testimonials container">
    <h2>Testimonios</h2>
    <div class="testimonial-slider">
      <div class="testimonial-item">
        <p>“Excelente servicio y soporte.”</p>
        <h4>Juan Pérez, CEO de Empresa X</h4>
      </div>
      <div class="testimonial-item">
        <p>“Nuestra productividad se incrementó un 50%.”</p>
        <h4>María López, CTO de Empresa Y</h4>
      </div>
    </div>
  </section>

  <section id="contact" class="contact container">
    <h2>Contáctanos</h2>
    <form action="#" method="POST" class="contact-form">
      <label for="name">Nombre</label>
      <input type="text" id="name" name="name" required>
      <label for="email">Email</label>
      <input type="email" id="email" name="email" required>
      <label for="message">Mensaje</label>
      <textarea id="message" name="message" rows="4" required></textarea>
      <button type="submit" class="btn-primary">Enviar</button>
    </form>
  </section>

  <footer class="footer container">
    <p>&copy; 2025 Landing Soluciones. Todos los derechos reservados.</p>
    <ul class="social-links">
      <li><a href="#">Facebook</a></li>
      <li><a href="#">Twitter</a></li>
      <li><a href="#">LinkedIn</a></li>
    </ul>
  </footer>

</body>
</html>

<!-- css/styles.css -->
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');

/* Variables */
:root {
  --primary-color: #0052cc;
  --secondary-color: #edf2f7;
  --text-color: #333;
  --bg-color: #fff;
  --radius: 8px;
}

/* Reset & base */n* { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: 'Inter', sans-serif; color: var(--text-color); background: var(--bg-color); line-height: 1.6; }
.container { width: 90%; max-width: 1200px; margin: 0 auto; }

/* Buttons */
.btn-primary { display: inline-block; background: var(--primary-color); color: #fff; padding: 0.75rem 1.5rem; border-radius: var(--radius); text-decoration: none; font-weight: 600; }
.btn-secondary { display: inline-block; background: transparent; border: 2px solid var(--primary-color); color: var(--primary-color); padding: 0.75rem 1.5rem; border-radius: var(--radius); text-decoration: none; font-weight: 600; }

/* Header */
.header { display: flex; align-items: center; justify-content: space-between; padding: 1rem 0; }
.nav ul { list-style: none; display: flex; gap: 1.5rem; }
.nav a { color: var(--text-color); text-decoration: none; font-weight: 600; }

/* Hero */
.hero { display: flex; align-items: center; justify-content: space-between; padding: 4rem 0; }
.hero-content { max-width: 50%; }
.hero-image img { max-width: 100%; }

/* Features */
.features { padding: 4rem 0; text-align: center; }
.feature-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 2rem; margin-top: 2rem; }
.feature-item img { width: 60px; margin-bottom: 1rem; }

/* Testimonials */
.testimonials { background: var(--secondary-color); padding: 4rem 0; text-align: center; }
.testimonial-slider { display: flex; overflow-x: auto; gap: 2rem; }
.testimonial-item { flex: 0 0 300px; background: #fff; padding: 1.5rem; border-radius: var(--radius); box-shadow: 0 2px 4px rgba(0,0,0,0.1); }

/* Contact */
.contact { padding: 4rem 0; }
.contact-form { display: grid; gap: 1rem; }
.contact-form input,
.contact-form textarea { padding: 0.75rem; border: 1px solid #ccc; border-radius: var(--radius); width: 100%; }

/* Footer */
.footer { padding: 2rem 0; text-align: center; font-size: 0.9rem; }
.social-links { list-style: none; display: flex; justify-content: center; gap: 1rem; margin-top: 1rem; }
.social-links a { text-decoration: none; color: var(--text-color); }
