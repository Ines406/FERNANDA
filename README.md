(https://github.com/user-attachments/files/31497605/Index.html)
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Invitación XV Años | María Fernanda</title>
  <meta name="description" content="Invitación digital elegante para XV años con confirmación de asistencia, QR para fotos y ubicación del evento." />
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
      --white: rgba(255, 255, 255, 0.72);
      --line: rgba(109, 78, 85, 0.12);
      --shadow: 0 24px 70px rgba(116, 74, 84, 0.12);
      --radius: 30px;
      --radius-lg: 42px;
      --max: 1200px;
    }

    * {
      box-sizing: border-box;
    }
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: "Outfit", sans-serif;
      color: var(--ink);
      background: radial-gradient(circle at 10% 8%, rgba(201, 165, 106, 0.18), transparent 18%),
        radial-gradient(circle at 86% 12%, rgba(184, 120, 133, 0.15), transparent 20%),
        linear-gradient(180deg, #fffdfa 0%, #f9f1ea 50%, #f6ede6 100%);
      overflow-x: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      inset: 0;
      pointer-events: none;
      opacity: 0.2;
      background: radial-gradient(circle at 20% 20%, rgba(255, 255, 255, 0.7) 0 2px, transparent 3px),
        radial-gradient(circle at 80% 30%, rgba(255, 255, 255, 0.65) 0 2px, transparent 3px),
        radial-gradient(circle at 35% 75%, rgba(255, 255, 255, 0.7) 0 2px, transparent 3px),
        radial-gradient(circle at 75% 80%, rgba(255, 255, 255, 0.7) 0 2px, transparent 3px);
      background-size: 260px 260px;
    }

    a {
      text-decoration: none;
      color: inherit;
    }
    img {
      max-width: 100%;
      display: block;
    }
    button,
    input,
    textarea,
    select {
      font: inherit;
    }

    .container {
      width: min(calc(100% - 2rem), var(--max));
      margin-inline: auto;
    }

    .reveal {
      opacity: 0;
      transform: translateY(28px);
      transition: opacity 0.9s ease, transform 0.9s ease;
    }
    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .topbar {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(14px);
      background: rgba(252, 248, 244, 0.65);
      border-bottom: 1px solid rgba(141, 86, 97, 0.08);
    }

    .nav {
      min-height: 74px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .brand {
      display: flex;
      flex-direction: column;
      line-height: 1;
    }
    .brand span {
      font-size: 0.74rem;
      letter-spacing: 0.26em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 0.35rem;
    }
    .brand strong {
      font-family: "Playfair Display", serif;
      font-size: 1.8rem;
      font-weight: 700;
    }

    .nav-links {
      display: none;
      gap: 1.25rem;
    }
    .nav-links a {
      font-size: 0.95rem;
      color: var(--muted);
      position: relative;
    }
    .nav-links a::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: -6px;
      width: 100%;
      height: 1px;
      background: var(--rose);
      transform: scaleX(0);
      transform-origin: right;
      transition: transform 0.3s ease;
    }
    .nav-links a:hover::after {
      transform: scaleX(1);
      transform-origin: left;
    }

    .hero {
      padding: clamp(2rem, 4vw, 4rem) 0 1rem;
    }

    .hero-shell {
      position: relative;
      overflow: hidden;
      border-radius: var(--radius-lg);
      border: 1px solid rgba(141, 86, 97, 0.1);
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.64), rgba(255, 255, 255, 0.45)),
        linear-gradient(135deg, rgba(255, 255, 255, 0.3), rgba(201, 165, 106, 0.08));
      box-shadow: var(--shadow);
      backdrop-filter: blur(12px);
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1fr;
    }

    .hero-copy {
      padding: clamp(1.5rem, 4vw, 3.5rem);
      position: relative;
      z-index: 1;
      min-height: 540px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .hero-art {
      position: relative;
      min-height: 420px;
      background: radial-gradient(circle at 30% 20%, rgba(255, 255, 255, 0.82), transparent 18%),
        linear-gradient(160deg, #f5e6dc 0%, #e8cdc8 48%, #d6b0ae 100%);
      overflow: hidden;
    }

    .hero-art::before {
      content: "";
      position: absolute;
      inset: 12% 12% auto auto;
      width: 180px;
      height: 180px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(201, 165, 106, 0.35), transparent 68%);
      filter: blur(8px);
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 0.7rem;
      width: max-content;
      padding: 0.55rem 0.9rem;
      border-radius: 999px;
      background: rgba(255, 255, 255, 0.58);
      border: 1px solid rgba(141, 86, 97, 0.1);
      color: var(--rose-deep);
      font-size: 0.75rem;
      letter-spacing: 0.24em;
      text-transform: uppercase;
      margin-bottom: 1rem;
    }

    .script {
      font-family: "Great Vibes", cursive;
      font-size: clamp(2.4rem, 6vw, 4rem);
      color: var(--gold);
      line-height: 1;
      margin-bottom: 0.2rem;
    }

    h1,
    h2,
    h3 {
      margin: 0;
      font-family: "Playfair Display", serif;
      line-height: 0.96;
      color: var(--ink);
    }

    h1 {
      font-size: clamp(3.2rem, 10vw, 6.9rem);
      letter-spacing: -0.04em;
      max-width: 8ch;
    }

    .lead {
      margin: 1.1rem 0 0;
      max-width: 58ch;
      color: var(--muted);
      line-height: 1.85;
      font-size: clamp(1rem, 2vw, 1.08rem);
    }

    .hero-data {
      display: grid;
      gap: 1rem;
      margin-top: 2rem;
    }

    .data-block {
      display: grid;
      grid-template-columns: 84px 1fr;
      gap: 1rem;
      padding: 1rem 0;
      border-top: 1px solid var(--line);
    }

    .data-block:first-child {
      border-top: 0;
      padding-top: 0;
    }

    .data-block small {
      font-size: 0.74rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--rose-deep);
      padding-top: 0.35rem;
    }

    .data-block strong {
      display: block;
      font-size: 1.05rem;
      margin-bottom: 0.2rem;
    }

    .data-block span {
      color: var(--muted);
      line-height: 1.7;
    }

    .cta-row {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
      margin-top: 1.6rem;
    }

    .btn {
      min-height: 52px;
      padding: 0 1.2rem;
      border: 0;
      border-radius: 999px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.7rem;
      cursor: pointer;
      font-weight: 700;
      transition: transform 0.25s ease, box-shadow 0.25s ease, background 0.25s ease;
    }

    .btn:active {
      transform: scale(0.98);
    }
    .btn-primary {
      color: #fff;
      background: linear-gradient(135deg, var(--rose) 0%, var(--rose-deep) 100%);
      box-shadow: 0 14px 30px rgba(141, 86, 97, 0.26);
    }
    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 18px 38px rgba(141, 86, 97, 0.32);
    }
    .btn-secondary {
      color: var(--ink);
      background: rgba(255, 255, 255, 0.76);
      border: 1px solid rgba(141, 86, 97, 0.12);
    }
    .btn-secondary:hover {
      transform: translateY(-2px);
      background: rgba(255, 255, 255, 0.9);
    }

    .frame {
      position: absolute;
      inset: 2rem;
      border: 1px solid rgba(255, 255, 255, 0.45);
      border-radius: 28px;
      pointer-events: none;
    }

    .portrait-wrap {
      position: absolute;
      inset: 1.5rem;
      display: grid;
      place-items: center;
    }

    .portrait-photo {
      width: min(100%, 420px);
      aspect-ratio: 4 / 5;
      border-radius: 28px;
      object-fit: cover;
      border: 10px solid rgba(255, 255, 255, 0.7);
      box-shadow: 0 30px 60px rgba(105, 70, 79, 0.2);
      background: #f4e5dc;
    }

    .portrait-placeholder {
      width: min(100%, 420px);
      aspect-ratio: 4 / 5;
      border-radius: 28px;
      border: 10px solid rgba(255, 255, 255, 0.7);
      box-shadow: 0 30px 60px rgba(105, 70, 79, 0.2);
      background: radial-gradient(circle at 30% 20%, rgba(255, 255, 255, 0.8), transparent 20%),
        linear-gradient(160deg, #f6eae2 0%, #e9d0c8 50%, #d8b3af 100%);
      position: relative;
      overflow: hidden;
    }

    .portrait-placeholder svg {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
    }

    .badge-xv {
      position: absolute;
      right: 1rem;
      bottom: 1rem;
      width: 88px;
      height: 88px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background: rgba(255, 255, 255, 0.82);
      border: 1px solid rgba(141, 86, 97, 0.12);
      box-shadow: 0 10px 30px rgba(105, 70, 79, 0.12);
      font-family: "Playfair Display", serif;
      font-size: 1.5rem;
      color: var(--rose-deep);
      backdrop-filter: blur(8px);
    }

    .section {
      padding: 1rem 0 1.4rem;
    }

    .section-head {
      display: grid;
      gap: 0.6rem;
      margin-bottom: 1.2rem;
    }
    .section-head span {
      font-size: 0.74rem;
      letter-spacing: 0.24em;
      text-transform: uppercase;
      color: var(--rose-deep);
    }
    .section-head h2 {
      font-size: clamp(2.2rem, 6vw, 4rem);
      letter-spacing: -0.03em;
    }
    .section-head p {
      margin: 0;
      color: var(--muted);
      line-height: 1.8;
      max-width: 65ch;
    }

    .split {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1.2rem;
    }

    .panel {
      border-radius: var(--radius);
      padding: 1.35rem;
      border: 1px solid rgba(141, 86, 97, 0.1);
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.72), rgba(255, 255, 255, 0.5));
      box-shadow: var(--shadow);
      backdrop-filter: blur(14px);
    }

    .timeline {
      display: grid;
    }

    .timeline-item {
      display: grid;
      grid-template-columns: 74px 1fr;
      gap: 1rem;
      padding: 1rem 0;
      border-top: 1px solid var(--line);
    }
    .timeline-item:first-child {
      border-top: 0;
      padding-top: 0;
    }
    .timeline-item b {
      color: var(--rose-deep);
      font-size: 0.98rem;
    }
    .timeline-item strong {
      display: block;
      margin-bottom: 0.25rem;
      font-size: 1.06rem;
    }
    .timeline-item p {
      margin: 0;
      color: var(--muted);
      line-height: 1.7;
    }

    .rsvp-form {
      display: grid;
      gap: 1rem;
      margin-top: 0.4rem;
    }

    .field {
      display: grid;
      gap: 0.45rem;
    }
    .field label {
      font-size: 0.8rem;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--rose-deep);
    }
    .field input,
    .field textarea,
    .field select {
      width: 100%;
      border: 1px solid rgba(141, 86, 97, 0.14);
      background: rgba(255, 255, 255, 0.84);
      border-radius: 18px;
      padding: 1rem;
      outline: none;
      color: var(--ink);
      transition: border-color 0.2s ease, box-shadow 0.2s ease, transform 0.2s ease;
    }
    .field input:focus,
    .field textarea:focus,
    .field select:focus {
      border-color: rgba(184, 120, 133, 0.55);
      box-shadow: 0 0 0 4px rgba(184, 120, 133, 0.12);
      transform: translateY(-1px);
    }
    textarea {
      min-height: 120px;
      resize: vertical;
    }

    .success {
      display: none;
      padding: 1rem 1.1rem;
      border-radius: 18px;
      background: rgba(120, 178, 132, 0.12);
      border: 1px solid rgba(92, 153, 104, 0.22);
      color: #315f3b;
      font-weight: 600;
    }

    .photo-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1.2rem;
    }

    .qr-shell {
      display: grid;
      align-content: start;
      gap: 1rem;
    }

    .tag {
      width: max-content;
      padding: 0.55rem 0.85rem;
      border-radius: 999px;
      background: rgba(201, 165, 106, 0.14);
      color: #77582b;
      font-size: 0.84rem;
      font-weight: 700;
    }

    .qr-box {
      width: min(100%, 320px);
      aspect-ratio: 1;
      border-radius: 26px;
      padding: 1rem;
      display: grid;
      place-items: center;
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.86), rgba(255, 255, 255, 0.66));
      border: 1px solid rgba(141, 86, 97, 0.12);
    }

    .qr-box img {
      width: 100%;
      height: 100%;
      border-radius: 26px;
      object-fit: contain;
    }

    .map-card {
      position: relative;
      min-height: 420px;
      overflow: hidden;
      border-radius: var(--radius);
      border: 1px solid rgba(141, 86, 97, 0.1);
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.25), rgba(255, 255, 255, 0.12)),
        linear-gradient(135deg, #efe6e0 0%, #ead8cf 100%);
      box-shadow: var(--shadow);
    }

    .map-card svg {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
    }

    .map-pin {
      position: absolute;
      left: 57%;
      top: 44%;
      transform: translate(-50%, -100%);
      width: 72px;
      height: 72px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background: radial-gradient(circle at 35% 30%, #f9d7de, var(--rose) 60%, var(--rose-deep) 100%);
      border: 6px solid rgba(255, 255, 255, 0.8);
      box-shadow: 0 16px 34px rgba(141, 86, 97, 0.34);
      animation: floatPin 3s ease-in-out infinite;
    }

    .map-label {
      position: absolute;
      left: 57%;
      top: 48%;
      transform: translateX(-50%);
      background: rgba(255, 255, 255, 0.88);
      border: 1px solid rgba(141, 86, 97, 0.12);
      border-radius: 18px;
      padding: 0.85rem 1rem;
      min-width: min(300px, calc(100% - 2rem));
      text-align: center;
      box-shadow: var(--shadow);
      backdrop-filter: blur(10px);
    }

    @keyframes floatPin {
      0%,
      100% {
        transform: translate(-50%, -100%);
      }
      50% {
        transform: translate(-50%, -108%);
      }
    }

    .footer {
      padding: 2.2rem 0 3rem;
      text-align: center;
      color: var(--muted);
      font-size: 0.92rem;
    }

    .stagger {
      opacity: 0;
      transform: translateY(18px);
      animation: rise 0.9s cubic-bezier(0.22, 1, 0.36, 1) forwards;
    }
    .stagger:nth-child(1) {
      animation-delay: 0.08s;
    }
    .stagger:nth-child(2) {
      animation-delay: 0.18s;
    }
    .stagger:nth-child(3) {
      animation-delay: 0.3s;
    }
    .stagger:nth-child(4) {
      animation-delay: 0.42s;
    }
    .stagger:nth-child(5) {
      animation-delay: 0.54s;
    }

    @keyframes rise {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @media (min-width: 900px) {
      .nav-links {
        display: flex;
      }
      .hero-grid {
        grid-template-columns: 1.08fr 0.92fr;
      }
      .split {
        grid-template-columns: 1fr 0.95fr;
      }
      .photo-grid {
        grid-template-columns: 0.9fr 1.1fr;
      }
    }

    @media (max-width: 899px) {
      .hero-copy {
        min-height: auto;
      }
      .hero-art {
        min-height: 360px;
      }
      .map-label {
        left: 50%;
        top: 50%;
      }
      .map-pin {
        left: 50%;
        top: 43%;
      }
    }
  </style>
</head>
<body>
  <header class="topbar">
    <div class="container nav">
      <a href="#inicio" class="brand" aria-label="Inicio de la invitación">
        <span>Invitación digital</span>
        <strong>XV Años</strong>
      </a>
      <nav class="nav-links" aria-label="Navegación principal">
        <a href="#evento">Evento</a>
        <a href="#confirmar">Confirmar</a>
        <a href="#fotos">Fotos</a>
        <a href="#ubicacion">Ubicación</a>
      </nav>
    </div>
  </header>

  <main id="inicio">
    <section class="hero">
      <div class="container hero-shell reveal">
        <div class="hero-grid">
          <div class="hero-copy">
            <div class="eyebrow stagger">Con la bendición de Dios y de mi familia</div>
            <div class="script stagger">Mis XV años</div>
            <h1 class="stagger">María Fernanda</h1>
            <p class="lead stagger">
              Hay noches que se guardan para siempre en el corazón. Con inmensa alegría quiero compartir contigo
              este momento tan especial y celebrar juntos una velada llena de emoción, música y recuerdos inolvidables.
            </p>

            <div class="hero-data">
              <div class="data-block stagger">
                <small>Fecha</small>
                <div>
                  <strong>Sábado 19 de Septiembre, 2026</strong>
                  <span>Recepción a partir de las 7:00 PM</span>
                </div>
              </div>
              <div class="data-block stagger">
                <small>Lugar</small>
                <div>
                  <strong>Salón La Floresta</strong>
                  <span>Carr. Antigua Matehuala Km4</span>
                </div>
              </div>
            </div>

            <div class="cta-row stagger">
              <a class="btn btn-primary" href="https://docs.google.com/forms/d/e/1FAIpQLSeIcGvxEVDkqtHy1ztPy_zT_lzhEAHD8qdwwyrTA4VrODxc8g/viewform?usp=publish-editor" target="_blank" rel="noopener noreferrer">Confirmar asistencia</a>
              <a class="btn btn-secondary" href="#ubicacion">Ver ubicación</a>
            </div>
          </div>

          <div class="hero-art" aria-label="Espacio para foto de la quinceañera">
            <div class="frame"></div>
            <div class="portrait-wrap">
              <!-- Reemplaza esta imagen por tu foto propia -->
              <!-- <img class="portrait-photo" src="tu-foto.jpg" alt="Foto de María Fernanda"> -->

              <div class="portrait-placeholder">
                <svg viewBox="0 0 500 620" aria-hidden="true">
                  <defs>
                    <linearGradient id="g1" x1="0" x2="1">
                      <stop offset="0%" stop-color="#fff6f0" />
                      <stop offset="100%" stop-color="#ecd3ca" />
                    </linearGradient>
                    <linearGradient id="g2" x1="0" x2="1">
                      <stop offset="0%" stop-color="#c9a56a" />
                      <stop offset="100%" stop-color="#b87885" />
                    </linearGradient>
                  </defs>
                  <circle cx="252" cy="150" r="62" fill="#f0d4c8" />
                  <path d="M190 203c22-18 87-18 114 0 27 18 76 72 96 200 11 70-53 135-148 135S93 473 104 403c19-129 59-182 86-200z" fill="url(#g1)" />
                  <path d="M150 317c58 28 134 34 201 0" fill="none" stroke="url(#g2)" stroke-width="4" opacity=".8" />
                  <path d="M178 256c40 22 96 23 142 0" fill="none" stroke="#dbb8b1" stroke-width="3" />
                  <path d="M252 66l12 14 17 4-11 11 3 17-14-8-14 8 3-17-11-11 17-4z" fill="#c9a56a" />
                </svg>
                <div class="badge-xv">XV</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section" id="evento">
      <div class="container split">
        <article class="panel reveal">
          <div class="section-head">
            <span>Programa</span>
            <h2>Una noche inolvidable</h2>
            <p>Te esperamos para compartir cada instante de esta celebración preparada con cariño.</p>
          </div>

          <div class="timeline">
            <div class="timeline-item">
              <b>7:00 PM</b>
              <div>
                <strong>Recepción de invitados</strong>
                <p>Bienvenida y acceso al salón para comenzar la celebración.</p>
              </div>
            </div>
            <div class="timeline-item">
              <b>7:30 PM</b>
              <div>
                <strong>Ceremonia</strong>
                <p>Momento especial de agradecimiento y bendición.</p>
              </div>
            </div>
            <div class="timeline-item">
              <b>8:30 PM</b>
              <div>
                <strong>Cena</strong>
                <p>Disfrutaremos juntos una cena en honor a la festejada.</p>
              </div>
            </div>
            <div class="timeline-item">
              <b>9:30 PM</b>
              <div>
                <strong>Vals y brindis</strong>
                <p>Uno de los momentos más emotivos de la noche.</p>
              </div>
            </div>
            <div class="timeline-item">
              <b>10:00 PM</b>
              <div>
                <strong>Fiesta</strong>
                <p>Música, baile y recuerdos que quedarán para siempre.</p>
              </div>
            </div>
          </div>
        </article>

        <article class="panel reveal" id="confirmar">
          <div class="section-head">
            <span>RSVP</span>
            <h2>Confirmar asistencia</h2>
            <p>Por favor confirma tu asistencia antes del 1 de septiembre para reservar tu lugar.</p>
          </div>

          <form class="rsvp-form" onsubmit="window.open('https://docs.google.com/forms/d/e/1FAIpQLSeIcGvxEVDkqtHy1ztPy_zT_lzhEAHD8qdwwyrTA4VrODxc8g/viewform?usp=publish-editor'); return false;">
            <button type="submit" class="btn btn-primary">Abrir Formulario de Confirmación</button>
          </form>
        </article>
      </div>
    </section>

    <section class="section" id="fotos">
      <div class="container photo-grid">
        <article class="panel qr-shell reveal">
          <div class="section-head" style="margin-bottom: 0.2rem">
            <span>Recuerdos</span>
            <h2>Comparte tus fotos</h2>
          </div>
          <div class="tag">Escanea el código el día del evento</div>

          <div class="qr-box" aria-label="Código QR para confirmar asistencia">
            <img src="https://api.qrserver.com/v1/create-qr-code/?size=240x240&data=https://docs.google.com/forms/d/e/1FAIpQLSeIcGvxEVDkqtHy1ztPy_zT_lzhEAHD8qdwwyrTA4VrODxc8g/viewform?usp=publish-editor" alt="Código QR para confirmar asistencia" />
          </div>
        </article>

        <article class="panel reveal">
          <div class="section-head">
            <span>Álbum compartido</span>
            <h2>Guardemos juntos cada recuerdo</h2>
            <p>
              El día del evento podrás escanear este código para subir fotos y videos a un álbum compartido.
              Reemplaza el enlace en el QR con el de tu plataforma preferida (Google Photos, Drive, Dropbox, etc.).
            </p>
          </div>

          <div class="cta-row" style="margin-top: 0.5rem">
            <a class="btn btn-secondary" href="#" onclick="alert('Aquí puedes enlazar el álbum compartido real.'); return false;">Abrir álbum</a>
          </div>
        </article>
      </div>
    </section>

    <section class="section" id="ubicacion">
      <div class="container">
        <div class="section-head reveal">
          <span>Cómo llegar</span>
          <h2>Salón La Floresta</h2>
          <p>Carr. Antigua Matehuala Km4</p>
        </div>

        <div class="map-card reveal" aria-label="Mapa ilustrado de la ubicación">
          <svg viewBox="0 0 1200 600" preserveAspectRatio="none" role="img" aria-label="Mapa decorativo">
            <rect width="1200" height="600" fill="transparent" />
            <g opacity=".7">
              <path d="M0 145 C180 120, 240 198, 420 170 S760 90, 1200 140" fill="none" stroke="#ffffff" stroke-width="42" stroke-linecap="round" />
              <path d="M90 0 C150 160, 170 280, 110 600" fill="none" stroke="#ffffff" stroke-width="28" stroke-linecap="round" />
              <path d="M380 0 C455 150, 470 340, 410 600" fill="none" stroke="#ffffff" stroke-width="22" stroke-linecap="round" />
              <path d="M720 0 C780 150, 840 310, 790 600" fill="none" stroke="#ffffff" stroke-width="30" stroke-linecap="round" />
              <path d="M1010 0 C950 140, 960 300, 1060 600" fill="none" stroke="#ffffff" stroke-width="24" stroke-linecap="round" />
              <path d="M0 430 C220 400, 280 480, 480 452 S930 362, 1200 435" fill="none" stroke="#ffffff" stroke-width="34" stroke-linecap="round" />
            </g>
            <g opacity=".9">
              <rect x="205" y="205" width="72" height="58" rx="8" fill="#dbc3b6" />
              <rect x="294" y="300" width="82" height="68" rx="10" fill="#e6d0c4" />
              <rect x="548" y="112" width="96" height="80" rx="10" fill="#d8bfb3" />
              <rect x="880" y="322" width="78" height="64" rx="10" fill="#e2cdc2" />
              <rect x="986" y="118" width="102" height="88" rx="10" fill="#d6bbaf" />
            </g>
          </svg>

          <div class="map-pin" aria-hidden="true">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none">
              <path d="M12 22s7-6.2 7-12a7 7 0 1 0-14 0c0 5.8 7 12 7 12Z" fill="white" />
              <circle cx="12" cy="10" r="3.2" fill="#b87885" />
            </svg>
          </div>

          <div class="map-label">
            <strong>Salón La Floresta</strong>
            <div style="color: var(--muted)">Carr. Antigua Matehuala Km4</div>
          </div>
        </div>

        <div class="cta-row reveal">
          <a class="btn btn-primary" href="https://maps.app.goo.gl/5dtMULV19pxriPjZ9" target="_blank" rel="noopener noreferrer">Abrir en Google Maps</a>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">Hecho con amor para una celebración inolvidable · XV Años de María Fernanda</div>
  </footer>

  <script>
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach((entry) => {
          if (entry.isIntersecting) {
            entry.target.classList.add("visible");
          }
        });
      },
      { threshold: 0.16 }
    );

    document.querySelectorAll(".reveal").forEach((el) => observer.observe(el));
  </script>
</body>
</html>
