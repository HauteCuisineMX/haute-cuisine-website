
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Haute Cuisine Advisors</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Open+Sans&display=swap" rel="stylesheet">

  <!-- Librería de íconos FontAwesome -->
  <script src="https://kit.fontawesome.com/3c4d2d3a5f.js" crossorigin="anonymous"></script>

  <style>
    :root {
      --crema: #fdfcf9;
      --arena: #e0c097;
      --blanco: #ffffff;
      --negro: #111111;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Open Sans', sans-serif;
      background: var(--crema);
      color: var(--negro);
    }

    header {
      background: url('https://images.unsplash.com/photo-1551782450-a2132b4ba21d?fit=crop&w=1600&q=80') center/cover no-repeat;
      color: var(--blanco);
      text-align: center;
      padding: 100px 20px;
      animation: fadeIn 2s ease-in-out;
    }

    header img {
      width: 120px;
      margin-bottom: 20px;
      animation: slideDown 1.5s ease-in-out;
    }

    header h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3em;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.2em;
      color: var(--arena);
      margin-bottom: 20px;
    }

    .btn-contacto {
      background: var(--arena);
      color: var(--negro);
      padding: 12px 25px;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn-contacto:hover {
      background: var(--blanco);
      color: var(--negro);
    }

    section {
      padding: 60px 20px;
      max-width: 1200px;
      margin: auto;
      animation: fadeInUp 1.5s ease-in-out;
    }

    section h2 {
      font-size: 2em;
      margin-bottom: 20px;
      border-left: 6px solid var(--arena);
      padding-left: 10px;
      font-family: 'Playfair Display', serif;
    }

    section p {
      font-size: 1.1em;
      line-height: 1.7;
      margin-bottom: 20px;
    }

    .servicios {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }

    .card {
      flex: 1 1 30%;
      background: var(--blanco);
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .card:hover {
      transform: translateY(-10px);
    }

    .card i {
      font-size: 2.5em;
      color: var(--arena);
      margin-bottom: 15px;
    }

    .casos, .testimonios {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
    }

    .testimonio {
      background: var(--blanco);
      padding: 20px;
      border-left: 4px solid var(--arena);
      border-radius: 5px;
    }

    footer {
      background: var(--negro);
      color: var(--blanco);
      text-align: center;
      padding: 30px;
    }

    footer .social-icons i {
      margin: 0 10px;
      font-size: 1.5em;
      color: var(--arena);
      transition: 0.3s;
    }

    footer .social-icons i:hover {
      color: var(--blanco);
    }

    /* Animaciones */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideDown {
      from { transform: translateY(-50px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
  </style>
</head>
<body>

<!-- HERO -->
<header>
  <img src="logo.png" alt="Logo Haute Cuisine Advisors">
  <h1>Haute Cuisine Advisors</h1>
  <p>Transformamos ideas en experiencias culinarias únicas</p>
  <a href="#contacto" class="btn-contacto">Contáctanos</a>
</header>

<!-- QUIÉNES SOMOS -->
<section>
  <h2>Quiénes Somos</h2>
  <p>Somos una consultora gastronómica integral que impulsa el éxito de negocios de alimentos y bebidas en México. Ofrecemos estrategias innovadoras que combinan creatividad, rentabilidad y excelencia operativa.</p>
</section>

<!-- SERVICIOS -->
<section>
  <h2>Servicios</h2>
  <div class="servicios">
    <div class="card">
      <i class="fas fa-utensils"></i>
      <h3>Creación de Conceptos</h3>
      <p>Desarrollamos conceptos únicos y diferenciadores que conectan con tus clientes.</p>
    </div>
    <div class="card">
      <i class="fas fa-book"></i>
      <h3>Manuales y Capacitación</h3>
      <p>Implementamos procesos y entrenamientos para elevar la calidad del servicio.</p>
    </div>
    <div class="card">
      <i class="fas fa-chart-line"></i>
      <h3>Optimización</h3>
      <p>Escandallos, control de costos y estrategias para maximizar la rentabilidad.</p>
    </div>
  </div>
</section>

<!-- CASOS DE ÉXITO -->
<section>
  <h2>Casos de Éxito</h2>
  <div class="casos">
    <div>
      <h3>Beef Master – Cabo San Lucas</h3>
      <p>Transformamos un negocio familiar de cortes al carbón en un destino culinario de referencia dentro del Container Park, atrayendo tanto locales como turistas.</p>
    </div>
    <div>
      <h3>Luna de Sal – Cocina de Autor Costera</h3>
      <p>Desarrollamos un proyecto integral con menú, capacitación, manuales y estrategia de marketing para un concepto ficticio que demuestra nuestro alcance y profesionalismo.</p>
    </div>
  </div>
</section>

<!-- TESTIMONIOS -->
<section>
  <h2>Testimonios</h2>
  <div class="testimonios">
    <div class="testimonio">
      <p>"Gracias a Haute Cuisine Advisors logramos profesionalizar nuestro restaurante y aumentar nuestras ventas en un 40% en menos de 6 meses."</p>
      <strong>- Cliente Restaurante</strong>
    </div>
    <div class="testimonio">
      <p>"Su equipo entiende la industria gastronómica y sabe cómo convertir ideas en proyectos exitosos."</p>
      <strong>- Socio Empresarial</strong>
    </div>
  </div>
</section>

<!-- CONTACTO -->
<section id="contacto">
  <h2>Contacto</h2>
  <p><i class="fas fa-envelope"></i> haute_cuisine@hotmail.com</p>
  <p><i class="fas fa-phone"></i> +52 624 138 4078</p>
</section>

<!-- FOOTER -->
<footer>
  <p>&copy; 2025 Haute Cuisine Advisors | Todos los derechos reservados</p>
  <div class="social-icons">
    <a href="https://instagram.com/Haute_cuisineMX" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="https://facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
    <a href="https://wa.me/526241384078" target="_blank"><i class="fab fa-whatsapp"></i></a>
  </div>
</footer>

</body>
</html>
