[Index.html](https://github.com/user-attachments/files/31500201/Index.html)
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>XV Años | María Fernanda</title>
  <meta name="description" content="Invitación digital para los XV años de María Fernanda." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@500;600;700;800&family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --ivory: #fcf8f4;
      --champagne: #f2e4d7;
      --blush: #e9c8cf;
      --rose: #b87885;
      --rose-deep: #8d5661;
      --gold: #c9a56a;
      --gold-2: #e4c48f;
      --ink: #3e2b31;
      --muted: #7f6870;
      --white: rgba(255, 255, 255, 0.85);
      --line: rgba(109, 78, 85, 0.12);
      --shadow: 0 16px 40px rgba(116, 74, 84, 0.12);
      --radius: 24px;
      --max: 600px;
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      padding-bottom: 70px;
      font-family: "Outfit", sans-serif;
      color: var(--ink);
      background: linear-gradient(180deg, #fffdfa 0%, #f9f1ea 50%, #f6ede6 100%);
    }

    .container {
      width: min(calc(100% - 1.5rem), var(--max));
      margin-inline: auto;
    }

    .bottom-nav {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      z-index: 100;
      background: rgba(252, 248, 244, 0.94);
      backdrop-filter: blur(12px);
      border-top: 1px solid rgba(141, 86, 97, 0.12);
      display: flex;
      justify-content: space-around;
      padding: 0.6rem 0;
    }
    .bottom-nav a {
      display: flex;
      flex-direction: column;
      align-items: center;
      font-size: 0.7rem;
      color: var(--muted);
      font-weight: 500;
      text-decoration: none;
    }
    .bottom-nav a svg {
      width: 20px;
      height: 20px;
      fill: var(--rose-deep);
      margin-bottom: 2px;
    }

    .hero-card {
      position: relative;
      margin-top: 1rem;
      padding: 2.5rem 1.2rem;
      border-radius: var(--radius);
      background: linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.7));
      border: 1px solid rgba(141, 86, 97, 0.15);
      box-shadow: var(--shadow);
      text-align: center;
    }

    /* Estilo estilizado para la foto principal */
    .profile-photo-container {
      width: 170px;
      height: 170px;
      margin: 0 auto 1.2rem auto;
      border-radius: 50%;
      padding: 6px;
      background: linear-gradient(135deg, var(--gold), var(--rose), var(--gold-2));
      box-shadow: 0 10px 25px rgba(184, 120, 133, 0.3);
    }
    .profile-photo {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top center;
      border-radius: 50%;
      border: 3px solid #fff;
      display: block;
    }

    .full-photo-container {
      width: 100%;
      border-radius: 18px;
      overflow: hidden;
      border: 1px solid rgba(141, 86, 97, 0.15);
      box-shadow: var(--shadow);
      margin-top: 1rem;
    }
    .full-photo {
      width: 100%;
      height: auto;
      display: block;
    }

    .eyebrow {
      font-size: 0.72rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--rose-deep);
      margin-bottom: 0.5rem;
    }

    .script {
      font-family: "Great Vibes", cursive;
      font-size: 3rem;
      color: var(--gold);
      line-height: 1;
    }

    h1 {
      font-family: "Playfair Display", serif;
      font-size: 3rem;
      margin: 0.2rem 0;
      line-height: 1;
    }

    .countdown-container {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 0.5rem;
      margin: 1.5rem 0;
    }
    .timer-box {
      background: rgba(255, 255, 255, 0.8);
      border: 1px solid rgba(141, 86, 97, 0.12);
      padding: 0.6rem 0.2rem;
      border-radius: 16px;
      text-align: center;
    }
    .timer-box strong {
      display: block;
      font-size: 1.4rem;
      font-family: "Playfair Display", serif;
      color: var(--rose-deep);
    }
    .timer-box span {
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--muted);
    }

    .panel {
      border-radius: var(--radius);
      padding: 1.5rem;
      margin-top: 1.2rem;
      border: 1px solid rgba(141, 86, 97, 0.1);
      background: rgba(255, 255, 255, 0.75);
      box-shadow: var(--shadow);
      backdrop-filter: blur(10px);
    }

    .section-title {
      font-family: "Playfair Display", serif;
      font-size: 1.8rem;
      color: var(--ink);
      margin-bottom: 0.2rem;
      text-align: center;
    }
    .section-sub {
      font-size: 0.75rem;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--rose-deep);
      text-align: center;
      display: block;
      margin-bottom: 1rem;
    }

    .family-grid {
      display: grid;
      gap: 1rem;
      text-align: center;
    }
    .family-group h4 {
      margin: 0 0 0.3rem 0;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--gold);
    }
    .family-group p {
      margin: 0;
      font-weight: 600;
      font-size: 1.05rem;
      line-height: 1.4;
    }

    .timeline-item {
      display: grid;
      grid-template-columns: 65px 1fr;
      gap: 0.8rem;
      padding: 0.8rem 0;
      border-bottom: 1px dashed var(--line);
    }
    .timeline-item:last-child { border-bottom: none; }
    .timeline-item b { color: var(--rose-deep); font-size: 0.9rem; }
    .timeline-item strong { display: block; font-size: 1rem; }
    .timeline-item p { margin: 0; font-size: 0.85rem; color: var(--muted); }

    .dresscode-box {
      text-align: center;
      padding: 1.2rem;
      background: linear-gradient(135deg, rgba(233, 200, 207, 0.2), rgba(201, 165, 106, 0.15));
      border-radius: 18px;
      border: 1px solid rgba(184, 120, 133, 0.3);
    }
    .dresscode-icon {
      font-size: 2rem;
      margin-bottom: 0.5rem;
    }

    .btn {
      width: 100%;
      min-height: 50px;
      padding: 0 1rem;
      border: 0;
      border-radius: 999px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      cursor: pointer;
      font-weight: 700;
      font-size: 0.95rem;
      margin-top: 0.8rem;
      text-decoration: none;
    }
    .btn-primary {
      color: #fff;
      background: linear-gradient(135deg, var(--rose) 0%, var(--rose-deep) 100%);
      box-shadow: 0 10px 24px rgba(141, 86, 97, 0.25);
    }
    .btn-secondary {
      color: var(--ink);
      background: #fff;
      border: 1px solid rgba(141, 86, 97, 0.2);
    }

    .footer {
      text-align: center;
      padding: 2rem 0;
      font-size: 0.85rem;
      color: var(--muted);
    }
  </style>
</head>
<body>

  <main class="container">

    <!-- Hero Card -->
    <section class="hero-card" id="inicio">
      <!-- Foto de Perfil Estilizada -->
      <div class="profile-photo-container">
        <img src="foto-xv.jpg" alt="María Fernanda" class="profile-photo" />
      </div>

      <div class="eyebrow">Con la bendición de Dios y mi familia</div>
      <div class="script">Mis XV Años</div>
      <h1>María Fernanda</h1>
      
      <p style="color: var(--muted); font-size: 0.95rem; line-height: 1.6; margin-top: 1rem;">
        Hay momentos en la vida que son inolvidables, pero compartirlos con quienes más quieres los hace eternos.
      </p>

      <!-- Cuenta Regresiva -->
      <div class="countdown-container">
        <div class="timer-box">
          <strong id="days">00</strong>
          <span>Días</span>
        </div>
        <div class="timer-box">
          <strong id="hours">00</strong>
          <span>Horas</span>
        </div>
        <div class="timer-box">
          <strong id="minutes">00</strong>
          <span>Min</span>
        </div>
        <div class="timer-box">
          <strong id="seconds">00</strong>
          <span>Seg</span>
        </div>
      </div>

      <a class="btn btn-primary" href="https://docs.google.com/forms/d/e/1FAIpQLSeIcGvxEVDkqtHy1ztPy_zT_lzhEAHD8qdwwyrTA4VrODxc8g/viewform?usp=publish-editor" target="_blank" rel="noopener noreferrer">
        Confirmar Asistencia
      </a>
    </section>

    <!-- Galería Destacada -->
    <section class="panel">
      <div class="full-photo-container">
        <img src="foto-xv.jpg" alt="María Fernanda XV Años" class="full-photo" />
      </div>
    </section>

    <!-- Familia y Padrinos -->
    <section class="panel" id="familia">
      <span class="section-sub">Acompañada de</span>
      <h2 class="section-title">Mi Familia</h2>

      <div class="family-grid" style="margin-top: 1.2rem;">
        <div class="family-group">
          <h4>Mis Padres</h4>
          <p>Cesar Alejandro Chávez Guevara</p>
          <p>Araceli Sierra Martínez</p>
        </div>

        <div class="family-group" style="margin-top: 0.6rem;">
          <h4>Mi Hermanita</h4>
          <p>Ana Julia Chávez Sierra</p>
        </div>

        <div class="family-group" style="margin-top: 0.6rem;">
          <h4>Mis Padrinos</h4>
          <p>Gerardo Meléndez</p>
          <p>Nadia Isabel Romero</p>
        </div>
      </div>
    </section>

    <!-- Programa -->
    <section class="panel" id="programa">
      <span class="section-sub">Itinerario</span>
      <h2 class="section-title">Programa del Evento</h2>
      
      <div class="timeline" style="margin-top: 1rem;">
        <div class="timeline-item">
          <b>5:30 PM</b>
          <div>
            <strong>Ceremonia Religiosa</strong>
            <p>La Acción Católica</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>7:00 PM</b>
          <div>
            <strong>Recepción de Invitados</strong>
            <p>Salón La Floresta</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>8:30 PM</b>
          <div>
            <strong>Cena de Honor</strong>
            <p>Disfrutaremos un banquete especial</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>9:30 PM</b>
          <div>
            <strong>Vals & Brindis</strong>
            <p>Momento principal de la noche</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>10:00 PM</b>
          <div>
            <strong>Gran Fiesta</strong>
            <p>¡Música y baile!</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Código de Vestimenta -->
    <section class="panel">
      <span class="section-sub">Detalles</span>
      <h2 class="section-title">Código de Vestimenta</h2>
      
      <div class="dresscode-box">
        <div class="dresscode-icon">👗👔</div>
        <h3 style="margin: 0 0 0.4rem 0; font-family: 'Playfair Display', serif;">Formal</h3>
        <p style="margin: 0; font-size: 0.9rem; color: var(--rose-deep); font-weight: 600;">
          ✨ Reservado el color Rosa exclusivamente para la Quinceañera. ✨
        </p>
      </div>
    </section>

    <!-- Ubicaciones -->
    <section class="panel" id="ubicaciones">
      <span class="section-sub">¿Cómo llegar?</span>
      <h2 class="section-title">Ubicaciones</h2>

      <div style="margin-top: 1rem;">
        <strong style="display:block; font-size: 1.1rem;">⛪ Ceremonia Religiosa</strong>
        <p style="margin: 0.2rem 0; color: var(--muted); font-size: 0.9rem;">La Acción Católica</p>
        <p style="margin: 0; color: var(--muted); font-size: 0.85rem;">Independencia #1000, Col. Centro, San Luis Potosí</p>
        <a class="btn btn-secondary" href="https://maps.google.com/?q=22.150908941603735,-100.97952416292142" target="_blank" rel="noopener noreferrer">Abrir Misa en Maps</a>
      </div>

      <hr style="border: 0; border-top: 1px solid var(--line); margin: 1.2rem 0;">

      <div>
        <strong style="display:block; font-size: 1.1rem;">🎉 Recepción & Fiesta</strong>
        <p style="margin: 0.2rem 0; color: var(--muted); font-size: 0.9rem;">Salón La Floresta</p>
        <p style="margin: 0; color: var(--muted); font-size: 0.85rem;">Carr. Antigua Matehuala Km4</p>
        <a class="btn btn-primary" href="https://maps.app.goo.gl/5dtMULV19pxriPjZ9" target="_blank" rel="noopener noreferrer">Abrir Salón en Maps</a>
      </div>
    </section>

    <!-- Galería / QR (Google Drive de Fotos) -->
    <section class="panel">
      <span class="section-sub">Recuerdos</span>
      <h2 class="section-title">Comparte tus Fotos</h2>
      <p style="text-align: center; color: var(--muted); font-size: 0.9rem; margin-bottom: 1rem;">
        Escanea el QR o da clic en el botón para subir tus fotos a la carpeta compartida en Google Drive.
      </p>
      <div style="display: flex; justify-content: center;">
        <a href="https://drive.google.com/drive/folders/1c7YFWJKr6N45P8C6X-K9EWjC5P-WZh8p?usp=sharing" target="_blank" rel="noopener noreferrer">
          <img src="https://api.qrserver.com/v1/create-qr-code/?size=180x180&data=https%3A%2F%2Fdrive.google.com%2Fdrive%2Ffolders%2F1c7YFWJKr6N45P8C6X-K9EWjC5P-WZh8p%3Fusp%3Dsharing" alt="QR Google Drive Fotos" style="border-radius: 16px; border: 1px solid var(--line); padding: 0.5rem; background: #fff;" />
        </a>
      </div>
      <a class="btn btn-secondary" href="https://drive.google.com/drive/folders/1c7YFWJKr6N45P8C6X-K9EWjC5P-WZh8p?usp=sharing" target="_blank" rel="noopener noreferrer">
        📁 Abrir Carpeta de Fotos
      </a>
    </section>

    <footer class="footer">
      Con amor, María Fernanda y Familia ❤️<br>2026
    </footer>

  </main>

  <!-- Navegación inferior estilo App Móvil -->
  <nav class="bottom-nav">
    <a href="#inicio">
      <svg viewBox="0 0 24 24"><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>
      Inicio
    </a>
    <a href="#familia">
      <svg viewBox="0 0 24 24"><path d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"/></svg>
      Familia
    </a>
    <a href="#programa">
      <svg viewBox="0 0 24 24"><path d="M19 3h-1V1h-2v2H8V1H6v2H5c-1.11 0-1.99.9-1.99 2L3 19c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm0 16H5V8h14v11z"/></svg>
      Evento
    </a>
    <a href="#ubicaciones">
      <svg viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
      Mapa
    </a>
  </nav>

  <!-- Lógica de Cuenta Regresiva Garantizada -->
  <script>
    // Fecha: 19 de Septiembre de 2026 a las 17:30:00 (Mes 8 = Septiembre en JS)
    const eventTarget = new Date(2026, 8, 19, 17, 30, 0).getTime();

    function updateTimer() {
      const now = new Date().getTime();
      const difference = eventTarget - now;

      if (difference <= 0) {
        document.getElementById("days").innerText = "00";
        document.getElementById("hours").innerText = "00";
        document.getElementById("minutes").innerText = "00";
        document.getElementById("seconds").innerText = "00";
        return;
      }

      const days = Math.floor(difference / (1000 * 60 * 60 * 24));
      const hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((difference % (1000 * 60)) / 1000);

      document.getElementById("days").innerText = days < 10 ? "0" + days : days;
      document.getElementById("hours").innerText = hours < 10 ? "0" + hours : hours;
      document.getElementById("minutes").innerText = minutes < 10 ? "0" + minutes : minutes;
      document.getElementById("seconds").innerText = seconds < 10 ? "0" + seconds : seconds;
    }

    updateTimer();
    setInterval(updateTimer, 1000);
  </script>
</body>
</html>
