# -Aislando-Futuro-
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Aislando Futuro - Lana Sustentable y Capacitación Técnica</title>
<style>
  body {
    margin: 0;
    padding: 0;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    background-color: #f0f4f7;
    color: #243016;
    line-height: 1.7;
  }
  a {
    color: #3a6b20;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  a:hover {
    color: #537d31;
    text-decoration: underline;
  }

  header {
    background: linear-gradient(90deg, #517d30 0%, #2b4f14 100%);
    color: #fefefe;
    text-align: center;
    padding: 80px 20px 60px;
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
  }
  header h1 {
    font-size: 4rem;
    margin-bottom: 0.3em;
    font-weight: 900;
    letter-spacing: 2px;
  }
  header p {
    font-size: 1.3rem;
    font-style: italic;
    margin: 0;
    font-weight: 600;
  }

  nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    background-color: #3a6b20;
    padding: 15px;
    gap: 20px;
    font-weight: 700;
    font-size: 1.1em;
    box-shadow: inset 0 -3px 6px rgba(0,0,0,0.2);
  }
  nav a {
    padding: 10px 15px;
    border-radius: 8px;
    color: #d7e3bf;
  }
  nav a.active, nav a:hover {
    background-color: #537d31;
    color: #fff;
  }

  main {
    max-width: 1200px;
    margin: 50px auto;
    padding: 50px 60px;
    background-color: #fffefb;
    border-radius: 15px;
    box-shadow: 0 8px 25px rgba(34, 68, 21, 0.3);
  }

  section {
    margin-bottom: 80px;
  }
  h2 {
    font-size: 3rem;
    border-bottom: 6px solid #52751a;
    padding-bottom: 15px;
    margin-bottom: 40px;
    color: #38501d;
    font-weight: 900;
  }
  h3 {
    font-size: 2rem;
    margin-bottom: 15px;
    color: #33641f;
  }
  p {
    font-size: 1.2em;
    margin-bottom: 20px;
  }
  /* Imágenes y contenido*/
  .content-img {
    max-width: 100%;
    border-radius: 15px;
    box-shadow: 0 5px 20px rgba(27, 87, 31, 0.3);
    margin-bottom: 20px;
  }
  /* Sección sobre nosotros */
  #sobre-nosotros p {
    max-width: 900px;
    margin: 0 auto 25px;
  }

  /* Beneficios y ventajas */
  ul.beneficios {
    list-style: none;
    columns: 2;
    column-gap: 40px;
    padding: 0;
  }
  ul.beneficios li {
    background-color: #d9f3c9;
    margin-bottom: 18px;
    padding: 12px 15px;
    border-left: 7px solid #569e2b;
    border-radius: 10px;
    font-weight: 600;
    font-size: 1.1em;
  }

  /* Cursos y explicaciones detalladas */
  #cursos {
    padding: 20px;
  }
  #cursos-item {
    font-size: 1.15em;
    background-color: #eaf4d8;
    margin-bottom: 30px;
    padding: 20px;
    border-radius: 15px;
    box-shadow: 0 4px 15px rgba(93, 158, 43, 0.2);
  }
  #cursos-item h4 {
    margin-top: 0;
    color: #417829;
  }
  #cursos-item p {
    margin-top: 10px;
  }

  /* Equipo de trabajo */
  #equipo {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 50px;
    margin-top: 40px;
  }
  .equipo-miembro {
    max-width: 280px;
    background-color: #e0f7e4;
    padding: 20px;
    border-radius: 15px;
    box-shadow: 0 4px 14px rgba(34, 78, 23, 0.2);
    text-align: center;
  }
  .equipo-miembro img {
    width: 100%;
    border-radius: 12px;
    margin-bottom: 15px;
  }
  .equipo-miembro h3 {
    margin-top: 0;
    color: #3a6b20;
  }

  /* Reseñas y testimonios */
  #reseñas {
    background-color: #d8f5d4;
    padding: 25px;
    border-radius: 15px;
    box-shadow: 0 4px 20px rgba(66, 94, 20, 0.3);
    margin-bottom: 80px;
  }
  #reseñas h2 {
    font-size: 2.8rem;
    margin-bottom: 30px;
  }
  #reseña-form {
    display: flex;
    flex-direction: column;
  }
  #reseña-form input, #reseña-form select, #reseña-form textarea {
    margin-bottom: 15px;
    padding: 12px;
    border-radius: 12px;
    border: 2px solid #3a6b20;
    font-size: 1.1em;
  }
  #reseña-form button {
    align-self: flex-start;
    padding: 14px 30px;
    margin-top: 10px;
    background-color: #39922c;
    color: #fff;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    font-weight: 700;
    font-size: 1.2em;
    transition: background-color 0.3s;
  }
  #reseña-form button:hover {
    background-color: #457a2f;
  }
  #lista-reseñas {
    margin-top: 30px;
    max-height: 350px;
    overflow-y: auto;
  }
  .reseña {
    background: #c9f1bb;
    padding: 15px;
    margin-bottom: 20px;
    border-radius: 12px;
    box-shadow: 0 3px 12px rgba(106, 174, 52, 0.2);
  }
  .reseña-rating {
    color: #f4b30a;
    font-size: 1.2em;
  }
  .reseña-aut {
    font-weight: bold;
    color: #345a17;
  }

  /* Footer */
  footer {
    background-color: #3b5921;
    padding: 40px 20px;
    color: #e0f7e4;
    text-align: center;
    font-size: 0.95em;
  }
  footer p {
    margin: 8px 0;
  }
  /* Responsividad */
  @media(max-width: 1024px) {
    #equipo {
      flex-direction: column;
      align-items: center;
    }
    #equipo div {
      flex: 1 1 100%;
    }
  }
</style>
</head>
<body>

<header>
  <h1>Aislando Futuro</h1>
  <p>Innovación sustentable en aislamiento térmico y formación técnica especializada</p>
</header>

<nav>
  <a href="#sobre-nosotros" class="active">Sobre Nosotros</a>
  <a href="#productos">Productos</a>
  <a href="#cursos">Capacitaciones</a>
  <a href="#beneficios">Beneficios</a>
  <a href="#equipo">Nuestro Equipo</a>
  <a href="#proyectos">Proyectos</a>
  <a href="#testimonios">Testimonios</a>
  <a href="#blog">Blog</a>
  <a href="#preguntas">FAQs</a>
  <a href="#reseñas">Reseñas</a>
  <a href="#contacto">Contacto</a>
</nav>

<main>

<!-- Sobre Nosotros -->
<section id="sobre-nosotros">
  <h2>Sobre Nosotros</h2>
  <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=600&q=80" alt="Lana de oveja natural" class="content-img" />
  <p>
    En <strong>Aislando Futuro</strong> conjugan innovación, ciencia y compromiso ambiental para entregar productos de lana de oveja con certificación IDIEM, enfocados en eficiencia y sustentabilidad. Nuestro propósito es transformar el sector de la construcción ecológica, promoviendo tecnologías renovables y procesos responsables.
  </p>
  <p>
    Nuestras soluciones térmicas permiten reducir el consumo energético en un 50-65%, protegen contra incendios, minimizan la contaminación y garantizan durabilidad infinita.
  </p>
</section>

<!-- Productos -->
<section id="productos">
  <h2>Productos</h2>
  <div class="product-info">
    <h3>Rollo aislante térmico sustentable</h3>
    <img src="https://images.unsplash.com/photo-1486308510493-cb558a7fb7f0?auto=format&fit=crop&w=600&q=80" alt="Rollo aislante" class="content-img"/>
    <p>
      Precio: <strong>$10.000 + IVA/m2</strong><br>
      Medidas: 2.40 x 0.60 m<br>
      Conductividad: 0,046 W/mK°<br>
      Espesor: 50 mm<br>
      Certificación: IDIEM<br>
      Características: Denso, ignífugo, natural, fácil instalación y alta resistencia térmica
    </p>
    <ul class="beneficios">
      <li>Reducción de consumo energético del edificio.</li>
      <li>Alta durabilidad y bajo impacto ambiental.</li>
      <li>Mejora del confort interior y control de humedad.</li>
      <li>Producto certificado y natural.</li>
    </ul>
  </div>
</section>

<!-- Capacitaciones -->
<section id="cursos">
  <h2>Nuestros Cursos y Capacitación</h2>
  <p>
    Implementamos programas técnicos especializados para profesionales, empresas, y entusiastas en construcción sustentable y aislamiento térmico. Cada curso está diseñado para ofrecer conocimientos teóricos y prácticos, dando paso a aplicaciones reales.
  </p>
  <div id="lista-cursos">
    <div id="cursos-item">
      <h4>Curso Introducción: Propiedades de la Lana de Oveja</h4>
      <p>Explora las propiedades físicas, químicas y ambientales del material. Aprende sobre beneficios, certificaciones y diferencias competitivas.</p>
    </div>
    <div id="cursos-item">
      <h4>Técnicas de Instalación Básica</h4>
      <p>Formación práctica para instalar lana en muros y techos, técnicas de corte, fijación y hermeticidad.</p>
    </div>
    <div id="cursos-item">
      <h4>Instalaciones Avanzadas y Normativas</h4>
      <p>Profundiza en métodos profesionales, cumplimiento normativo, control de calidad y soluciones a obstáculos técnicos.</p>
    </div>
    <div id="cursos-item">
      <h4>Construcción Sostenible y Certificación Verde</h4>
      <p>Conceptos de arquitectura ecoeficiente, certificaciones LEED y otros estándares internacionales.</p>
    </div>
  </div>
</section>

<!-- Equipo -->
<section id="equipo">
  <h2>Equipo de Trabajo</h2>
  <p>Somos un círculo de expertos dedicados a la sustentabilidad y construcción innovadora.</p>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px;">
    <div class="equipo-miembro">
      <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?auto=format&fit=crop&w=300&q=80" alt="Amara Canteros" />
      <h3>Amara Canteros</h3>
      <p>Ingeniera Ambiental, lidera innovación y desarrollo sustentable.</p>
    </div>
    <div class="equipo-miembro">
      <img src="https://images.unsplash.com/photo-1508214751196-bcfd4ca60f91?auto=format&fit=crop&w=300&q=80" alt="Paz Osorio" />
      <h3>Paz Osorio</h3>
      <p>Especialista en Instalaciones y Certificación Ambiental</p>
    </div>
    <div class="equipo-miembro">
      <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=300&q=80" alt="Alejandro Cáceres" />
      <h3>Alejandro Cáceres</h3>
      <p>Ingeniero en Sistemas y Automatización, encargado de innovación digital y soporte técnico.</p>
    </div>
  </div>
</section>

<!-- Proyectos destacados -->
<section id="proyectos">
  <h2>Proyectos Destacados</h2>
  <div>
    <h3>Viviendas sustentables en Temuco</h3>
    <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=600&q=80" class="content-img" alt="Proyecto viviendas Temuco"/>
    <p>Implementamos aislamiento de lana en 50 viviendas, logrando reducir su consumo energético en promedio del 55%. Los hogares manifiestan mayor confort térmico y acústico.</p>
  </div>
  <div style="margin-top: 40px;">
    <h3>Institución Educativa "Escuela Verde" - Valdivia</h3>
    <img src="https://images.unsplash.com/photo-1494526585095-c41746248156?auto=format&fit=crop&w=600&q=80" class="content-img" alt="Escuela sustentable"/>
    <p>Rehabilitación y aislamiento en aulas con lana de oveja, ofreciendo un ambiente saludable y eficiente con reconocimiento a la certificación de sostenibilidad.</p>
  </div>
</section>

<!-- Reseñas y testimonios -->
<section id="reseñas">
  <h2>Deja tu Reseña</h2>
  <p>Tu experiencia ayuda a otros a confiar en nuestro trabajo. Escribe tu reseña acerca de nuestros productos, cursos o asesorías.</p>
  <form id="reseña-form" onsubmit="return agregarReseña(event)">
    <input type="text" id="reseña-nombre" placeholder="Tu nombre" required minlength="3" />
    <select id="reseña-estrellas" required>
      <option value="">Calificación</option>
      <option value="5">★★★★★ Excelente</option>
      <option value="4">★★★★ Muy Bueno</option>
      <option value="3">★★★ Bueno</option>
      <option value="2">★★ Regular</option>
      <option value="1">★ Malo</option>
    </select>
    <textarea id="reseña-comentario" placeholder="Tu comentario aquí" required minlength="15"></textarea>
    <button type="submit">Enviar Reseña</button>
  </form>
  <div id="lista-resenas" style="margin-top: 30px; max-height: 400px; overflow-y: auto;">
    <!-- reseñas aparecerán aquí -->
  </div>
</section>

<!-- Contacto -->
<section id="contacto">
  <h2>Contacto</h2>
  <p>Contáctanos para más información, cotizaciones, o reserva de capacitaciones.</p>
  <p>📞 Teléfono / WhatsApp: <a href="tel:+56928963880" style="color:#3b6d20;">+56 9 2896 3880</a></p>
  <p>✉️ Email: <a href="mailto:contacto@aislandofuturo.com" style="color:#3b6d20;">contacto@aislandofuturo.com</a></p>
</section>

</main>

<!-- Pie de página -->
<footer>
  <p>© 2025 Aislando Futuro | Todos los derechos reservados</p>
  <p>Dirección: Calle de la Innovación 123, Santiago, Chile</p>
</footer>

<script>
  // Función para validar el formulario de contacto
  function validarFormulario() {
    const nombre = document.getElementById('nombreC').value.trim();
    const email = document.getElementById('emailC').value.trim();
    const mensaje = document.getElementById('mensajeC').value.trim();
    const regex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

    if (nombre.length < 3) {
      alert('Por favor, ingresa un nombre válido.');
      return false;
    }
    if (!regex.test(email)) {
      alert('Por favor, ingresa un email válido.');
      return false;
    }
    if (mensaje.length < 15) {
      alert('El mensaje debe tener mínimo 15 caracteres.');
      return false;
    }
    alert('Mensaje enviado con éxito. Nos pondremos en contacto pronto.');
    return true;
  }

  // Función para agregar reseña
  function agregarReseña(e) {
    e.preventDefault();

    const nombre = document.getElementById('reseña-nombre').value.trim();
    const estrellas = document.getElementById('reseña-estrellas').value;
    const comentario = document.getElementById('reseña-comentario').value.trim();

    if (!nombre || !estrellas || comentario.length < 15) {
      alert('Por favor completa todos los datos correctamente.');
      return false;
    }

    // crear estrellas visuales
    const estrellasVis = '★'.repeat(estrellas) + '☆'.repeat(5 - estrellas);
    const reseñaDiv = document.createElement('div');
    reseñaDiv.className = 'reseña';

    reseñaDiv.innerHTML = `
      <div class="reseña-rating">${estrellasVis}</div>
      <div class="reseña-aut">${nombre}</div>
      <p>${comentario}</p>
    `;
    document.getElementById('lista-resenas').prepend(reseñaDiv);
    document.getElementById('reseña-form').reset();
    alert('¡Gracias por tu reseña!');
    return false;
  }
</script>

</body>
</html>
