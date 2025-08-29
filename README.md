<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Haute Cuisine Advisors</title>
  <meta name="description" content="Transformamos ideas en experiencias culinarias únicas. Consultoría gastronómica profesional para restaurantes, hoteles, bares y más.">
  <link rel="icon" href="assets/favicon.png" type="image/png">

  <!-- Fuentes y estilos -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">

  <!-- Iconos -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
  <!-- HEADER -->
  <header class="hero">
    <nav>
      <img src="logo.png" alt="Logo Haute Cuisine Advisors" class="logo">
      <ul>
        <li><a href="#nosotros">Nosotros</a></li>
        <li><a href="#servicios">Servicios</a></li>
        <li><a href="#clientes">Clientes</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
    <div class="hero-text">
      <h1>Haute Cuisine Advisors</h1>
      <p>Transformamos ideas en experiencias culinarias únicas</p>
      <a href="#contacto" class="btn">Agenda tu asesoría</a>
    </div>
  </header>

  <!-- NOSOTROS -->
  <section id="nosotros" class="section">
    <h2>¿Quiénes somos?</h2>
    <p>Somos una consultora gastronómica especializada en transformar conceptos culinarios en negocios exitosos. Con experiencia en restaurantes, bares, hoteles y proyectos gastronómicos, ayudamos a nuestros clientes a crecer, innovar y destacar.</p>
  </section>

  <!-- SERVICIOS -->
  <section id="servicios" class="section bg-light">
    <h2>Servicios</h2>
    <div class="services">
      <div class="card">
        <i class="fa-solid fa-utensils"></i>
        <h3>Consultoría de Restaurantes</h3>
        <p>Desde la creación de menús hasta la optimización de costos y operación diaria.</p>
      </div>
      <div class="card">
        <i class="fa-solid fa-clipboard-list"></i>
        <h3>Capacitación</h3>
        <p>Entrenamiento profesional de equipos en servicio, cocina y hospitalidad.</p>
      </div>
      <div class="card">
        <i class="fa-solid fa-lightbulb"></i>
        <h3>Conceptualización</h3>
        <p>Desarrollamos ideas innovadoras y memorables para negocios gastronómicos.</p>
      </div>
    </div>
  </section>

  <!-- CLIENTES / ÉXITOS -->
  <section id="clientes" class="section">
    <h2>Historias de Éxito</h2>
    <div class="testimonials">
      <blockquote>
        “Gracias a Haute Cuisine Advisors, logramos relanzar nuestro restaurante Beef Master y duplicar la asistencia en menos de 3 meses.”  
        <span>- Cliente: Beef Master, Cabo San Lucas</span>
      </blockquote>
      <blockquote>
        “Su visión nos ayudó a crear un concepto único para nuestro hotel boutique. ¡Los recomendaríamos una y mil veces!”  
        <span>- Hotel Boutique</span>
      </blockquote>
    </div>
  </section>

  <!-- CONTACTO -->
  <section id="contacto" class="section bg-light">
    <h2>Contáctanos</h2>
    <form class="contact-form">
      <input type="text" placeholder="Tu Nombre" required>
      <input type="email" placeholder="Tu Correo" required>
      <textarea placeholder="Tu Mensaje" required></textarea>
      <button type="submit" class="btn">Enviar</button>
    </form>
    <div class="socials">
      <a href="https://www.facebook.com/Haute_cuisineMX" target="_blank"><i class="fab fa-facebook"></i></a>
      <a href="https://www.instagram.com/Haute_cuisineMX" target="_blank"><i class="fab fa-instagram"></i></a>
      <a href="mailto:haute_cuisine@hotmail.com"><i class="fa-solid fa-envelope"></i></a>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>© 2025 Haute Cuisine Advisors | Todos los derechos reservados</p>
  </footer>

  <!-- BOTÓN WHATSAPP -->
  <a href="https://wa.me/526241384078?text=Hola%20Haute%20Cuisine%20Advisors%2C%20me%20gustaría%20más%20información%20sobre%20sus%20servicios." 
     class="whatsapp-float" target="_blank">
     <i class="fab fa-whatsapp"></i>
  </a>

</body>
</html>

/* Fuentes y estilos globales */
body {
  font-family: 'Open Sans', sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.6;
  color: #333;
}

h1, h2, h3 {
  font-family: 'Playfair Display', serif;
}

a {
  text-decoration: none;
  color: inherit;
}

/* HEADER */
.hero {
  background: url('assets/hero.jpg') center/cover no-repeat;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  color: white;
  text-align: center;
}

.hero nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}

.hero nav ul {
  list-style: none;
  display: flex;
  gap: 20px;
}

.hero nav a {
  color: white;
  font-weight: 600;
}

.hero-text {
  margin-bottom: 100px;
}

.hero-text h1 {
  font-size: 3rem;
  animation: fadeInDown 1.5s ease;
}

.hero-text p {
  font-size: 1.2rem;
  margin: 20px 0;
  animation: fadeInUp 2s ease;
}

.btn {
  background: #000;
  color: #fff;
  padding: 12px 25px;
  border-radius: 5px;
  transition: 0.3s;
}

.btn:hover {
  background: #333;
}

/* SECCIONES */
.section {
  padding: 80px 20px;
  text-align: center;
}

.bg-light {
  background: #f9f9f9;
}

.services {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.card {
  background: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  flex: 1 1 300px;
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-10px);
}

.card i {
  font-size: 2rem;
  color: #b59f5b;
  margin-bottom: 10px;
}

/* TESTIMONIOS */
.testimonials {
  display: grid;
  gap: 20px;
  max-width: 800px;
  margin: auto;
}

blockquote {
  background: #fff;
  padding: 20px;
  border-left: 5px solid #b59f5b;
  font-style: italic;
  border-radius: 5px;
}

/* CONTACTO */
.contact-form {
  display: flex;
  flex-direction: column;
  gap: 15px;
  max-width: 600px;
  margin: auto;
}

.contact-form input,
.contact-form textarea {
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.socials {
  margin-top: 20px;
}

.socials a {
  margin: 0 10px;
  font-size: 1.5rem;
  color: #333;
  transition: 0.3s;
}

.socials a:hover {
  color: #b59f5b;
}

/* FOOTER */
footer {
  background: #000;
  color: #fff;
  text-align: center;
  padding: 15px;
}

/* WHATSAPP FLOAT */
.whatsapp-float {
  position: fixed;
  width: 60px;
  height: 60px;
  bottom: 20px;
  right: 20px;
  background-color: #25d366;
  color: #fff;
  border-radius: 50%;
  text-align: center;
  font-size: 30px;
  box-shadow: 2px 2px 5px #999;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: center;
}

.whatsapp-float:hover {
  background-color: #20b857;
}

/* ANIMACIONES */
@keyframes fadeInDown {
  from { opacity: 0; transform: translateY(-50px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(50px); }
  to { opacity: 1; transform: translateY(0); }
}
