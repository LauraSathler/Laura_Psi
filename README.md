<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Laura Sathler | Psicóloga (CRP 04/30866)</title>
  <meta name="description" content="Psicoterapia humanista‑existencial com acolhimento e presença. Agende sua sessão com Laura Sathler (CRP 04/30866).">
  <meta name="theme-color" content="#f6efe9">
  <link rel="icon" href="Logomarca.png">
  <style>
    :root{
      /* Paleta já usada no seu site */
      --bg:#f6efe9; --bg2:#fbf8f5; --card:#ffffff;
      --text:#2b2b2b; --muted:#6b6b6b;
      --accent:#79a6a3; --accent-2:#e2d6cc;
      --radius:18px; --shadow:0 10px 24px rgba(0,0,0,.08);
      --maxw:1080px;
      --s1:.5rem; --s2:.75rem; --s3:1rem; --s4:1.5rem; --s5:2rem; --s6:3rem;
      --header-h: 88px;              /* atualizado por JS conforme tamanho do topo */
      --header-bg: rgba(246,239,233,.0);  /* transparente no topo */
      --header-bg-solid: rgba(246,239,233,.92); /* sólido ao rolar */
    }

    *,*::before,*::after{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0; font-family:system-ui,-apple-system,"Segoe UI",Roboto,Arial,sans-serif;
      color:var(--text); line-height:1.6; overflow-x:hidden;
      background:linear-gradient(180deg,var(--bg),var(--bg2) 40%,var(--bg) 100%);
      -webkit-font-smoothing:antialiased; text-rendering:optimizeLegibility;
    }
    h1,h2,h3{line-height:1.2; margin:0 0 var(--s2)}
    h1{font-size:clamp(2rem,4vw,3rem)}
    h2{font-size:clamp(1.5rem,3vw,2rem)}
    p{margin:0 0 var(--s3)}
    a{color:var(--accent); text-decoration:none}
    a:hover{text-decoration:underline}
    .container{width:min(var(--maxw),92vw); margin-inline:auto}

    /* ====== HEADER ====== */
    header{
      position:fixed; inset:0 0 auto 0; z-index:30;
      background:var(--header-bg);
      backdrop-filter:saturate(160%) blur(8px);
      transition: background .25s ease, box-shadow .25s ease;
      border-bottom:1px solid transparent;
    }
    header.scrolled{
      background:var(--header-bg-solid);
      border-bottom-color:#eadfd6;
      box-shadow:0 6px 18px rgba(0,0,0,.06);
    }
    .nav{
      min-height:72px; padding:.7rem 0;
      display:flex; align-items:center; justify-content:space-between; gap:.8rem; flex-wrap:wrap;
    }
    .brand{display:flex; align-items:center; gap:.75rem; min-width:240px}
    .brand-logo{height:60px; width:auto; display:block}
    .brand-text{display:flex; flex-direction:column}
    .brand-text b{font-weight:800}
    .brand-text small{color:var(--muted)}

    .menu-toggle{display:none}
    .menu-btn{display:none; align-items:center; gap:.5rem; font-weight:700;
      padding:.5rem .75rem; border-radius:10px; cursor:pointer}
    nav ul{display:flex; gap:.9rem; list-style:none; margin:0; padding:0}
    nav a{display:inline-block; padding:.45rem .7rem; border-radius:10px; font-weight:600}
    nav a:hover{background:var(--accent-2); text-decoration:none}

    /* Para que as âncoras não fiquem escondidas atrás do topo */
    section{scroll-margin-top:calc(var(--header-h) + 12px); padding:var(--s6) 0}
    .card{background:var(--card); border:1px solid #eee4da; border-radius:var(--radius); box-shadow:var(--shadow); padding:var(--s4)}
    .grid-2{display:grid; grid-template-columns:1fr 1fr; gap:var(--s4); align-items:center}
    .muted{color:var(--muted)}

    /* ====== HERO (capa) ====== */
    .hero{
      min-height:84svh; display:grid; place-items:center;
      background:
        linear-gradient(180deg, rgba(10,10,10,.28), rgba(10,10,10,.15) 35%, rgba(246,239,233,.75)),
        url("Terapeuta-Paciente.png") center/cover no-repeat;
      color:#223; text-align:left;
      padding-top:calc(var(--header-h) + var(--s4)); /* evita sobrepor o topo */
    }
    .hero .wrap{width:min(var(--maxw),92vw); display:grid; grid-template-columns:1.1fr .9fr; gap:var(--s5); align-items:center}
    .hero h1{color:#213; text-shadow:0 2px 18px rgba(255,255,255,.65)}
    .hero p{color:#2b2b2b}
    .cta{display:flex; gap:.7rem; flex-wrap:wrap; margin-top:var(--s2)}
    .btn{display:inline-flex; align-items:center; justify-content:center; gap:.45rem; padding:.9rem 1.05rem; border-radius:12px; font-weight:700; border:1px solid transparent; box-shadow:var(--shadow); cursor:pointer}
    .btn-primary{background:var(--accent); color:#fff}
    .btn-primary:hover{filter:brightness(.95); text-decoration:none}
    .btn-ghost{background:#fff; border:1px solid #e8e0d7}

    /* ====== IMAGENS ====== */
    .img-cover{width:100%; height:auto; border-radius:var(--radius); box-shadow:var(--shadow); object-fit:cover}
    .portrait-circle{width:300px; height:300px; border-radius:50%; object-fit:cover; box-shadow:var(--shadow); display:block; margin:auto}

    /* ====== QUANDO PROCURAR ====== */
    .why{display:grid; grid-template-columns:repeat(2,1fr); gap:1rem; margin-top:.75rem}
    .why li{background:#fff; border:1px solid #eee4da; border-radius:14px; padding:.9rem 1rem}

    /* ====== WHATSAPP FLUTUANTE ====== */
    .wa-fab{
      position:fixed; right:16px; bottom:16px; z-index:40;
      background:#25D366; color:#fff; border-radius:999px; padding:.85rem 1.05rem; font-weight:800; box-shadow:0 12px 28px rgba(0,0,0,.18);
    }
    .wa-fab:hover{filter:brightness(.95); text-decoration:none}

    /* ====== RODAPÉ ====== */
    footer{padding:2rem 0; border-top:1px solid #eadfd6; color:var(--muted); text-align:center}

    /* ====== MOBILE ====== */
    @media (max-width:900px){
      .grid-2{grid-template-columns:1fr}
      .hero .wrap{grid-template-columns:1fr; gap:var(--s4)}
      .portrait-circle{width:240px; height:240px}
      .card{padding:var(--s3)}
      .brand-logo{height:52px}
      /* Menu mobile em fluxo (não sobrepõe conteúdo) */
      .menu-btn{display:flex}
      nav{width:100%}
      nav ul{flex-direction:column; padding:.6rem 0}
      .menu-toggle:not(:checked) + .menu-btn + nav{display:none}
      .menu-toggle:checked + .menu-btn + nav{display:block}
    }
  </style>
</head>
<body>
  <!-- ====== HEADER ====== -->
  <header id="topbar">
    <div class="container nav">
      <div class="brand" aria-label="Identidade do site">
        <img src="Logomarca.png" alt="Logomarca Laura Sathler" class="brand-logo"
             onerror="this.onerror=null;this.src='Logomarca.jpeg'">
        <div class="brand-text">
          <b>Laura Sathler</b>
          <small>Psicóloga · CRP 04/30866</small>
        </div>
      </div>

      <input id="menu" class="menu-toggle" type="checkbox" />
      <label for="menu" class="menu-btn" aria-label="Abrir menu">☰ Menu</label>

      <nav aria-label="principal">
        <ul>
          <li><a href="#psicoterapia">O que é Psicoterapia</a></li>
          <li><a href="#sobre">Sobre mim</a></li>
          <li><a href="#quando">Quando procurar</a></li>
          <li><a href="#contato">Contato</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Empurra o conteúdo para baixo do topo fixo -->
  <div style="height:var(--header-h)"></div>

  <!-- ====== HERO ====== -->
  <section class="hero" id="inicio">
    <div class="wrap">
      <div>
        <h1>Cuidado psicológico com acolhimento e presença</h1>
        <p>Um espaço seguro para falar sobre o que você sente e pensa — no seu tempo e do seu jeito.</p>
        <div class="cta">
          <a class="btn btn-primary" href="https://wa.me/5531991593800" target="_blank" rel="noopener">📱 Agendar no WhatsApp</a>
          <a class="btn btn-ghost" href="#psicoterapia">Saiba mais</a>
        </div>
      </div>
      <div><!-- coluna vazia (hero centrado/balanceado) --></div>
    </div>
  </section>

  <main>
    <!-- ====== O QUE É PSICOTERAPIA ====== -->
    <section id="psicoterapia">
      <div class="container grid-2">
        <div class="card text">
          <h2>O que é Psicoterapia?</h2>
          <p>A psicoterapia é um espaço de escuta e reflexão onde você pode se expressar com liberdade, sem julgamentos. É um processo que convida ao autoconhecimento, ajuda a reconhecer sua história, acolher as dores, cuidar de si e fortalecer aquilo que traz sentido e vitalidade à vida.</p>
          <p>Nem sempre é simples — exige presença e, às vezes, coragem para olhar para dentro. Ao mesmo tempo, é um lugar de encontro e clareza, que favorece escolhas mais conscientes e formas mais autênticas de viver.</p>
          <p>Cada conversa abre possibilidades para se escutar, se compreender e se posicionar no mundo, no seu tempo e do seu jeito.</p>
        </div>
        <div class="media">
          <img class="img-cover" src="Terapeuta-Paciente.png" alt="Sessão de psicoterapia" loading="lazy" decoding="async">
        </div>
      </div>
    </section>

    <!-- ====== SOBRE MIM ====== -->
    <section id="sobre">
      <div class="container grid-2">
        <div class="media" style="text-align:center">
          <img class="portrait-circle" src="Laura.jpeg" alt="Foto de Laura Sathler" loading="lazy" decoding="async">
        </div>
        <div class="card text">
          <h2>Sobre mim</h2>
          <p>Sou <strong>Laura Sathler</strong>, psicóloga (CRP 04/30866) formada pela PUC Minas, com mais de 10 anos de experiência clínica e especialização em <strong>Avaliação e Diagnóstico Psicológico</strong>. Minha prática se baseia na abordagem <strong>humanista‑existencial</strong>, valorizando a singularidade de cada pessoa e a construção de um espaço de presença, acolhimento e diálogo genuíno.</p>
          <p>Atendo questões como ansiedade, tristeza persistente, vazio existencial, estresse e burnout, autoestima e desafios nos relacionamentos. O objetivo é favorecer clareza, fortalecimento emocional e novas perspectivas para uma vida mais coerente e autêntica.</p>
        </div>
      </div>
    </section>

    <!-- ====== QUANDO PROCURAR ====== -->
    <section id="quando">
      <div class="container card">
        <h2>Quando procurar terapia</h2>
        <ul class="why">
          <li>Ansiedade, tristeza ou cansaço emocional frequentes.</li>
          <li>Dificuldade para lidar com mudanças, perdas ou transições.</li>
          <li>Sentimento de vazio ou falta de sentido.</li>
          <li>Conflitos recorrentes nos relacionamentos ou no trabalho.</li>
          <li>Desejo de se conhecer melhor e viver com mais autenticidade.</li>
          <li>Vontade de desenvolver recursos internos para enfrentar desafios.</li>
        </ul>
        <p class="muted" style="margin-top:.5rem">Cuidar da saúde emocional é um investimento em qualidade de vida.</p>
      </div>
    </section>

    <!-- ====== CONTATO ====== -->
    <section id="contato">
      <div class="container card" style="text-align:center">
        <h2>Agende sua sessão</h2>
        <p>Se sentir que este é um bom momento para começar, estou à disposição para conversarmos.</p>
        <div class="cta" style="justify-content:center">
          <a class="btn btn-primary" href="https://wa.me/5531991593800" target="_blank" rel="noopener">📱 Falar no WhatsApp</a>
          <a class="btn btn-ghost" href="mailto:Laurasathler@yahoo.com.br">📧 Enviar e‑mail</a>
        </div>
        <p style="margin-top:var(--s2)"><strong>Telefone:</strong> +55 31 99159‑3800 · <strong>E‑mail:</strong> <a href="mailto:Laurasathler@yahoo.com.br">Laurasathler@yahoo.com.br</a></p>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">© <span id="year"></span> Laura Sathler · Psicóloga · CRP 04/30866</div>
  </footer>

  <!-- WhatsApp flutuante -->
  <a class="wa-fab" href="https://wa.me/5531991593800" target="_blank" rel="noopener" aria-label="Abrir conversa no WhatsApp">WhatsApp</a>

  <script>
    // Atualiza ano no rodapé
    document.getElementById('year').textContent = new Date().getFullYear();

    // Torna o topo sólido quando rola
    const topbar = document.getElementById('topbar');
    const updateHeader = () => {
      const scrolled = window.scrollY > 8;
      topbar.classList.toggle('scrolled', scrolled);
      // atualiza variável --header-h conforme altura real do topo
      const h = topbar.getBoundingClientRect().height;
      document.documentElement.style.setProperty('--header-h', h + 'px');
    };
    updateHeader();
    window.addEventListener('scroll', updateHeader, {passive:true});
    window.addEventListener('resize', updateHeader);

    // Fecha menu mobile ao clicar
    document.querySelectorAll('nav a').forEach(a=>{
      a.addEventListener('click',()=>{ const cb=document.getElementById('menu'); if(cb) cb.checked=false; });
    });

    // Fallback favicon se PNG não existir
    (function(){
      const link = document.querySelector('link[rel="icon"]');
      const test = new Image();
      test.onerror = ()=> link.href = 'Logomarca.jpeg';
      test.src = link.href;
    })();

    // (Opcional) Forçar HTTPS enquanto o certificado não está ativo
    // if (location.protocol === 'http:') {
    //   location.replace('https://' + location.host + location.pathname + location.search + location.hash);
    // }
  </script>
</body>
</html>
