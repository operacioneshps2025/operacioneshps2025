<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hidropower System, Inc.</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: 'Roboto', sans-serif; line-height: 1.6; color: #FFB100; background: #000000; }
    header { background: #FFB100; color: #003366; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; }
    nav a { color: #003366; margin-left: 1rem; text-decoration: none; font-weight: bold; }
    .hero { background: url('https://images.unsplash.com/photo-1581090700227-1f94c6f87b99') no-repeat center/cover; padding: 5rem 2rem; color: white; text-align: center; }
    .hero h1 { font-size: 3rem; margin-bottom: 1rem; }
    .hero p { font-size: 1.2rem; margin-bottom: 2rem; }
    .btn { background: #FFB100; color: #003366; padding: 0.75rem 1.5rem; border: none; border-radius: 5px; cursor: pointer; text-decoration: none; font-weight: bold; }
    .section { padding: 3rem 2rem; max-width: 1200px; margin: auto; color: #FFB100; }
    .services { display: flex; flex-wrap: wrap; justify-content: space-around; gap: 2rem; }
    .card { background: #1a1a1a; padding: 1.5rem; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.5); flex: 1 1 30%; }
    .card h3 { margin-bottom: 1rem; color: #FFB100; }
    .why-us ul { list-style: none; margin-top: 1rem; }
    .why-us li::before { content: '✅ '; }
    form { display: flex; flex-direction: column; gap: 1rem; max-width: 600px; margin: auto; }
    input, select, textarea { padding: 0.75rem; border: 1px solid #ccc; border-radius: 5px; background: #1a1a1a; color: #FFB100; }
    footer { background: #FFB100; color: #003366; padding: 2rem; text-align: center; margin-top: 3rem; }
    .testimonio { background: #1a1a1a; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.5); margin-top: 2rem; text-align: center; color: #FFB100; }
    .testimonio p { font-style: italic; margin-bottom: 1rem; }
    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #25D366;
      color: white;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      z-index: 1000;
      text-decoration: none;
      font-size: 2rem;
    }
  </style>
</head>
<body>
  <header>
    <img src="logo principal-min (1) (1).jpg" alt="Logo Hidropower" style="height: 100px;">
    <nav>
      <a href="#servicios">Servicios</a>
      <a href="#porque">¿Por qué elegirnos?</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Soluciones de Energía y Agua</h1>
    <p>Generadores, hidroneumáticos y limpieza de tanques para hogares y empresas</p>
    <a href="#contacto" class="btn">Solicita una inspección gratuita</a>
  </section>

  <section id="servicios" class="section">
    <h2 style="text-align:center; margin-bottom: 2rem;">Nuestros Servicios</h2>
    <div class="services">
      <div class="card">
        <h3>⚡ Generadores Eléctricos</h3>
        <p>Venta, instalación y mantenimiento preventivo de generadores para todo tipo de necesidad.</p>
      </div>
      <div class="card">
        <h3>💧 Sistemas Hidroneumáticos</h3>
        <p>Diseño, instalación y servicio técnico para garantizar presión constante de agua.</p>
      </div>
      <div class="card">
        <h3>🧼 Limpieza de Tanques</h3>
        <p>Sanitización profesional de tanques de reserva para uso residencial o comercial.</p>
      </div>
    </div>
  </section>

  <section id="porque" class="section why-us">
    <h2 style="text-align:center; margin-bottom: 2rem;">¿Por qué elegirnos?</h2>
    <ul>
      <li>Más de 10 años de experiencia en el mercado.</li>
      <li>Atención personalizada y soporte técnico rápido.</li>
      <li>Personal capacitado y certificado.</li>
      <li>Cumplimiento de normativas de seguridad e higiene.</li>
    </ul>
  </section>

  <section class="section">
    <h2 style="text-align:center; margin-bottom: 2rem;">Testimonios</h2>
    <div class="testimonio">
      <p>“Excelente servicio y puntualidad. Solucionaron nuestro problema de presión de agua en menos de un día.”</p>
      <strong>- María González, cliente residencial</strong>
    </div>
    <div class="testimonio">
      <p>“Los generadores que instalaron en nuestra empresa han funcionado sin fallas. Muy recomendados.”</p>
      <strong>- José Rivera, gerente de operaciones</strong>
    </div>
  </section>

  <section id="contacto" class="section">
    <h2 style="text-align:center; margin-bottom: 2rem;">Contáctanos</h2>
    <form onsubmit="enviarWhatsapp(event)">
      <input type="text" name="nombre" placeholder="Nombre completo" required>
      <input type="tel" name="telefono" placeholder="Teléfono" required>
      <input type="email" name="email" placeholder="Correo electrónico" required>
      <select name="servicio">
        <option>Servicio de interés</option>
        <option>Generadores eléctricos</option>
        <option>Sistemas hidroneumáticos</option>
        <option>Limpieza de tanques</option>
      </select>
      <textarea name="comentarios" rows="4" placeholder="Comentarios adicionales"></textarea>
      <button class="btn" type="submit">Enviar por WhatsApp</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Hidropower System, Inc. – Todos los derechos reservados.</p>
    <p>Tel: +507 6211-9020 | Correo: servicios@hidropower.com</p>
  </footer>

  <a href="https://wa.me/50762119020" class="whatsapp-float" target="_blank" title="Escríbenos por WhatsApp">
    🟢
  </a>

  <script>
    function enviarWhatsapp(event) {
      event.preventDefault();
      const form = event.target;
      const nombre = form.nombre.value;
      const telefono = form.telefono.value;
      const email = form.email.value;
      const servicio = form.servicio.value;
      const comentarios = form.comentarios.value;
      const mensaje = `Hola, soy ${nombre}. Tel: ${telefono}, Email: ${email}. Estoy interesado en: ${servicio}. Comentarios: ${comentarios}`;
      const url = `https://wa.me/50762119020?text=${encodeURIComponent(mensaje)}`;
      window.open(url, '_blank');
    }
  </script>
</body>
</html>
