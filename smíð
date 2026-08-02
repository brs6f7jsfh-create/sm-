<!DOCTYPE html>
<html lang="is">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Smíð — öpp smíðuð af alúð</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,380;0,9..144,500;0,9..144,600;1,9..144,420&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>

  :root{
    --paper: #F4EFE5;
    --paper-warm: #FBF7EF;
    --ink: #2C2620;
    --ink-soft: #5B5245;
    --moss: #5F7A5C;
    --moss-deep: #445C43;
    --brass: #B98A4A;
    --line: rgba(44,38,32,0.14);
  }

  *{ margin:0; padding:0; box-sizing:border-box; }

  html{ scroll-behavior:smooth; }

  body{
    background: var(--paper);
    color: var(--ink);
    font-family: 'Inter', sans-serif;
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    overflow-x: hidden;
  }

  body::before{
    content:"";
    position: fixed;
    inset:0;
    pointer-events:none;
    background-image:
      radial-gradient(circle at 1px 1px, rgba(44,38,32,0.045) 1px, transparent 0);
    background-size: 22px 22px;
    z-index: 0;
  }

  .wrap{
    max-width: 920px;
    margin: 0 auto;
    padding: 0 32px;
    position: relative;
    z-index: 1;
  }

  /* ---------- NAV ---------- */
  nav{
    position: sticky;
    top: 0;
    z-index: 20;
    background: rgba(244,239,229,0.86);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid var(--line);
  }
  nav .wrap{
    display:flex;
    align-items:center;
    justify-content:space-between;
    height: 76px;
  }
  .logo{
    font-family:'Fraunces', serif;
    font-weight: 600;
    font-size: 1.35rem;
    letter-spacing: -0.01em;
    color: var(--ink);
    text-decoration:none;
  }
  .logo em{
    font-style: italic;
    font-weight: 420;
    color: var(--moss-deep);
  }
  .nav-cta{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.8rem;
    letter-spacing: 0.02em;
    color: var(--ink);
    text-decoration:none;
    border: 1px solid var(--ink);
    padding: 9px 18px;
    border-radius: 999px;
    transition: all 0.25s ease;
    white-space: nowrap;
  }
  .nav-cta:hover{
    background: var(--ink);
    color: var(--paper-warm);
  }

  /* ---------- HERO ---------- */
  header.hero{
    padding: 100px 0 80px;
    position: relative;
  }
  .eyebrow{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.78rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: var(--moss-deep);
    display:flex;
    align-items:center;
    gap: 10px;
    margin-bottom: 28px;
  }
  .eyebrow::before{
    content:"";
    width: 26px;
    height: 1px;
    background: var(--brass);
  }
  h1{
    font-family:'Fraunces', serif;
    font-weight: 500;
    font-size: clamp(2.6rem, 6vw, 4.6rem);
    line-height: 1.04;
    letter-spacing: -0.02em;
    max-width: 780px;
    color: var(--ink);
  }
  h1 .accent{
    font-style: italic;
    font-weight: 420;
    color: var(--moss-deep);
  }
  .hero-sub{
    margin-top: 26px;
    font-size: 1.18rem;
    color: var(--ink-soft);
    max-width: 540px;
    font-weight: 400;
  }
  .hero-actions{
    margin-top: 40px;
    display:flex;
    gap: 16px;
    align-items:center;
    flex-wrap: wrap;
  }
  .btn-primary{
    font-family:'Inter', sans-serif;
    font-weight: 600;
    font-size: 0.98rem;
    background: var(--moss-deep);
    color: var(--paper-warm);
    text-decoration:none;
    padding: 15px 30px;
    border-radius: 999px;
    display:inline-flex;
    align-items:center;
    gap: 10px;
    box-shadow: 0 1px 0 rgba(0,0,0,0.05);
    transition: transform 0.2s ease, background 0.2s ease;
  }
  .btn-primary:hover{
    background: var(--moss);
    transform: translateY(-2px);
  }
  .btn-secondary{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.85rem;
    color: var(--ink-soft);
    text-decoration: none;
    border-bottom: 1px solid var(--line);
    padding-bottom: 2px;
    transition: color 0.2s, border-color 0.2s;
  }
  .btn-secondary:hover{
    color: var(--ink);
    border-color: var(--ink);
  }

  /* ---------- JOINT SIGNATURE ---------- */
  .joint-wrap{
    margin-top: 64px;
    display:flex;
    align-items:center;
    gap: 28px;
  }
  .joint-svg{ width: 190px; height: auto; flex-shrink:0; }
  .joint-line{
    fill:none;
    stroke: var(--moss-deep);
    stroke-width: 2.4;
    stroke-linecap: round;
    stroke-linejoin: round;
    stroke-dasharray: 620;
    stroke-dashoffset: 620;
    animation: draw 2.1s ease forwards 0.4s;
  }
  .joint-line.brass{ stroke: var(--brass); }
  @keyframes draw{ to{ stroke-dashoffset: 0; } }
  .joint-caption{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.78rem;
    color: var(--ink-soft);
    line-height: 1.7;
    max-width: 220px;
  }
  @media (prefers-reduced-motion: reduce){
    .joint-line{ animation: none; stroke-dashoffset: 0; }
  }

  /* ---------- SECTION SHARED ---------- */
  section{ padding: 88px 0; border-top: 1px solid var(--line); }
  .section-head{ max-width: 560px; margin-bottom: 56px; }
  .section-label{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.78rem;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    color: var(--brass);
    margin-bottom: 14px;
    display:block;
  }
  h2{
    font-family:'Fraunces', serif;
    font-weight: 500;
    font-size: clamp(1.8rem, 3.4vw, 2.5rem);
    letter-spacing: -0.01em;
    color: var(--ink);
  }
  .section-head p{
    margin-top: 16px;
    color: var(--ink-soft);
    font-size: 1.05rem;
  }

  /* ---------- WHAT I BUILD ---------- */
  .craft-grid{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--line);
    border: 1px solid var(--line);
    border-radius: 18px;
    overflow: hidden;
  }
  .craft-card{
    background: var(--paper-warm);
    padding: 38px 30px;
    transition: background 0.25s ease;
  }
  .craft-card:hover{ background: #F6F1E4; }
  .craft-mark{
    font-family:'Fraunces', serif;
    font-style: italic;
    font-size: 1.05rem;
    color: var(--moss-deep);
    margin-bottom: 18px;
    display:block;
  }
  .craft-card h3{
    font-family:'Fraunces', serif;
    font-weight: 500;
    font-size: 1.3rem;
    margin-bottom: 10px;
    color: var(--ink);
  }
  .craft-card p{
    font-size: 0.95rem;
    color: var(--ink-soft);
  }

  @media (max-width: 760px){
    .craft-grid{ grid-template-columns: 1fr; }
  }

  /* ---------- APPROACH ---------- */
  .approach{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
    align-items: start;
  }
  .approach-copy p{
    color: var(--ink-soft);
    font-size: 1.05rem;
    margin-bottom: 18px;
  }
  .approach-copy strong{
    color: var(--ink);
    font-weight: 600;
  }
  .value-list{ list-style:none; }
  .value-list li{
    padding: 20px 0;
    border-top: 1px solid var(--line);
    display:flex;
    gap: 18px;
    align-items: baseline;
  }
  .value-list li:last-child{ border-bottom: 1px solid var(--line); }
  .value-list .v-mark{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.78rem;
    color: var(--brass);
    flex-shrink:0;
    width: 26px;
  }
  .value-list h4{
    font-family:'Fraunces', serif;
    font-weight: 500;
    font-size: 1.08rem;
    color: var(--ink);
    margin-bottom: 4px;
  }
  .value-list span.desc{
    font-size: 0.92rem;
    color: var(--ink-soft);
  }

  @media (max-width: 760px){
    .approach{ grid-template-columns: 1fr; gap: 32px; }
  }

  /* ---------- CONTACT ---------- */
  .contact{
    text-align: center;
    padding: 100px 0 120px;
  }
  .contact .section-label{ display:flex; justify-content:center; }
  .contact h2{
    max-width: 620px;
    margin: 0 auto;
    font-size: clamp(2rem, 4.2vw, 3rem);
  }
  .contact p.lead{
    max-width: 480px;
    margin: 20px auto 44px;
    color: var(--ink-soft);
    font-size: 1.08rem;
  }
  .email-card{
    display:inline-flex;
    align-items:center;
    gap: 16px;
    background: var(--ink);
    color: var(--paper-warm);
    padding: 22px 30px;
    border-radius: 16px;
    text-decoration:none;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
    box-shadow: 0 10px 30px -12px rgba(44,38,32,0.35);
  }
  .email-card:hover{
    transform: translateY(-3px);
    box-shadow: 0 16px 36px -12px rgba(44,38,32,0.45);
  }
  .email-icon{
    width: 40px; height: 40px;
    border-radius: 10px;
    background: var(--moss);
    display:flex; align-items:center; justify-content:center;
    flex-shrink:0;
  }
  .email-text{ text-align:left; }
  .email-text .label{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.72rem;
    color: #C9BFA9;
    letter-spacing: 0.04em;
    text-transform: uppercase;
  }
  .email-text .addr{
    font-family:'Fraunces', serif;
    font-size: 1.15rem;
    font-weight: 500;
  }
  .contact-note{
    margin-top: 28px;
    font-family:'JetBrains Mono', monospace;
    font-size: 0.8rem;
    color: var(--ink-soft);
  }

  /* ---------- FOOTER ---------- */
  footer{
    border-top: 1px solid var(--line);
    padding: 32px 0;
  }
  footer .wrap{
    display:flex;
    justify-content:space-between;
    align-items:center;
    flex-wrap: wrap;
    gap: 12px;
  }
  footer .logo{ font-size: 1.05rem; }
  footer .foot-note{
    font-family:'JetBrains Mono', monospace;
    font-size: 0.75rem;
    color: var(--ink-soft);
  }

  a:focus-visible, button:focus-visible{
    outline: 2px solid var(--moss-deep);
    outline-offset: 3px;
  }
</style>
</head>
<body>

<nav>
  <div class="wrap">
    <a href="#top" class="logo">Sm<em>í</em>ð</a>
    <a class="nav-cta" href="#samband">Senda fyrirspurn</a>
  </div>
</nav>

<div id="top"></div>

<header class="hero">
  <div class="wrap">
    <span class="eyebrow">Hugbúnaðarsmíði fyrir fyrirtæki</span>
    <h1>Öpp sem eru <span class="accent">smíðuð</span>, ekki bara sett saman.</h1>
    <p class="hero-sub">Ég hanna og byggi vefforrit fyrir fyrirtæki sem vilja lausn sem hentar þeim nákvæmlega — ekki staðlað box með of mörgum eða of fáum eiginleikum.</p>

    <div class="hero-actions">
      <a href="#samband" class="btn-primary">
        Segðu mér frá verkefninu
        <span>→</span>
      </a>
      <a href="#hvad" class="btn-secondary">Sjá hvað ég geri</a>
    </div>

    <div class="joint-wrap">
      <svg class="joint-svg" viewBox="0 0 200 90" fill="none">
        <path class="joint-line" d="M10 20 L70 20 L70 45 L100 45 L100 20 L130 20" />
        <path class="joint-line brass" d="M10 70 L70 70 L70 45 L100 45 L100 70 L130 70" />
        <path class="joint-line" d="M10 20 L10 70" style="stroke-dasharray:60; stroke-dashoffset:60; animation-delay:1.6s;" />
        <path class="joint-line brass" d="M130 20 L130 70" style="stroke-dasharray:60; stroke-dashoffset:60; animation-delay:1.6s;" />
      </svg>
      <p class="joint-caption">Tvær hliðar sem falla saman — þín hugmynd og mín útfærsla. Þannig verða góð öpp til.</p>
    </div>
  </div>
</header>

<section id="hvad">
  <div class="wrap">
    <div class="section-head">
      <span class="section-label">Hvað ég geri</span>
      <h2>Frá hugmynd á servíettu að appi í notkun.</h2>
      <p>Hvert verkefni er smíðað frá grunni utan um þarfir fyrirtækisins — engar afgangslausnir.</p>
    </div>

    <div class="craft-grid">
      <div class="craft-card">
        <span class="craft-mark">01</span>
        <h3>Innri kerfi</h3>
        <p>Verkfæri og mælaborð sem starfsfólkið þitt notar á hverjum degi til að vinna hraðar og skipulagðar.</p>
      </div>
      <div class="craft-card">
        <span class="craft-mark">02</span>
        <h3>Viðskiptavinagáttir</h3>
        <p>Vefsvæði þar sem viðskiptavinir þínir geta pantað, fylgst með stöðu eða séð sín gögn.</p>
      </div>
      <div class="craft-card">
        <span class="craft-mark">03</span>
        <h3>Sérsmíðuð vefforrit</h3>
        <p>Lausnir sem passa ekki í fyrirfram gefið box — byggðar frá grunni utan um þinn rekstur.</p>
      </div>
    </div>
  </div>
</section>

<section id="um-mig">
  <div class="wrap">
    <div class="approach">
      <div class="approach-copy">
        <span class="section-label">Hver stendur á bak við Smíð</span>
        <h2 style="margin-bottom:22px;">Ágúst Þór Kjartansson.</h2>
        <p>Ég er á <strong>viðskipta- og hagfræðibraut í Flensborg</strong> og hef samhliða náminu verið að læra að forrita og smíða vefforrit sjálfur. Áhuginn kviknaði af því að skilja bæði hliðarnar — hvernig fyrirtæki hugsa og hvernig lausnin á bak við tjöldin virkar í raun og veru.</p>
        <p>Þessi blanda þýðir að ég tala ekki bara kóða — ég skil líka reksturinn, viðskiptalíkanið og hvað skiptir fyrirtæki raunverulega máli þegar vefforrit er smíðað.</p>
      </div>

      <ul class="value-list">
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Nám</h4>
            <span class="desc">Viðskipta- og hagfræðibraut, Flensborg.</span>
          </div>
        </li>
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Áhugi</h4>
            <span class="desc">Að byggja vefforrit sem leysa raunveruleg vandamál fyrirtækja.</span>
          </div>
        </li>
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Nálgun</h4>
            <span class="desc">Skilningur á rekstri og tækni í senn — ekki bara annað hvort.</span>
          </div>
        </li>
      </ul>
    </div>
  </div>
</section>

<section id="nalgun">
  <div class="wrap">
    <div class="approach">
      <div class="approach-copy">
        <span class="section-label">Vinnulagið</span>
        <h2 style="margin-bottom:22px;">Handverk, ekki færibandavinna.</h2>
        <p>Ég tek að mér <strong>fá verkefni í einu</strong> svo hvert þeirra fái þá athygli sem það á skilið. Þú talar beint við þann sem skrifar kóðann — engir milliliðir, engin týnd skilaboð.</p>
        <p>Markmiðið er ekki bara app sem virkar á opnunardegi, heldur eitthvað sem þolir álag, vöxt og árin sem á eftir koma.</p>
      </div>

      <ul class="value-list">
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Beint samtal</h4>
            <span class="desc">Þú hittir og talar við mig, ekki söluteymi.</span>
          </div>
        </li>
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Sniðið að þér</h4>
            <span class="desc">Lausnin er byggð utan um þinn rekstur, ekki öfugt.</span>
          </div>
        </li>
        <li>
          <span class="v-mark">◆</span>
          <div>
            <h4>Til framtíðar</h4>
            <span class="desc">Kóði sem er auðvelt að byggja ofan á síðar.</span>
          </div>
        </li>
      </ul>
    </div>
  </div>
</section>

<section class="contact" id="samband">
  <div class="wrap">
    <span class="section-label">Eigum við að spjalla?</span>
    <h2>Segðu mér frá því sem þig vantar að byggja.</h2>
    <p class="lead">Sendu mér línu með stuttri lýsingu á verkefninu — ég svara yfirleitt innan sólarhrings.</p>

    <a class="email-card" href="mailto:agustthorpk@gmail.com">
      <span class="email-icon">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#FBF7EF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="2" y="4" width="20" height="16" rx="2"></rect>
          <path d="m22 6-10 7L2 6"></path>
        </svg>
      </span>
      <span class="email-text">
        <span class="label">Sendu tölvupóst</span><br>
        <span class="addr">agustthorpk@gmail.com</span>
      </span>
    </a>

    <p class="contact-note">— eða settu bara „Smíð" í efnislínuna, ég finn það.</p>
  </div>
</section>

<footer>
  <div class="wrap">
    <a href="#top" class="logo">Sm<em>í</em>ð</a>
    <span class="foot-note">© 2026 · Hannað og smíðað á Íslandi</span>
  </div>
</footer>

</body>
</html>
