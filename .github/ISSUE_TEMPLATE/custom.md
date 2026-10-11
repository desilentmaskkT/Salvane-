---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#10100f">
  <title>SALVANE — Faith in Every Thread</title>
  <meta name="description" content="Salvane is faith-driven streetwear built around belief, identity and purpose.">
  <style>
    :root {
      --black: #10100f;
      --cream: #eeeae1;
      --muted: #a6a39b;
      --line: rgba(238,234,225,.2);
      --red: #873d35;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      background: var(--black);
      color: var(--cream);
      font-family: Arial, Helvetica, sans-serif;
    }
    a { color: inherit; text-decoration: none; }
    button, a { -webkit-tap-highlight-color: transparent; }
    .announcement {
      padding: 10px 15px;
      text-align: center;
      border-bottom: 1px solid var(--line);
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }
    header {
      height: 76px;
      padding: 0 6%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid var(--line);
    }
    .logo {
      font-size: 23px;
      font-weight: 900;
      letter-spacing: 5px;
    }
    nav { display: flex; gap: 27px; }
    nav a, .nav-note {
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
    }
    nav a:hover, .text-link:hover { color: #b5a58b; }
    .hero {
      display: grid;
      grid-template-columns: 1.05fr .95fr;
      min-height: 590px;
      border-bottom: 1px solid var(--line);
    }
    .hero-copy {
      padding: 90px 8% 75px 12%;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;
    }
    .eyebrow {
      font-size: 10px;
      letter-spacing: 3px;
      line-height: 1.8;
      text-transform: uppercase;
      color: var(--muted);
    }
    h1 {
      font-size: clamp(55px, 8.5vw, 112px);
      line-height: .86;
      letter-spacing: -.085em;
      margin: 27px 0;
      font-weight: 900;
    }
    h1 span { color: #a8a397; }
    .hero-copy p {
      color: #c3bfb5;
      font-size: 13px;
      line-height: 1.9;
      max-width: 340px;
    }
    .button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 17px 22px;
      margin-top: 25px;
      background: var(--cream);
      color: var(--black);
      font-size: 10px;
      letter-spacing: 1.8px;
      font-weight: 700;
      text-transform: uppercase;
      transition: background .2s;
    }
    .button:hover { background: #c9bda8; }
    .hero-art {
      min-height: 480px;
      background:
        radial-gradient(ellipse at 50% 43%, #45433e 0%, #252421 32%, #171716 67%, #10100f 100%);
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }
    .art-index {
      position: absolute;
      top: 26px;
      right: 26px;
      font-size: 9px;
      letter-spacing: 2px;
      color: #c0bbb0;
    }
    .tee {
      width: min(76%, 360px);
      filter: drop-shadow(0 25px 25px #0008);
      transform: rotate(-3deg);
    }
    .art-caption {
      position: absolute;
      bottom: 25px;
      left: 25px;
      right: 25px;
      display: flex;
      justify-content: space-between;
      gap: 10px;
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: #d2cec5;
    }
    .ticker {
      overflow: hidden;
      white-space: nowrap;
      padding: 17px 0;
      border-bottom: 1px solid var(--line);
      font-size: 10px;
      letter-spacing: 3px;
      color: #c2b9a9;
      text-align: center;
    }
    section { padding: 90px 7%; }
    .section-top {
      display: flex;
      align-items: end;
      justify-content: space-between;
      gap: 20px;
      margin-bottom: 35px;
    }
    h2 {
      font-size: clamp(32px, 5vw, 56px);
      letter-spacing: -.06em;
      line-height: 1;
      margin: 13px 0 0;
    }
    .text-link {
      padding-bottom: 7px;
      border-bottom: 1px solid var(--cream);
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      white-space: nowrap;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 16px;
    }
    .product-visual {
      min-height: 290px;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      background: #201f1c;
      position: relative;
    }
    .product-visual.light { background: #d8d3c8; }
    .product-visual.grey { background: #34332f; }
    .product-visual svg {
      width: 76%;
      max-height: 275px;
      filter: drop-shadow(0 15px 13px #0005);
      transition: transform .4s;
    }
    .product-card:hover svg { transform: scale(1.04); }
    .product-number {
      position: absolute;
      top: 15px;
      left: 15px;
      font-size: 9px;
      letter-spacing: 2px;
      color: #aaa69e;
    }
    .product-visual.light .product-number { color: #555148; }
    .product-meta {
      padding: 16px 0 5px;
      display: flex;
      justify-content: space-between;
      gap: 10px;
    }
    .product-meta h3 {
      margin: 0;
      font-size: 11px;
      letter-spacing: 1.3px;
    }
    .product-meta span {
      font-size: 9px;
      color: var(--muted);
      text-align: right;
    }
    .product-note {
      font-size: 11px;
      color: var(--muted);
      line-height: 1.8;
    }
    .manifesto {
      background: var(--cream);
      color: var(--black);
      display: grid;
      grid-template-columns: .8fr 1.2fr;
      gap: 45px;
      align-items: start;
    }
    .manifesto .eyebrow { color: #625d53; }
    .manifesto h2 { font-size: clamp(38px, 6vw, 72px); }
    .manifesto-copy p {
      max-width: 470px;
      font-size: 14px;
      line-height: 2;
      color: #49463f;
    }
    .scripture {
      border-left: 2px solid var(--red);
      padding-left: 17px;
      margin-top: 28px;
      font-size: 11px;
      letter-spacing: 1px;
      line-height: 1.9;
    }
    .editorial {
      display: grid;
      grid-template-columns: 1fr 1fr;
      min-height: 370px;
      border-bottom: 1px solid var(--line);
    }
    .editorial-art {
      background:
        linear-gradient(145deg, transparent 45%, #ffffff08 45% 46%, transparent 46%),
        radial-gradient(ellipse at 50% 45%, #37352f, #181817 70%);
      display: grid;
      place-items: center;
      padding: 40px;
    }
    .cross-mark {
      font-family: Georgia, serif;
      font-size: clamp(100px, 18vw, 210px);
      color: #c3bba9;
      line-height: 1;
      font-weight: normal;
    }
    .editorial-copy {
      padding: 65px 10%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
    }
    .editorial-copy h2 { max-width: 430px; }
    .editorial-copy p {
      font-size: 12px;
      color: var(--muted);
      line-height: 2;
      max-width: 370px;
    }
    .closing {
      padding: 85px 20px;
      text-align: center;
    }
    .closing h2 {
      font-size: clamp(38px, 8vw, 86px);
      margin: 20px 0;
    }
    .closing p {
      color: var(--muted);
      font-size: 12px;
      line-height: 1.8;
    }
    footer {
      border-top: 1px solid var(--line);
      padding: 28px 6%;
      display: flex;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
      align-items: center;
    }
    footer .logo { font-size: 16px; }
    footer small {
      color: var(--muted);
      font-size: 9px;
      letter-spacing: 1px;
    }
    @media (max-width: 700px) {
      header { height: 67px; padding: 0 5%; }
      .logo { font-size: 19px; letter-spacing: 4px; }
      nav { gap: 13px; }
      nav a { font-size: 8px; letter-spacing: .8px; }
      .nav-note { display: none; }
      .hero { grid-template-columns: 1fr; }
      .hero-copy { padding: 65px 7% 50px; }
      h1 { font-size: clamp(64px, 16vw, 100px); }
      .hero-art { min-height: 380px; }
      .tee { width: min(68%, 290px); }
      section { padding: 65px 6%; }
      .products { grid-template-columns: 1fr 1fr; gap: 20px 12px; }
      .product-visual { min-height: 220px; }
      .product-card:last-child { grid-column: 1 / -1; }
      .product-card:last-child .product-visual { min-height: 260px; }
      .section-top { align-items: start; }
      .section-top .text-link { margin-top: 13px; }
      .manifesto { grid-template-columns: 1fr; gap: 20px; }
      .editorial { grid-template-columns: 1fr; }
      .editorial-art { min-height: 260px; }
      .editorial-copy { padding: 55px 7%; }
      footer { padding: 25px 6%; }
    }
    @media (max-width: 360px) {
      nav { gap: 9px; }
      nav a { font-size: 7px; }
      .products { grid-template-columns: 1fr; }
      .product-card:last-child { grid-column: auto; }
    }
  </style>
</head>
<body>
  <div class="announcement">Faith in every thread · Est. 2026</div>

  <header>
    <a class="logo" href="#" aria-label="Salvane home">SALVANE</a>
    <nav aria-label="Main navigation">
      <a href="#collection">Collection</a>
      <a href="#story">Our purpose</a>
    </nav>
    <span class="nav-note">Accra, GH</span>
  </header>

  <main>
    <section class="hero" style="padding:0">
      <div class="hero-copy">
        <div class="eyebrow">Independent faith-driven streetwear</div>
        <h1>WEAR<br>YOUR<br><span>FAITH.</span></h1>
        <p>Clothing with conviction. Created to carry a message greater than ourselves.</p>
        <a class="button" href="#collection">Explore the collection ↗</a>
      </div>

      <div class="hero-art" aria-label="Salvane black tee concept">
        <span class="art-index">SALVANE / 001</span>
        <svg class="tee" viewBox="0 0 400 440" role="img" aria-label="Black oversized Salvane T-shirt with a cross">
          <path d="M115 45 L158 27 Q200 55 242 27 L285 45 L365 102 L324 164 L282 139 L292 407 Q200 427 108 407 L118 139 L76 164 L35 102 Z" fill="#0b0b0a" stroke="#55534d" stroke-width="2"/>
          <path d="M158 27 Q160 76 200 80 Q240 76 242 27" fill="#161614" stroke="#55534d" stroke-width="2"/>
          <path d="M118 139 L108 407 M282 139 L292 407" stroke="#292824" stroke-width="2" fill="none"/>
          <text x="200" y="205" text-anchor="middle" fill="#e8e2d6" font-size="20" font-weight="bold" letter-spacing="5">SALVANE</text>
          <path d="M200 227 V274 M184 243 H216" stroke="#e8e2d6" stroke-width="4" stroke-linecap="square"/>
          <text x="200" y="300" text-anchor="middle" fill="#bcb5a8" font-size="8" letter-spacing="3">FAITH OVER EVERYTHING</text>
          <text x="200" y="380" text-anchor="middle" fill="#77736a" font-size="8" letter-spacing="2">EST. MMXXVI</text>
        </svg>
        <div class="art-caption">
          <span>Chapter 001</span>
          <span>Made with purpose</span>
        </div>
      </div>
    </section>

    <div class="ticker">BELIEF IS PERSONAL — LET IT BE VISIBLE — SALVANE EST. 2026</div>

    <section id="collection">
      <div class="section-top">
        <div>
          <div class="eyebrow">01 / Selected concepts</div>
          <h2>THE COLLECTION.</h2>
        </div>
        <a class="text-link" href="#story">Our philosophy ↗</a>
      </div>

      <div class="products">
        <article class="product-card">
          <div class="product-visual">
            <span class="product-number">CONCEPT 001</span>
            <svg viewBox="0 0 240 270" aria-label="Black Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#090909" stroke="#55534e"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#444"/>
              <text x="120" y="132" text-anchor="middle" fill="#eeeae1" font-size="12" font-weight="bold" letter-spacing="2">SALVANE</text>
              <path d="M120 144 V174 M109 154 H131" stroke="#eeeae1" stroke-width="3"/>
            </svg>
          </div>
          <div class="product-meta"><h3>THE FOUNDATION</h3><span>BLACK / CONCEPT</span></div>
          <p class="product-note">A quiet statement. A lasting purpose.</p>
        </article>

        <article class="product-card">
          <div class="product-visual light">
            <span class="product-number">CONCEPT 002</span>
            <svg viewBox="0 0 240 270" aria-label="Cream Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#e7e0d3" stroke="#b4ac9c"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#c0b8aa"/>
              <text x="120" y="132" text-anchor="middle" fill="#181715" font-size="12" font-weight="bold" letter-spacing="2">SALVANE</text>
              <path d="M120 144 V174 M109 154 H131" stroke="#181715" stroke-width="3"/>
            </svg>
          </div>
          <div class="product-meta"><h3>THE WITNESS</h3><span>CREAM / CONCEPT</span></div>
          <p class="product-note">Understated design. Unshaken belief.</p>
        </article>

        <article class="product-card">
          <div class="product-visual grey">
            <span class="product-number">CONCEPT 003</span>
            <svg viewBox="0 0 240 270" aria-label="Graphic Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#1b1b19" stroke="#666158"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#444"/>
              <text x="120" y="120" text-anchor="middle" fill="#eeeae1" font-size="10" font-weight="bold" letter-spacing="2">FAITH</text>
              <path d="M120 135 V173 M107 147 H133" stroke="#eeeae1" stroke-width="3"/>
              <text x="120" y="193" text-anchor="middle" fill="#c9c1b4" font-size="8" letter-spacing="2">OVER FEAR</text>
            </svg>
          </div>
          <div class="product-meta"><h3>THE REMINDER</h3><span>GRAPHIC / CONCEPT</span></div>
          <p class="product-note">Wear the message. Live the meaning.</p>
        </article>
      </div>
      <p class="product-note" style="margin-top:25px">These are visual concepts, not products currently available for purchase.</p>
    </section>

    <section class="manifesto" id="story">
      <div>
        <div class="eyebrow">02 / Why Salvane exists</div>
        <h2>MORE THAN<br>A LABEL.</h2>
      </div>
      <div class="manifesto-copy">
        <p>Salvane is a faith-driven streetwear project built to share God's Word through clothing and culture. We believe what you wear can open a conversation, express conviction, and remind you of what matters.</p>
        <p>Rooted in belief. Designed with intention. Made to stand for something.</p>
        <div class="scripture">“Let your light shine before others.”<br>MATTHEW 5:16</div>
      </div>
    </section>

    <section class="editorial">
      <div class="editorial-art" aria-label="Cross symbol">
        <span class="cross-mark">✝</span>
      </div>
      <div class="editorial-copy">
        <div class="eyebrow">03 / The principle</div>
        <h2>LET YOUR<br>LIFE SPEAK.</h2>
        <p>Not hype for the sake of hype. Not clothing without meaning. Salvane is an invitation to live what you believe, wherever you go.</p>
        <a class="text-link" href="#collection">Discover our concepts ↗</a>
      </div>
    </section>

    <section class="closing">
      <div class="eyebrow">SALVANE · EST. 2026</div>
      <h2>FAITH IN<br>EVERY THREAD.</h2>
      <p>Accra, Ghana · Independent faith-driven streetwear</p>
      <a class="button" href="#collection">Explore Salvane ↑</a>
    </section>
  </main>

  <footer>
    <a class="logo" href="#">SALVANE</a>
    <small>FAITH · IDENTITY · PURPOSE</small>
    <small>© 2026 SALVANE. ALL RIGHTS RESERVED.</small>
  </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#10100f">
  <title>SALVANE — Faith in Every Thread</title>
  <meta name="description" content="Salvane is faith-driven streetwear built around belief, identity and purpose.">
  <style>
    :root {
      --black: #10100f;
      --cream: #eeeae1;
      --muted: #a6a39b;
      --line: rgba(238,234,225,.2);
      --red: #873d35;
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      background: var(--black);
      color: var(--cream);
      font-family: Arial, Helvetica, sans-serif;
    }
    a { color: inherit; text-decoration: none; }
    button, a { -webkit-tap-highlight-color: transparent; }
    .announcement {
      padding: 10px 15px;
      text-align: center;
      border-bottom: 1px solid var(--line);
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }
    header {
      height: 76px;
      padding: 0 6%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid var(--line);
    }
    .logo {
      font-size: 23px;
      font-weight: 900;
      letter-spacing: 5px;
    }
    nav { display: flex; gap: 27px; }
    nav a, .nav-note {
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
    }
    nav a:hover, .text-link:hover { color: #b5a58b; }
    .hero {
      display: grid;
      grid-template-columns: 1.05fr .95fr;
      min-height: 590px;
      border-bottom: 1px solid var(--line);
    }
    .hero-copy {
      padding: 90px 8% 75px 12%;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: center;
    }
    .eyebrow {
      font-size: 10px;
      letter-spacing: 3px;
      line-height: 1.8;
      text-transform: uppercase;
      color: var(--muted);
    }
    h1 {
      font-size: clamp(55px, 8.5vw, 112px);
      line-height: .86;
      letter-spacing: -.085em;
      margin: 27px 0;
      font-weight: 900;
    }
    h1 span { color: #a8a397; }
    .hero-copy p {
      color: #c3bfb5;
      font-size: 13px;
      line-height: 1.9;
      max-width: 340px;
    }
    .button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 17px 22px;
      margin-top: 25px;
      background: var(--cream);
      color: var(--black);
      font-size: 10px;
      letter-spacing: 1.8px;
      font-weight: 700;
      text-transform: uppercase;
      transition: background .2s;
    }
    .button:hover { background: #c9bda8; }
    .hero-art {
      min-height: 480px;
      background:
        radial-gradient(ellipse at 50% 43%, #45433e 0%, #252421 32%, #171716 67%, #10100f 100%);
      position: relative;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }
    .art-index {
      position: absolute;
      top: 26px;
      right: 26px;
      font-size: 9px;
      letter-spacing: 2px;
      color: #c0bbb0;
    }
    .tee {
      width: min(76%, 360px);
      filter: drop-shadow(0 25px 25px #0008);
      transform: rotate(-3deg);
    }
    .art-caption {
      position: absolute;
      bottom: 25px;
      left: 25px;
      right: 25px;
      display: flex;
      justify-content: space-between;
      gap: 10px;
      font-size: 9px;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: #d2cec5;
    }
    .ticker {
      overflow: hidden;
      white-space: nowrap;
      padding: 17px 0;
      border-bottom: 1px solid var(--line);
      font-size: 10px;
      letter-spacing: 3px;
      color: #c2b9a9;
      text-align: center;
    }
    section { padding: 90px 7%; }
    .section-top {
      display: flex;
      align-items: end;
      justify-content: space-between;
      gap: 20px;
      margin-bottom: 35px;
    }
    h2 {
      font-size: clamp(32px, 5vw, 56px);
      letter-spacing: -.06em;
      line-height: 1;
      margin: 13px 0 0;
    }
    .text-link {
      padding-bottom: 7px;
      border-bottom: 1px solid var(--cream);
      font-size: 10px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      white-space: nowrap;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 16px;
    }
    .product-visual {
      min-height: 290px;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      background: #201f1c;
      position: relative;
    }
    .product-visual.light { background: #d8d3c8; }
    .product-visual.grey { background: #34332f; }
    .product-visual svg {
      width: 76%;
      max-height: 275px;
      filter: drop-shadow(0 15px 13px #0005);
      transition: transform .4s;
    }
    .product-card:hover svg { transform: scale(1.04); }
    .product-number {
      position: absolute;
      top: 15px;
      left: 15px;
      font-size: 9px;
      letter-spacing: 2px;
      color: #aaa69e;
    }
    .product-visual.light .product-number { color: #555148; }
    .product-meta {
      padding: 16px 0 5px;
      display: flex;
      justify-content: space-between;
      gap: 10px;
    }
    .product-meta h3 {
      margin: 0;
      font-size: 11px;
      letter-spacing: 1.3px;
    }
    .product-meta span {
      font-size: 9px;
      color: var(--muted);
      text-align: right;
    }
    .product-note {
      font-size: 11px;
      color: var(--muted);
      line-height: 1.8;
    }
    .manifesto {
      background: var(--cream);
      color: var(--black);
      display: grid;
      grid-template-columns: .8fr 1.2fr;
      gap: 45px;
      align-items: start;
    }
    .manifesto .eyebrow { color: #625d53; }
    .manifesto h2 { font-size: clamp(38px, 6vw, 72px); }
    .manifesto-copy p {
      max-width: 470px;
      font-size: 14px;
      line-height: 2;
      color: #49463f;
    }
    .scripture {
      border-left: 2px solid var(--red);
      padding-left: 17px;
      margin-top: 28px;
      font-size: 11px;
      letter-spacing: 1px;
      line-height: 1.9;
    }
    .editorial {
      display: grid;
      grid-template-columns: 1fr 1fr;
      min-height: 370px;
      border-bottom: 1px solid var(--line);
    }
    .editorial-art {
      background:
        linear-gradient(145deg, transparent 45%, #ffffff08 45% 46%, transparent 46%),
        radial-gradient(ellipse at 50% 45%, #37352f, #181817 70%);
      display: grid;
      place-items: center;
      padding: 40px;
    }
    .cross-mark {
      font-family: Georgia, serif;
      font-size: clamp(100px, 18vw, 210px);
      color: #c3bba9;
      line-height: 1;
      font-weight: normal;
    }
    .editorial-copy {
      padding: 65px 10%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
    }
    .editorial-copy h2 { max-width: 430px; }
    .editorial-copy p {
      font-size: 12px;
      color: var(--muted);
      line-height: 2;
      max-width: 370px;
    }
    .closing {
      padding: 85px 20px;
      text-align: center;
    }
    .closing h2 {
      font-size: clamp(38px, 8vw, 86px);
      margin: 20px 0;
    }
    .closing p {
      color: var(--muted);
      font-size: 12px;
      line-height: 1.8;
    }
    footer {
      border-top: 1px solid var(--line);
      padding: 28px 6%;
      display: flex;
      justify-content: space-between;
      gap: 20px;
      flex-wrap: wrap;
      align-items: center;
    }
    footer .logo { font-size: 16px; }
    footer small {
      color: var(--muted);
      font-size: 9px;
      letter-spacing: 1px;
    }
    @media (max-width: 700px) {
      header { height: 67px; padding: 0 5%; }
      .logo { font-size: 19px; letter-spacing: 4px; }
      nav { gap: 13px; }
      nav a { font-size: 8px; letter-spacing: .8px; }
      .nav-note { display: none; }
      .hero { grid-template-columns: 1fr; }
      .hero-copy { padding: 65px 7% 50px; }
      h1 { font-size: clamp(64px, 16vw, 100px); }
      .hero-art { min-height: 380px; }
      .tee { width: min(68%, 290px); }
      section { padding: 65px 6%; }
      .products { grid-template-columns: 1fr 1fr; gap: 20px 12px; }
      .product-visual { min-height: 220px; }
      .product-card:last-child { grid-column: 1 / -1; }
      .product-card:last-child .product-visual { min-height: 260px; }
      .section-top { align-items: start; }
      .section-top .text-link { margin-top: 13px; }
      .manifesto { grid-template-columns: 1fr; gap: 20px; }
      .editorial { grid-template-columns: 1fr; }
      .editorial-art { min-height: 260px; }
      .editorial-copy { padding: 55px 7%; }
      footer { padding: 25px 6%; }
    }
    @media (max-width: 360px) {
      nav { gap: 9px; }
      nav a { font-size: 7px; }
      .products { grid-template-columns: 1fr; }
      .product-card:last-child { grid-column: auto; }
    }
  </style>
</head>
<body>
  <div class="announcement">Faith in every thread · Est. 2026</div>

  <header>
    <a class="logo" href="#" aria-label="Salvane home">SALVANE</a>
    <nav aria-label="Main navigation">
      <a href="#collection">Collection</a>
      <a href="#story">Our purpose</a>
    </nav>
    <span class="nav-note">Accra, GH</span>
  </header>

  <main>
    <section class="hero" style="padding:0">
      <div class="hero-copy">
        <div class="eyebrow">Independent faith-driven streetwear</div>
        <h1>WEAR<br>YOUR<br><span>FAITH.</span></h1>
        <p>Clothing with conviction. Created to carry a message greater than ourselves.</p>
        <a class="button" href="#collection">Explore the collection ↗</a>
      </div>

      <div class="hero-art" aria-label="Salvane black tee concept">
        <span class="art-index">SALVANE / 001</span>
        <svg class="tee" viewBox="0 0 400 440" role="img" aria-label="Black oversized Salvane T-shirt with a cross">
          <path d="M115 45 L158 27 Q200 55 242 27 L285 45 L365 102 L324 164 L282 139 L292 407 Q200 427 108 407 L118 139 L76 164 L35 102 Z" fill="#0b0b0a" stroke="#55534d" stroke-width="2"/>
          <path d="M158 27 Q160 76 200 80 Q240 76 242 27" fill="#161614" stroke="#55534d" stroke-width="2"/>
          <path d="M118 139 L108 407 M282 139 L292 407" stroke="#292824" stroke-width="2" fill="none"/>
          <text x="200" y="205" text-anchor="middle" fill="#e8e2d6" font-size="20" font-weight="bold" letter-spacing="5">SALVANE</text>
          <path d="M200 227 V274 M184 243 H216" stroke="#e8e2d6" stroke-width="4" stroke-linecap="square"/>
          <text x="200" y="300" text-anchor="middle" fill="#bcb5a8" font-size="8" letter-spacing="3">FAITH OVER EVERYTHING</text>
          <text x="200" y="380" text-anchor="middle" fill="#77736a" font-size="8" letter-spacing="2">EST. MMXXVI</text>
        </svg>
        <div class="art-caption">
          <span>Chapter 001</span>
          <span>Made with purpose</span>
        </div>
      </div>
    </section>

    <div class="ticker">BELIEF IS PERSONAL — LET IT BE VISIBLE — SALVANE EST. 2026</div>

    <section id="collection">
      <div class="section-top">
        <div>
          <div class="eyebrow">01 / Selected concepts</div>
          <h2>THE COLLECTION.</h2>
        </div>
        <a class="text-link" href="#story">Our philosophy ↗</a>
      </div>

      <div class="products">
        <article class="product-card">
          <div class="product-visual">
            <span class="product-number">CONCEPT 001</span>
            <svg viewBox="0 0 240 270" aria-label="Black Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#090909" stroke="#55534e"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#444"/>
              <text x="120" y="132" text-anchor="middle" fill="#eeeae1" font-size="12" font-weight="bold" letter-spacing="2">SALVANE</text>
              <path d="M120 144 V174 M109 154 H131" stroke="#eeeae1" stroke-width="3"/>
            </svg>
          </div>
          <div class="product-meta"><h3>THE FOUNDATION</h3><span>BLACK / CONCEPT</span></div>
          <p class="product-note">A quiet statement. A lasting purpose.</p>
        </article>

        <article class="product-card">
          <div class="product-visual light">
            <span class="product-number">CONCEPT 002</span>
            <svg viewBox="0 0 240 270" aria-label="Cream Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#e7e0d3" stroke="#b4ac9c"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#c0b8aa"/>
              <text x="120" y="132" text-anchor="middle" fill="#181715" font-size="12" font-weight="bold" letter-spacing="2">SALVANE</text>
              <path d="M120 144 V174 M109 154 H131" stroke="#181715" stroke-width="3"/>
            </svg>
          </div>
          <div class="product-meta"><h3>THE WITNESS</h3><span>CREAM / CONCEPT</span></div>
          <p class="product-note">Understated design. Unshaken belief.</p>
        </article>

        <article class="product-card">
          <div class="product-visual grey">
            <span class="product-number">CONCEPT 003</span>
            <svg viewBox="0 0 240 270" aria-label="Graphic Salvane tee concept">
              <path d="M73 30 L99 19 Q120 35 141 19 L167 30 L211 65 L188 101 L164 87 L170 245 Q120 256 70 245 L76 87 L52 101 L29 65 Z" fill="#1b1b19" stroke="#666158"/>
              <path d="M99 19 Q100 50 120 51 Q140 50 141 19" fill="none" stroke="#444"/>
              <text x="120" y="120" text-anchor="middle" fill="#eeeae1" font-size="10" font-weight="bold" letter-spacing="2">FAITH</text>
              <path d="M120 135 V173 M107 147 H133" stroke="#eeeae1" stroke-width="3"/>
              <text x="120" y="193" text-anchor="middle" fill="#c9c1b4" font-size="8" letter-spacing="2">OVER FEAR</text>
            </svg>
          </div>
          <div class="product-meta"><h3>THE REMINDER</h3><span>GRAPHIC / CONCEPT</span></div>
          <p class="product-note">Wear the message. Live the meaning.</p>
        </article>
      </div>
      <p class="product-note" style="margin-top:25px">These are visual concepts, not products currently available for purchase.</p>
    </section>

    <section class="manifesto" id="story">
      <div>
        <div class="eyebrow">02 / Why Salvane exists</div>
        <h2>MORE THAN<br>A LABEL.</h2>
      </div>
      <div class="manifesto-copy">
        <p>Salvane is a faith-driven streetwear project built to share God's Word through clothing and culture. We believe what you wear can open a conversation, express conviction, and remind you of what matters.</p>
        <p>Rooted in belief. Designed with intention. Made to stand for something.</p>
        <div class="scripture">“Let your light shine before others.”<br>MATTHEW 5:16</div>
      </div>
    </section>

    <section class="editorial">
      <div class="editorial-art" aria-label="Cross symbol">
        <span class="cross-mark">✝</span>
      </div>
      <div class="editorial-copy">
        <div class="eyebrow">03 / The principle</div>
        <h2>LET YOUR<br>LIFE SPEAK.</h2>
        <p>Not hype for the sake of hype. Not clothing without meaning. Salvane is an invitation to live what you believe, wherever you go.</p>
        <a class="text-link" href="#collection">Discover our concepts ↗</a>
      </div>
    </section>

    <section class="closing">
      <div class="eyebrow">SALVANE · EST. 2026</div>
      <h2>FAITH IN<br>EVERY THREAD.</h2>
      <p>Accra, Ghana · Independent faith-driven streetwear</p>
      <a class="button" href="#collection">Explore Salvane ↑</a>
    </section>
  </main>

  <footer>
    <a class="logo" href="#">SALVANE</a>
    <small>FAITH · IDENTITY · PURPOSE</small>
    <small>© 2026 SALVANE. ALL RIGHTS RESERVED.</small>
  </footer>
</body>
</html>
