<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Haute Cuisine Advisors</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
<style>
/* Reset y tipografía */
* { margin:0; padding:0; box-sizing:border-box; }
body { font-family: 'Montserrat', sans-serif; line-height:1.6; color:#111; background-color:#fff; scroll-behavior:smooth; overflow-x:hidden; }
a { text-decoration:none; color:inherit; }

/* Contenedores */
.container { width:90%; max-width:1200px; margin:0 auto; }

/* Hero / Inicio con Parallax */
header { height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; background: url('assets/hero.jpg') center/cover no-repeat fixed; text-align:center; position:relative; color:#fff; overflow:hidden; }
header::after { content:""; position:absolute; top:0; left:0; width:100%; height:100%; background:rgba(0,0,0,0.4); }
header img { width:180px; margin-bottom:20px; z-index:1; }
header h1, header p { opacity:0; transform:translateY(50px); }
header h1 { font-size:3rem; z-index:1; animation: fadeInUp 2s forwards; }
header p { font-size:1.3rem; margin-top:1rem; z-index:1; animation: fadeInUp 2.5s forwards; }
.btn-hero { margin-top:2rem; padding:0.8rem 2rem; background:#c2a67a; color:#fff; border:none; border-radius:5px; cursor:pointer; transition:0.3s; z-index:1; position:relative; font-weight:700; opacity:0; transform:translateY(50px); animation: fadeInUp 3s forwards; }
.btn-hero:hover { background:#a68b5a; transform: scale(1.08); }

/* Secciones */
section { padding:100px 0; position:relative; }
section:nth-of-type(even) { background:#f8f4ef; }
section h2 { text-align:center; font-size:2.5rem; margin-bottom:50px; color:#111; position:relative; opacity:0; transform:translateY(50px); }
section h2::after { content:""; width:80px; height:4px; background:#c2a67a; display:block; margin:10px auto 0; border-radius:2px; }

/* Textos */
section p { max-width:800px; margin:0 auto 30px; text-align:center; color:#333; font-size:1.1rem; opacity:0; transform:translateY(50px); }

/* Grid avanzado para servicios y portafolio */
.grid { display:grid; grid-template-columns:repeat(auto-fit, minmax(280px,1fr)); gap:40px; margin-top:50px; }
.card { background:#fff; padding:20px; border-radius:15px; box-shadow:0 8px 20px rgba(0,0,0,0.1); transition:0.5s; overflow:hidden; position:relative; opacity:0; transform: translateY(50px); cursor:pointer; }
.card img { width:100%; border-radius:15px; transition:0.5s; }
.card p { margin-top:15px; text-align:center; font-weight:600; }
.card:hover { transform: translateY(-15px) scale(1.03); box-shadow:0 15px 35px rgba(0,0,0,0.2); }
.card:hover img { transform: scale(1.1); filter: brightness(0.85); }

/* Testimonios estilo revista */
.testimonial { background:#c2a67a; color:#fff; padding:50px 30px; border-radius:15px; margin:20px; text-align:center; font-size:1.1rem; line-height:1.5; font-style:italic; opacity:0; transform: translateY(50px); transition:0.5s; position:relative; cursor:default; }
.testimonial::before { content:"“"; font-size:3rem; position:absolute; left:20px; top:-10px; opacity:0.2; }

/* Contacto */
form { max-width:600px; margin:0 auto; display:flex; flex-direction:column; gap:20px; }
input, textarea { padding:15px; border:1px solid #ccc; border-radius:10px; width:100%; font-size:1rem; transition:0.3s; }
input:focus, textarea:focus { border-color:#c2a67a; outline:none; }
button { padding:0.8rem 2rem; background:#111; color:#fff; border:none; border-radius:10px; cursor:pointer; font-weight:600; transition:0.3s; }
button:hover { background:#333; transform: scale(1.08); }

/* Botón flotante WhatsApp */
.whatsapp { position:fixed; bottom:30px; right:30px; background:#25D366; color:#fff; width:70px; height:70px; border-radius:50%; display:flex; justify-content:center; align-items:center; font-size:32px; box-shadow:0 8px 16px rgba(0,0,0,0.3); z-index:100; cursor:pointer; transition:0.3s; }
.whatsapp:hover { transform:scale(1.2); }

/* Animaciones */
@keyframes fadeIn { from {opacity:0;} to {opacity:1;} }
@keyframes fadeInUp { from {opacity:0; transform:translateY(50px);} to {opacity:1; transform:translateY(0);} }

/* Footer */
footer { text-align:center; padding:40px 0; background:#111; color:#fff; }
footer .socials a { margin:0 15px; color:#fff; font-size:1.8rem; transition:0.3s; }
footer .socials a:hover { color:#c2a67a; }

/* Responsive */
@media(max-width:768px){
    header h1 { font-size:2.2rem; }
    section h2 { font-size:2rem; }
}
</style>
</head>
<body>

<!-- Hero / Inicio -->
<header>
    <img src="assets/logo.png" alt="Logo Haute Cuisine Advisors">
    <h1>Haute Cuisine Advisors</h1>
    <p>Transformamos ideas en experiencias culinarias únicas</p>
    <button class="btn-hero" onclick="window.location.href='#contacto'">Contáctanos</button>
</header>

<!-- Introducción / Sobre Nosotros -->
<section id="sobre">
    <h2>Sobre Nosotros</h2>
    <p>En <strong>Haute Cuisine Advisors</strong> combinamos pasión, creatividad y estrategia para transformar restaurantes y proyectos gastronómicos en experiencias inolvidables. Nuestro enfoque integra innovación, eficiencia operativa y diseño de alta calidad.</p>
    <img src="assets/cocina.jpg" alt="Equipo trabajando en cocina" style="display:block; margin:30px auto; max-width:80%; border-radius:15px;">
</section>

<!-- Misión y Visión -->
<section id="misionvision">
    <h2>Misión y Visión</h2>
    <p><strong>Misión:</strong> Transformar ideas culinarias en experiencias únicas, elevando la calidad, la rentabilidad y la satisfacción del cliente.</p>
    <p><strong>Visión:</strong> Ser la consultoría gastronómica líder en México, reconocida por innovación, profesionalismo y resultados extraordinarios.</p>
</section>

<!-- Importancia Consultoría -->
<section id="importancia">
    <h2>La Importancia de la Consultoría Gastronómica</h2>
    <p>La consultoría gastronómica profesional permite:</p>
    <div class="grid">
        <div class="card"><img src="assets/gestion.jpg" alt="Optimización de Menús"><p>Optimización de Menús: Mejoramos la selección y presentación de tus platillos.</p></div>
        <div class="card"><img src="assets/cocina.jpg" alt="Capacitación de Personal"><p>Capacitación de Personal: Garantizamos servicio de excelencia y consistencia.</p></div>
        <div class="card"><img src="assets/logo.png" alt="Diseño y Branding"><p>Diseño y Branding: Creamos una imagen coherente y atractiva para tus clientes.</p></div>
    </div>
</section>

<!-- Servicios -->
<section id="servicios">
    <h2>Nuestros Servicios</h2>
    <div class="grid">
        <div class="card"><img src="assets/hero.jpg" alt="Consultoría Integral"><p><strong>Consultoría Integral:</strong> Análisis completo del negocio y estrategias personalizadas.</p></div>
        <div class="card"><img src="assets/gestion.jpg" alt="Planificación de Proyectos"><p><strong>Planificación de Proyectos:</strong> Desarrollo de proyectos de apertura y expansión.</p></div>
        <div class="card"><img src="assets/cocina.jpg" alt="Marketing Gastronómico"><p><strong>Marketing Gastronómico:</strong> Estrategias para posicionar tu marca y atraer clientes.</p></div>
    </div>
</section>

<!-- Portafolio -->
<section id="portafolio">
    <h2>Portafolio de Proyectos</h2>
    <div class="grid">
        <div class="card"><img src="assets/cocina.jpg" alt="Proyecto 1"><p>Proyecto Simulado: Diseño completo de restaurante de cocina costera de autor.</p></div>
        <div class="card"><img src="assets/gestion.jpg" alt="Proyecto 2"><p>Optimización de operaciones y menú para un restaurante de cortes.</p></div>
        <div class="card"><img src="assets/hero.jpg" alt="Proyecto 3"><p>Planificación de preapertura y estrategia de marketing.</p></div>
    </div>
</section>

<!-- Testimonios -->
<section id="testimonios">
    <h2>Testimonios</h2>
    <div class="grid">
        <div class="testimonial">"Haute Cuisine Advisors transformó completamente nuestro restaurante, aumentando nuestras ventas y mejorando la experiencia del cliente."</div>
        <div class="testimonial">"La asesoría fue profesional, clara y efectiva. Recomiendo ampliamente sus servicios."</div>
    </div>
</section>

<!-- Contacto -->
<section id="contacto">
    <h2>Contacto</h2>
    <form>
        <input type="text" placeholder="Nombre" required>
        <input type="email" placeholder="Correo" required>
        <textarea placeholder="Mensaje" rows="5" required></textarea>
        <button type="submit">Enviar</button>
    </form>
</section>

<!-- Botón flotante WhatsApp -->
<div class="whatsapp" onclick="window.open('https://wa.me/526241842775','_blank')">💬</div>

<!-- Footer -->
<footer>
    <p>© 2025 Haute Cuisine Advisors</p>
    <div class="socials">
        <a href="https://www.instagram.com/Haute_cuisineMX" target="_blank">📷</a>
        <a href="https://www.facebook.com/HauteCuisineAdvisors" target="_blank">📘</a>
        <a href="mailto:haute.cuicineadv@gmail.com">✉️</a>
    </div>
</footer>

<!-- Animaciones al scroll -->
<script>
const observer = new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
        if(entry.isIntersecting){
            entry.target.style.opacity = 1;
            entry.target.style.transform = 'translateY(0)';
        }
    });
},{threshold:0.1});

document.querySelectorAll('section h2, section p, .card, .testimonial, .btn-hero').forEach(el=>observer.observe(el));
</script>

</body>
</html>
