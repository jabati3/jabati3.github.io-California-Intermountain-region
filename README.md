<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#17271f" />
  <meta
    name="description"
    content="Explore the art and strategy of golf course architecture: routing, risk and reward, green complexes, and the architects who shape the game."
  />
  <title>Ground Game — The Art of Golf Course Architecture</title>

  <style>
    :root {
      --forest: #17271f;
      --forest-light: #23392d;
      --cream: #f3f0e7;
      --paper: #e8e4d8;
      --sand: #d7c6a1;
      --sage: #a9b69a;
      --ink: #1b261f;
      --muted: #647064;
      --line: rgba(23, 39, 31, 0.18);
      --serif: Georgia, "Times New Roman", serif;
      --sans: "Helvetica Neue", Helvetica, Arial, sans-serif;
    }

    *,
    *::before,
    *::after {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      color: var(--ink);
      background: var(--cream);
      font-family: var(--sans);
      line-height: 1.6;
    }

    a {
      color: inherit;
    }

    .site-header {
      position: absolute;
      z-index: 5;
      top: 0;
      left: 0;
      display: flex;
      width: 100%;
      align-items: center;
      justify-content: space-between;
      padding: 1.3rem 6vw;
      color: var(--cream);
      border-bottom: 1px solid rgba(243, 240, 231, 0.24);
    }

    .wordmark {
      font-size: 0.8rem;
      font-weight: 700;
      letter-spacing: 0.2em;
      text-decoration: none;
      text-transform: uppercase;
    }

    .wordmark span {
      display: block;
      margin-top: 0.15rem;
      color: var(--sage);
      font-size: 0.57rem;
      font-weight: 400;
      letter-spacing: 0.25em;
    }

    .site-nav {
      display: flex;
      gap: clamp(1rem, 3vw, 2.5rem);
    }

    .site-nav a {
      color: var(--cream);
      font-size: 0.7rem;
      letter-spacing: 0.12em;
      text-decoration: none;
      text-transform: uppercase;
      transition: color 180ms ease;
    }

    .site-nav a:hover,
    .site-nav a:focus-visible {
      color: var(--sand);
    }

    .hero {
      position: relative;
      display: grid;
      min-height: min(820px, 100svh);
      align-items: end;
      overflow: hidden;
      padding: 9rem 8vw 8vh;
      color: var(--cream);
      background:
        linear-gradient(90deg, rgba(13, 27, 21, 0.76), rgba(13, 27, 21, 0.12) 78%),
        linear-gradient(0deg, rgba(13, 27, 21, 0.5), transparent 55%),
        url("https://images.unsplash.com/photo-1587174486073-ae5e5cff23aa?auto=format&fit=crop&w=2200&q=85")
          center 54% / cover;
    }

    .hero-content {
      max-width: 850px;
      animation: rise-in 850ms ease both;
    }

    .eyebrow {
      display: flex;
      align-items: center;
      gap: 0.8rem;
      margin: 0 0 1.2rem;
      color: var(--sage);
      font-size: 0.68rem;
      font-weight: 700;
      letter-spacing: 0.2em;
      text-transform: uppercase;
    }

    .eyebrow::before {
      width: 2rem;
      height: 1px;
      background: currentColor;
      content: "";
    }

    h1,
    h2,
    h3,
    p {
      margin-top: 0;
    }

    .hero h1 {
      max-width: 800px;
      margin-bottom: 1.2rem;
      font-family: var(--serif);
      font-size: clamp(3.6rem, 10vw, 8.5rem);
      font-weight: 400;
      letter-spacing: -0.065em;
      line-height: 0.89;
    }

    .hero-copy {
      max-width: 600px;
      margin-bottom: 2rem;
      color: rgba(243, 240, 231, 0.84);
      font-size: clamp(1rem, 1.5vw, 1.18rem);
    }

    .text-link {
      display: inline-flex;
      align-items: center;
      gap: 0.8rem;
      color: var(--cream);
      font-size: 0.72rem;
      font-weight: 700;
      letter-spacing: 0.13em;
      text-decoration: none;
      text-transform: uppercase;
    }

    .text-link span {
      display: inline-grid;
      width: 2.1rem;
      height: 2.1rem;
      place-items: center;
      border: 1px solid rgba(243, 240, 231, 0.65);
      border-radius: 50%;
      transition: color 180ms ease, background 180ms ease, transform 180ms ease;
    }

    .text-link:hover span {
      transform: translateX(4px);
      color: var(--forest);
      background: var(--cream);
    }

    .section {
      padding: clamp(5rem, 10vw, 9rem) 8vw;
    }

    .section-heading {
      display: grid;
      grid-template-columns: minmax(0, 0.8fr) minmax(280px, 1.2fr);
      gap: 3rem;
      align-items: end;
      margin-bottom: 3.5rem;
    }

    .section-heading h2 {
      max-width: 620px;
      margin: 0;
      font-family: var(--serif);
      font-size: clamp(2.6rem, 6vw, 5.2rem);
      font-weight: 400;
      letter-spacing: -0.055em;
      line-height: 0.98;
    }

    .section-heading > p {
      max-width: 540px;
      margin: 0;
      color: var(--muted);
      font-size: 1rem;
    }

    .intro {
      background: var(--cream);
    }

    .intro-grid {
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: clamp(2rem, 7vw, 7rem);
      align-items: center;
    }

    .intro-image {
      position: relative;
      min-height: 540px;
      background:
        linear-gradient(0deg, rgba(19, 38, 27, 0.13), transparent 50%),
        url("https://images.unsplash.com/photo-1593111774240-d529f12cf4bb?auto=format&fit=crop&w=1200&q=85")
          center / cover;
    }

    .image-caption {
      position: absolute;
      right: 1.2rem;
      bottom: 1.2rem;
      left: 1.2rem;
      color: white;
      font-size: 0.65rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
    }

    .intro-copy .eyebrow {
      color: #647b59;
    }

    .intro-copy h2 {
      margin-bottom: 1.4rem;
      font-family: var(--serif);
      font-size: clamp(2.4rem, 4vw, 4.25rem);
      font-weight: 400;
      letter-spacing: -0.05em;
      line-height: 1;
    }

    .intro-copy p {
      color: var(--muted);
    }

    .pull-quote {
      margin: 2rem 0;
      padding: 0.3rem 0 0.3rem 1.3rem;
      color: var(--forest);
      border-left: 2px solid #879777;
      font-family: var(--serif);
      font-size: 1.35rem;
      line-height: 1.4;
    }

    .principles {
      color: var(--cream);
      background: var(--forest);
    }

    .principles .section-heading > p {
      color: rgba(243, 240, 231, 0.67);
    }

    .principles .eyebrow {
      color: var(--sage);
    }

    .principle-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      border-top: 1px solid rgba(243, 240, 231, 0.24);
    }

    .principle-card {
      min-height: 290px;
      padding: 2rem clamp(1rem, 3vw, 2.5rem) 1rem 0;
    }

    .principle-card + .principle-card {
      padding-left: clamp(1rem, 3vw, 2.5rem);
      border-left: 1px solid rgba(243, 240, 231, 0.24);
    }

    .principle-number {
      color: var(--sage);
      font-size: 0.7rem;
      letter-spacing: 0.15em;
    }

    .principle-card h3 {
      margin: 2.6rem 0 0.8rem;
      font-family: var(--serif);
      font-size: clamp(1.7rem, 3vw, 2.5rem);
      font-weight: 400;
    }

    .principle-card p {
      max-width: 320px;
      margin-bottom: 0;
      color: rgba(243, 240, 231, 0.68);
      font-size: 0.93rem;
    }

    .strategy {
      background: var(--paper);
    }

    .strategy-layout {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: clamp(2rem, 7vw, 6rem);
      align-items: center;
    }

    .strategy-layout h2 {
      max-width: 550px;
      margin: 0 0 1.5rem;
      font-family: var(--serif);
      font-size: clamp(2.7rem, 6vw, 5.4rem);
      font-weight: 400;
      letter-spacing: -0.055em;
      line-height: 0.96;
    }

    .strategy-layout p {
      max-width: 540px;
      color: var(--muted);
    }

    .strategy-note {
      margin-top: 2rem;
      padding-top: 1rem;
      color: var(--forest);
      border-top: 1px solid var(--line);
      font-size: 0.72rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .hole-diagram {
      position: relative;
      display: grid;
      min-height: 520px;
      place-items: center;
      overflow: hidden;
      background:
        radial-gradient(ellipse at 48% 56%, rgba(196, 184, 145, 0.72) 0 4%, transparent 4.5%),
        radial-gradient(ellipse at 48% 56%, rgba(134, 157, 111, 0.44) 0 13%, transparent 13.5%),
        radial-gradient(ellipse at 30% 43%, rgba(134, 157, 111, 0.35) 0 17%, transparent 17.5%),
        radial-gradient(ellipse at 67% 67%, rgba(134, 157, 111, 0.3) 0 16%, transparent 16.5%),
        radial-gradient(ellipse at 63% 31%, rgba(134, 157, 111, 0.26) 0 13%, transparent 13.5%),
        #d5d0bd;
      border: 1px solid rgba(23, 39, 31, 0.12);
    }

    .hole-diagram::before,
    .hole-diagram::after {
      position: absolute;
      width: 150%;
      height: 1px;
      background: rgba(70, 91, 64, 0.22);
      content: "";
      transform: rotate(-24deg);
    }

    .hole-diagram::after {
      transform: rotate(28deg);
    }

    .route {
      position: absolute;
      z-index: 1;
      width: 55%;
      height: 63%;
      border: 2px dashed rgba(23, 39, 31, 0.58);
      border-bottom-color: transparent;
      border-left-color: transparent;
      border-radius: 0 62% 0 0;
      transform: rotate(-28deg);
    }

    .route::before,
    .route::after {
      position: absolute;
      width: 12px;
      height: 12px;
      border: 2px solid var(--forest);
      border-radius: 50%;
      background: var(--cream);
      content: "";
    }

    .route::before {
      right: -7px;
      bottom: -3px;
    }

    .route::after {
      top: -7px;
      right: -6px;
      background: var(--sand);
    }

    .map-label {
      position: absolute;
      z-index: 2;
      color: var(--forest);
      font-size: 0.62rem;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    .map-label.tee {
      right: 24%;
      bottom: 23%;
    }

    .map-label.green {
      top: 23%;
      right: 21%;
    }

    .map-label.bunker {
      top: 40%;
      left: 19%;
      color: #725d3e;
    }

    .map-label.route-label {
      top: 54%;
      right: 18%;
      transform: rotate(-25deg);
    }

    .architects {
      background: var(--cream);
    }

    .architect-list {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      border-top: 1px solid var(--line);
    }

    .architect-group {
      padding: 1.5rem 1.2rem 0 0;
    }

    .architect-group + .architect-group {
      padding-left: 1.5rem;
      border-left: 1px solid var(--line);
    }

    .architect-group h3 {
      margin-bottom: 1rem;
      color: #718067;
      font-size: 0.68rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
    }

    .architect-group p {
      margin: 0;
      font-family: var(--serif);
      font-size: clamp(1.15rem, 1.8vw, 1.6rem);
      line-height: 1.65;
    }

    .closing {
      position: relative;
      min-height: 560px;
      display: flex;
      align-items: center;
      color: var(--cream);
      background:
        linear-gradient(90deg, rgba(15, 31, 23, 0.83), rgba(15, 31, 23, 0.2)),
        url("https://images.unsplash.com/photo-1600166898405-da9535204843?auto=format&fit=crop&w=2000&q=85")
          center / cover;
    }

    .closing-content {
      width: min(760px, 84vw);
      margin-left: 8vw;
      padding: 5rem 0;
    }

    .closing h2 {
      margin-bottom: 1rem;
      font-family: var(--serif);
      font-size: clamp(3rem, 8vw, 6.8rem);
      font-weight: 400;
      letter-spacing: -0.06em;
      line-height: 0.93;
    }

    .closing p {
      max-width: 490px;
      color: rgba(243, 240, 231, 0.78);
    }

    footer {
      display: flex;
      justify-content: space-between;
      gap: 1rem;
      padding: 1.6rem 8vw;
      color: rgba(243, 240, 231, 0.67);
      background: var(--forest);
      font-size: 0.68rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    footer p {
      margin: 0;
    }

    @keyframes rise-in {
      from {
        opacity: 0;
        transform: translateY(18px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @media (max-width: 760px) {
      .site-header {
        padding: 1rem 6vw;
      }

      .site-nav {
        gap: 0.85rem;
      }

      .site-nav a {
        font-size: 0.58rem;
      }

      .hero {
        min-height: 740px;
        min-height: 92svh;
        padding: 8rem 7vw 7vh;
        background-position: 58% center;
      }

      .section {
        padding: 5rem 7vw;
      }

      .section-heading,
      .intro-grid,
      .strategy-layout {
        grid-template-columns: 1fr;
        gap: 1.7rem;
      }

      .section-heading {
        margin-bottom: 2.3rem;
      }

      .intro-image {
        min-height: 390px;
        order: 2;
      }

      .principle-grid {
        grid-template-columns: 1fr;
      }

      .principle-card,
      .principle-card + .principle-card {
        min-height: auto;
        padding: 1.5rem 0 2rem;
        border-left: 0;
      }

      .principle-card + .principle-card {
        border-top: 1px solid rgba(243, 240, 231, 0.24);
      }

      .principle-card h3 {
        margin-top: 1.2rem;
      }

      .hole-diagram {
        min-height: 390px;
      }

      .architect-list {
        grid-template-columns: repeat(2, 1fr);
      }

      .architect-group {
        padding: 1.3rem 0;
      }

      .architect-group + .architect-group {
        padding-left: 1rem;
      }

      .architect-group:nth-child(odd) {
        border-left: 0;
      }

      .architect-group:nth-child(n + 3) {
        border-top: 1px solid var(--line);
      }

      .closing {
        min-height: 470px;
      }

      footer {
        flex-direction: column;
        padding: 1.5rem 7vw;
      }
    }

    @media (max-width: 430px) {
      .site-nav {
        gap: 0.65rem;
      }

      .site-nav a {
        font-size: 0.52rem;
        letter-spacing: 0.07em;
      }

      .wordmark {
        font-size: 0.7rem;
      }

      .wordmark span {
        font-size: 0.5rem;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *,
      *::before,
      *::after {
        scroll-behavior: auto !important;
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>

<body>
  <header class="site-header">
    <a class="wordmark" href="#home" aria-label="Ground Game home">
      Ground Game
      <span>Golf course architecture</span>
    </a>

    <nav class="site-nav" aria-label="Main navigation">
      <a href="#philosophy">Philosophy</a>
      <a href="#strategy">Strategy</a>
      <a href="#architects">Architects</a>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="hero-content">
        <p class="eyebrow">Land, shaped by play</p>
        <h1>The ground<br />is the game.</h1>
        <p class="hero-copy">
          Golf course architecture turns a landscape into an unfolding
          conversation between player, strategy, and place.
        </p>
        <a class="text-link" href="#philosophy">
          Explore the craft <span aria-hidden="true">↓</span>
        </a>
      </div>
    </section>

    <section class="section intro" id="philosophy">
      <div class="intro-grid">
        <div class="intro-image" role="img" aria-label="Rolling golf course landscape">
          <span class="image-caption">A course begins with the land</span>
        </div>

        <div class="intro-copy">
          <p class="eyebrow">01 — Read the land</p>
          <h2>Design begins with looking.</h2>
          <p>
            Before a hole is drawn, the architect walks the site. Topography,
            drainage, soil, native vegetation, elevation, and prevailing winds
            all help reveal the natural shape of a course.
          </p>
          <p>
            The goal is not to force the land into a template. It is to find an
            organic routing: a sequence of holes that flows naturally, with
            varied lengths, directions, and short, intuitive walks from green
            to tee.
          </p>
          <blockquote class="pull-quote">
            “The best courses feel discovered, not imposed.”
          </blockquote>
          <p>
            Done well, the landscape itself becomes the designer’s material—and
            every round becomes a new way to experience it.
          </p>
        </div>
      </div>
    </section>

    <section class="section principles">
      <div class="section-heading">
        <div>
          <p class="eyebrow">02 — Three ways to challenge</p>
          <h2>One game.<br />Many questions.</h2>
        </div>
        <p>
          Great architecture balances challenge with choice. The classic
          design philosophies—penal, heroic, and strategic—offer different
          ways to test a player’s imagination and judgment.
        </p>
      </div>

      <div class="principle-grid">
        <article class="principle-card">
          <span class="principle-number">01 / PENAL</span>
          <h3>Risk has a price.</h3>
          <p>
            A direct challenge asks for precision. Miss the intended line and
            the hazards make the consequence clear.
          </p>
        </article>

        <article class="principle-card">
          <span class="principle-number">02 / HEROIC</span>
          <h3>Take on the bold line.</h3>
          <p>
            The ambitious route offers a reward for a well-executed shot—and
            leaves the player to decide if the gamble is worth it.
          </p>
        </article>

        <article class="principle-card">
          <span class="principle-number">03 / STRATEGIC</span>
          <h3>Choose your angle.</h3>
          <p>
            Generous space invites different routes. Position, not just
            distance, determines the next shot and opens up options.
          </p>
        </article>
      </div>
    </section>

    <section class="section strategy" id="strategy">
      <div class="strategy-layout">
        <div>
          <p class="eyebrow">03 — Risk &amp; reward</p>
          <h2>Space to play. Angles to earn.</h2>
          <p>
            A thoughtful hole gives every golfer a way forward. Wide fairways,
            deceptive sightlines, subtle contours, and carefully placed
            hazards create choices rather than a single forced line.
          </p>
          <p>
            A safer route can leave a longer or less direct approach. A bolder
            tee shot may flirt with a cross-bunker or natural slope to earn a
            clearer angle at a tucked pin. The decision changes with the
            player, the conditions, and the day.
          </p>
          <p class="strategy-note">A hole is a puzzle, not a corridor.</p>
        </div>

        <div
          class="hole-diagram"
          role="img"
          aria-label="Illustrated golf hole showing a tee, green, route, and bunker"
        >
          <span class="route" aria-hidden="true"></span>
          <span class="map-label tee">Tee</span>
          <span class="map-label green">Green</span>
          <span class="map-label bunker">Cross-bunker</span>
          <span class="map-label route-label">Play the angle</span>
        </div>
      </div>
    </section>

    <section class="section intro">
      <div class="intro-grid">
        <div class="intro-copy">
          <p class="eyebrow">04 — The green complex</p>
          <h2>Where the ground game comes alive.</h2>
          <p>
            The green is more than a target. Internal ridges, crowned surfaces,
            false fronts, and surrounding collection areas turn an approach
            into a test of trajectory, spin, and imagination.
          </p>
          <p>
            Closely mown hollows and natural tie-ins reward creativity on the
            ground, while thoughtful bailout areas give players another way
            to recover. The best green complexes are challenging without
            feeling unfair.
          </p>
          <p>
            In the end, the course works like outdoor chess: the terrain sets
            the problem, and every golfer finds a different way to solve it.
          </p>
        </div>

        <div
          class="intro-image"
          role="img"
          aria-label="Golf green shaped into a natural landscape"
          style="background-image: url('https://images.unsplash.com/photo-1562204320-31975a5e09ce?auto=format&fit=crop&w=1200&q=85');"
        >
          <span class="image-caption">The green is the heart of the hole</span>
        </div>
      </div>
    </section>

    <section class="section architects" id="architects">
      <div class="section-heading">
        <div>
          <p class="eyebrow">05 — The people behind the places</p>
          <h2>A tradition of thoughtful design.</h2>
        </div>
        <p>
          Across generations, influential architects have shown how restraint,
          strategy, and a close reading of the land can create courses that
          remain compelling for decades.
        </p>
      </div>

      <div class="architect-list">
        <article class="architect-group">
          <h3>Golden Age</h3>
          <p>Alister MacKenzie<br />Donald Ross</p>
        </article>
        <article class="architect-group">
          <h3>Golden Age</h3>
          <p>Harry Colt<br />C.B. Macdonald</p>
        </article>
        <article class="architect-group">
          <h3>Golden Age</h3>
          <p>A.W. Tillinghast</p>
        </article>
        <article class="architect-group">
          <h3>Modern minimalists</h3>
          <p>Bill Coore &amp; Ben Crenshaw<br />Gil Hanse<br />Tom Doak</p>
        </article>
      </div>
    </section>

    <section class="closing">
      <div class="closing-content">
        <p class="eyebrow">A living landscape</p>
        <h2>No two rounds<br />ask the same question.</h2>
        <p>
          Weather shifts. Pin positions move. A familiar hole reveals a new
          line. Great golf course architecture leaves room for the land—and
          the player—to keep surprising us.
        </p>
      </div>
    </section>
  </main>

  <footer>
    <p>Ground Game — The art of golf course architecture</p>
    <p>Read the land. Play the ground.</p>
  </footer>
</body>
</html>
