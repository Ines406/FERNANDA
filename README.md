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
      /* Fondo general de la pantalla */
      --bg-body: #f7ebeb;

      /* Paleta Rosa Gold para el interior de las tarjetas */
      --rose-gold-card: linear-gradient(135deg, #ffffff 0%, #fbebeb 50%, #f4d4d8 100%);
      --rose-gold-dark: #b86b77;
      --rose-gold-deep: #8c424e;
      --gold-border: linear-gradient(135deg, #e6ca65 0%, #b86b77 50%, #e6ca65 100%);
      
      --ink: #3a2226;
      --muted: #6b4d52;
      --line: rgba(184, 107, 119, 0.25);
      --shadow: 0 16px 35px rgba(140, 66, 78, 0.2);
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
      background-color: var(--bg-body);
    }

    .container {
      width: min(calc(100% - 1.5rem), var(--max));
      margin-inline: auto;
    }

    /* Botón flotante de Música */
    .music-control {
      position: fixed;
      top: 15px;
      right: 15px;
      z-index: 1000;
      background: #ffffff;
      border: 2px solid var(--rose-gold-dark);
      border-radius: 50%;
      width: 48px;
      height: 48px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 15px rgba(140, 66, 78, 0.25);
      cursor: pointer;
      font-size: 1.2rem;
    }

    .bottom-nav {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      z-index: 100;
      background: rgba(255, 240, 243, 0.95);
      backdrop-filter: blur(12px);
      border-top: 1px solid var(--line);
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
      font-weight: 600;
      text-decoration: none;
    }
    .bottom-nav a svg {
      width: 20px;
      height: 20px;
      fill: var(--rose-gold-deep);
      margin-bottom: 2px;
    }

    /* Tarjetas principales */
    .hero-card {
      position: relative;
      margin-top: 1rem;
      padding: 2.5rem 1.2rem;
      border-radius: var(--radius);
      background: var(--rose-gold-card);
      border: 2px solid #e6ca65;
      box-shadow: var(--shadow);
      text-align: center;
    }

    .profile-photo-container {
      width: 180px;
      height: 180px;
      margin: 0 auto 1.2rem auto;
      border-radius: 50%;
      padding: 5px;
      background: var(--gold-border);
      box-shadow: 0 10px 25px rgba(140, 66, 78, 0.3);
    }
    .profile-photo {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top center;
      border-radius: 50%;
      border: 4px solid #fff;
      display: block;
    }

    .eyebrow {
      font-size: 0.75rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--rose-gold-deep);
      font-weight: 600;
      margin-bottom: 0.5rem;
    }

    .script {
      font-family: "Great Vibes", cursive;
      font-size: 3.4rem;
      color: var(--rose-gold-deep);
      line-height: 1;
      text-shadow: 1px 1px 2px rgba(255, 255, 255, 0.8);
    }

    h1 {
      font-family: "Playfair Display", serif;
      font-size: 3rem;
      color: var(--ink);
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
      background: rgba(255, 255, 255, 0.85);
      border: 1px solid var(--rose-gold-dark);
      padding: 0.6rem 0.2rem;
      border-radius: 16px;
      text-align: center;
      box-shadow: 0 4px 10px rgba(184, 107, 119, 0.15);
    }
    .timer-box strong {
      display: block;
      font-size: 1.4rem;
      font-family: "Playfair Display", serif;
      color: var(--rose-gold-deep);
    }
    .timer-box span {
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--muted);
      font-weight: 600;
    }

    .panel {
      border-radius: var(--radius);
      padding: 1.5rem;
      margin-top: 1.2rem;
      border: 1px solid rgba(230, 202, 101, 0.6);
      background: var(--rose-gold-card);
      box-shadow: var(--shadow);
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
      color: var(--rose-gold-deep);
      font-weight: 600;
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
      color: var(--rose-gold-deep);
    }
    .family-group p {
      margin: 0;
      font-weight: 600;
      font-size: 1.05rem;
      line-height: 1.4;
      color: var(--ink);
    }

    .timeline-item {
      display: grid;
      grid-template-columns: 65px 1fr;
      gap: 0.8rem;
      padding: 0.8rem 0;
      border-bottom: 1px dashed var(--rose-gold-dark);
    }
    .timeline-item:last-child { border-bottom: none; }
    .timeline-item b { color: var(--rose-gold-deep); font-size: 0.9rem; }
    .timeline-item strong { display: block; font-size: 1rem; color: var(--ink); }
    .timeline-item p { margin: 0; font-size: 0.85rem; color: var(--muted); }

    .dresscode-box, .gift-box {
      text-align: center;
      padding: 1.2rem;
      background: rgba(255, 255, 255, 0.7);
      border-radius: 18px;
      border: 1px solid var(--rose-gold-dark);
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
      background: linear-gradient(135deg, #b86b77 0%, #8c424e 100%);
      box-shadow: 0 8px 20px rgba(140, 66, 78, 0.3);
    }
    .btn-secondary {
      color: var(--rose-gold-deep);
      background: #ffffff;
      border: 1.5px solid var(--rose-gold-dark);
      font-weight: 600;
    }

    .footer {
      text-align: center;
      padding: 2rem 0;
      font-size: 0.85rem;
      color: var(--muted);
      font-weight: 500;
    }
  </style>
</head>
<body>

  <!-- Reproductor de audio apuntando a Valiente.mp3 -->
  <audio id="bg-music" loop preload="auto" src="Valiente.mp3"></audio>

  <!-- Botón Flotante para Audio -->
  <button class="music-control" id="music-btn" onclick="toggleMusic()" title="Reproducir / Pausar Música">
    🎵
  </button>

  <main class="container">

    <!-- Hero Card -->
    <section class="hero-card" id="inicio">
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

    <!-- Programa del Evento -->
    <section class="panel" id="programa">
      <span class="section-sub">Itinerario</span>
      <h2 class="section-title">Programa del Evento</h2>
      
      <div class="timeline" style="margin-top: 1rem;">
        <div class="timeline-item">
          <b>7:00 PM</b>
          <div>
            <strong>Ceremonia Religiosa</strong>
            <p>La Acción Católica</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>8:00 PM</b>
          <div>
            <strong>Recepción de Invitados</strong>
            <p>Salón La Floresta</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>9:30 PM</b>
          <div>
            <strong>Cena de Honor</strong>
            <p>Disfrutaremos un banquete especial</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>10:30 PM</b>
          <div>
            <strong>Vals & Brindis</strong>
            <p>Momento principal de la noche</p>
          </div>
        </div>
        <div class="timeline-item">
          <b>11:00 PM</b>
          <div>
            <strong>Gran Fiesta</strong>
            <p>¡Música y baile!</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Mesa de Regalos -->
    <section class="panel" id="regalos">
      <span class="section-sub">Muestra de afecto</span>
      <h2 class="section-title">Mesa de Regalos</h2>
      <p style="text-align: center; color: var(--muted); font-size: 0.9rem; margin-bottom: 1rem;">
        El mejor regalo es tu presencia en este día tan especial. Si deseas tenerme un detalle, puedes consultar las siguientes opciones:
      </p>

      <div class="gift-box">
        <div style="font-size: 2rem; margin-bottom: 0.3rem;">🎁</div>
        <strong style="display:block; font-size: 1.05rem; color: var(--rose-gold-deep);">Lluvia de Sobres</strong>
        <p style="margin: 0.4rem 0 0 0; font-size: 0.85rem; color: var(--muted);">
          Habrá un buzón especial en la entrada del salón para depositar tu sobre.
        </p>
      </div>
    </section>

    <!-- Código de Vestimenta -->
    <section class="panel">
      <span class="section-sub">Detalles</span>
      <h2 class="section-title">Código de Vestimenta</h2>
      
      <div class="dresscode-box">
        <div style="font-size: 2rem; margin-bottom: 0.5rem;">👗👔</div>
        <h3 style="margin: 0 0 0.4rem 0; font-family: 'Playfair Display', serif; color: var(--ink);">Formal</h3>
        <p style="margin: 0; font-size: 0.9rem; color: var(--rose-gold-deep); font-weight: 600;">
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

      <hr style="border: 0; border-top: 1px dashed var(--rose-gold-dark); margin: 1.2rem 0;">

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
          <img src="https://api.qrserver.com/v1/create-qr-code/?size=180x180&data=https%3A%2F%2Fdrive.google.com%2Fdrive%2Ffolders%2F1c7YFWJKr6N45P8C6X-K9EWjC5P-WZh8p%3Fusp%3Dsharing" alt="QR Google Drive Fotos" style="border-radius: 16px; border: 2px solid var(--rose-gold-dark); padding: 0.5rem; background: #fff;" />
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

  <!-- Navegación inferior -->
  <nav class="bottom-nav">
    <a href="#inicio">
      <svg viewBox="0 0 24 24"><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>
      Inicio
    </a>
    <a href="#programa">
      <svg viewBox="0 0 24 24"><path d="M19 3h-1V1h-2v2H8V1H6v2H5c-1.11 0-1.99.9-1.99 2L3 19c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm0 16H5V8h14v11z"/></svg>
      Evento
    </a>
    <a href="#regalos">
      <svg viewBox="0 0 24 24"><path d="M20 6h-3.18C16.96 5.42 17 4.72 17 4c0-2.21-1.79-4-4-4-1.2 0-2.27.53-3 1.36C9.27.53 8.2 0 7 0 4.79 0 3 1.79 3 4c0 .72.04 1.42.18 2H0v14c0 1.1.9 2 2 2h20c1.1 0 2-.9 2-2V6h-4zm-7-2c0-1.1.9-2 2-2s2 .9 2 2-.9 2-2 2h-2V4zM7 2c1.1 0 2 .9 2 2v2H7c-1.1 0-2-.9-2-2s.9-2 2-2z"/></svg>
      Regalos
    </a>
    <a href="#ubicaciones">
      <svg viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
      Mapa
    </a>
  </nav>

  <script>
    const music = document.getElementById('bg-music');
    const musicBtn = document.getElementById('music-btn');

    // Intentar reproducción automática al cargar la página
    function tryPlayMusic() {
      music.play().then(() => {
        musicBtn.innerHTML = '🔊';
      }).catch(() => {
        // Si el navegador bloquea el autoplay, cambiar ícono para inducir clic
        musicBtn.innerHTML = '🎵';
      });
    }

    window.addEventListener('DOMContentLoaded', tryPlayMusic);

    // Iniciar reproducción al primer clic/toque en la página (restricción común de navegadores móviles)
    const enableAudioOnTouch = () => {
      if (music.paused) {
        music.play().then(() => {
          musicBtn.innerHTML = '🔊';
        });
      }
      document.removeEventListener('click', enableAudioOnTouch);
      document.removeEventListener('touchstart', enableAudioOnTouch);
    };

    document.addEventListener('click', enableAudioOnTouch);
    document.addEventListener('touchstart', enableAudioOnTouch);

    function toggleMusic() {
      if (music.paused) {
        music.play();
        musicBtn.innerHTML = '🔊';
      } else {
        music.pause();
        musicBtn.innerHTML = '🎵';
      }
    }

    // Lógica de Cuenta Regresiva (Ajustado a 7:00 PM)
    const eventTarget = new Date(2026, 8, 19, 19, 0, 0).getTime();

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
