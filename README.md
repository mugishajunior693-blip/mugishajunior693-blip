<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>DJ AMBROY UG | MR 5 STAR</title>

  <meta name="description"
        content="Official website of DJ AMBROY UG — MR 5 STAR. Mixtapes, music, events and bookings.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #080808;
      color: white;
      line-height: 1.6;
    }

    /* NAVIGATION */

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(0,0,0,0.9);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid #222;
    }

    nav {
      max-width: 1200px;
      margin: auto;
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 25px;
    }

    .logo {
      font-size: 22px;
      font-weight: 900;
      letter-spacing: 2px;
    }

    .logo span {
      color: #ffcc00;
    }

    nav ul {
      display: flex;
      list-style: none;
      gap: 25px;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      color: #ffcc00;
    }

    /* HERO */

    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 120px 20px 60px;

      background:
        linear-gradient(rgba(0,0,0,0.72), rgba(0,0,0,0.9)),
        url("https://images.unsplash.com/photo-1571266028243-d220c9c3b7a5?auto=format&fit=crop&w=2000&q=80");

      background-size: cover;
      background-position: center;
    }

    .hero-content {
      max-width: 850px;
    }

    .hero h1 {
      font-size: clamp(45px, 8vw, 95px);
      line-height: 1;
      font-weight: 900;
      letter-spacing: 3px;
    }

    .hero h1 span {
      color: #ffcc00;
    }

    .hero p {
      margin: 25px 0;
      font-size: 20px;
      color: #ddd;
    }

    .tag {
      color: #ffcc00;
      font-size: 18px;
      font-weight: bold;
      letter-spacing: 4px;
      margin-bottom: 15px;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-block;
      padding: 14px 28px;
      border-radius: 30px;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    .primary {
      background: #ffcc00;
      color: #000;
    }

    .secondary {
      border: 2px solid white;
      color: white;
    }

    .btn:hover {
      transform: translateY(-4px);
    }

    /* SECTIONS */

    section {
      padding: 90px 20px;
    }

    .container {
      max-width: 1100px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 42px;
    }

    .section-title span {
      color: #ffcc00;
    }

    /* ABOUT */

    .about {
      background: #101010;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
      align-items: center;
    }

    .about-image {
      height: 450px;
      border-radius: 20px;
      background:
        linear-gradient(rgba(0,0,0,0.15), rgba(0,0,0,0.5)),
        url("https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?auto=format&fit=crop&w=1000&q=80");

      background-size: cover;
      background-position: center;
    }

    .about-text h3 {
      font-size: 32px;
      margin-bottom: 15px;
    }

    .about-text p {
      color: #bbb;
      margin-bottom: 15px;
    }

    .star {
      color: #ffcc00;
    }

    /* MIXTAPES */

    .mixtapes {
      background: #080808;
    }

    .mix-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 25px;
    }

    .mix-card {
      background: #151515;
      border: 1px solid #252525;
      border-radius: 15px;
      overflow: hidden;
      transition: 0.3s;
    }

    .mix-card:hover {
      transform: translateY(-8px);
      border-color: #ffcc00;
    }

    .mix-image {
      height: 220px;
      background-size: cover;
      background-position: center;
    }

    .mix1 {
      background-image: url("https://images.unsplash.com/photo-1493225457124-a3eb161ffa5f?auto=format&fit=crop&w=800&q=80");
    }

    .mix2 {
      background-image: url("https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?auto=format&fit=crop&w=800&q=80");
    }

    .mix3 {
      background-image: url("https://images.unsplash.com/photo-1571266028243-d220c9c3b7a5?auto=format&fit=crop&w=800&q=80");
    }

    .mix-info {
      padding: 20px;
    }

    .mix-info h3 {
      margin-bottom: 8px;
    }

    .mix-info p {
      color: #aaa;
      margin-bottom: 15px;
    }

    .listen {
      display: inline-block;
      padding: 9px 18px;
      background: #ffcc00;
      color: black;
      border-radius: 20px;
      text-decoration: none;
      font-weight: bold;
    }

    /* YOUTUBE */

    .youtube {
      background: #111;
      text-align: center;
    }

    .youtube-box {
      max-width: 750px;
      margin: auto;
      background: #181818;
      padding: 40px;
      border-radius: 20px;
    }

    .youtube-box h3 {
      font-size: 30px;
      margin-bottom: 15px;
    }

    .youtube-box p {
      color: #bbb;
      margin-bottom: 25px;
    }

    .youtube-btn {
      background: #e00000;
      color: white;
    }

    /* BOOKING */

    .booking {
      background: #080808;
    }

    .booking-box {
      max-width: 750px;
      margin: auto;
      text-align: center;
      background: #151515;
      padding: 45px 25px;
      border-radius: 20px;
      border: 1px solid #292929;
    }

    .booking-box h3 {
      font-size: 32px;
      margin-bottom: 15px;
    }

    .booking-box p {
      color: #bbb;
      margin-bottom: 25px;
    }

    /* CONTACT */

    .contact {
      background: #101010;
      text-align: center;
    }

    .contact-links {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 15px;
      margin-top: 30px;
    }

    .contact-links a {
      text-decoration: none;
      color: white;
      border: 1px solid #444;
      padding: 12px 22px;
      border-radius: 25px;
      transition: 0.3s;
    }

    .contact-links a:hover {
      background: #ffcc00;
      color: #000;
      border-color: #ffcc00;
    }

    /* FOOTER */

    footer {
      background: #050505;
      text-align: center;
      padding: 35px 20px;
      color: #777;
    }

    footer strong {
      color: white;
    }

    /* WHATSAPP */

    .whatsapp {
      position: fixed;
      right: 20px;
      bottom: 20px;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      background: #25d366;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      text-decoration: none;
      font-size: 27px;
      font-weight: bold;
      box-shadow: 0 5px 20px rgba(0,0,0,0.5);
      z-index: 999;
    }

    /* MOBILE */

    @media(max-width: 800px) {

      nav ul {
        display: none;
      }

      .about-grid {
        grid-template-columns: 1fr;
      }

      .about-image {
        height: 350px;
      }

      .mix-grid {
        grid-template-columns: 1fr;
      }

      .hero p {
        font-size: 17px;
      }

      section {
        padding: 70px 18px;
      }

    }

  </style>
</head>

<body>

<!-- NAVIGATION -->

<header>
  <nav>

    <div class="logo">
      DJ <span>AMBROY</span>
    </div>

    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#mixtapes">Mixtapes</a></li>
      <li><a href="#youtube">YouTube</a></li>
      <li><a href="#booking">Booking</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>

  </nav>
</header>


<!-- HERO -->

<section class="hero" id="home">

  <div class="hero-content">

    <div class="tag">
      UGANDAN DJ • MUSIC • VIBES
    </div>

    <h1>
      DJ <span>AMBROY</span>
    </h1>

    <p>
      MR 5 STAR ⭐
    </p>

    <p>
      Bringing you the hottest Ugandan vibes,
      nonstop mixtapes and unforgettable sounds.
    </p>

    <div class="buttons">

      <a href="#mixtapes" class="btn primary">
        🎵 LISTEN TO MIXTAPES
      </a>

      <a href="#booking" class="btn secondary">
        📅 BOOK DJ AMBROY
      </a>

    </div>

  </div>

</section>


<!-- ABOUT -->

<section class="about" id="about">

  <div class="container">

    <div class="section-title">
      <h2>ABOUT <span>DJ AMBROY</span></h2>
    </div>

    <div class="about-grid">

      <div class="about-image"></div>

      <div class="about-text">

        <h3>
          DJ AMBROY UG
          <span class="star">★</span>
        </h3>

        <p>
          Welcome to the official home of DJ Ambroy UG —
          Mr 5 Star.
        </p>

        <p>
          From Ugandan vibes to African sounds, DJ Ambroy
          brings energy, creativity and nonstop entertainment
          to every mix and event.
        </p>

        <p>
          No skipping. No stopping.
          Just pure vibes.
        </p>

      </div>

    </div>

  </div>

</section>


<!-- MIXTAPES -->

<section class="mixtapes" id="mixtapes">

  <div class="container">

    <div class="section-title">
      <h2>LATEST <span>MIXTAPES</span></h2>
      <p>Listen to the latest sounds from DJ Ambroy.</p>
    </div>


    <div class="mix-grid">


      <div class="mix-card">

        <div class="mix-image mix1"></div>

        <div class="mix-info">

          <h3>
            UG MONTHLY MIXTAPE SERIES V19
          </h3>

          <p>
            Pure Ugandan vibes — nonstop.
          </p>

          <a href="#" class="listen">
            ▶ Listen
          </a>

        </div>

      </div>


      <div class="mix-card">

        <div class="mix-image mix2"></div>

        <div class="mix-info">

          <h3>
            THE AFRICAN VIBE MIX
          </h3>

          <p>
            African sounds mixed by DJ Ambroy.
          </p>

          <a href="#" class="listen">
            ▶ Listen
          </a>

        </div>

      </div>


      <div class="mix-card">

        <div class="mix-image mix3"></div>

        <div class="mix-info">

          <h3>
            UG LOVE ANTHEMS
          </h3>

          <p>
            Volume 1 — Ugandan love vibes.
          </p>

          <a href="#" class="listen">
            ▶ Listen
          </a>

        </div>

      </div>


    </div>

  </div>

</section>


<!-- YOUTUBE -->

<section class="youtube" id="youtube">

  <div class="container">

    <div class="section-title">
      <h2>WATCH ON <span>YOUTUBE</span></h2>
    </div>

    <div class="youtube-box">

      <h3>
        DJ AMBROY UG
      </h3>

      <p>
        Watch my latest mixtapes, music videos,
        DJ drops and more on YouTube.
      </p>

      <!-- CHANGE THIS LINK TO YOUR REAL YOUTUBE CHANNEL -->

      <a
        href="https://www.youtube.com/"
        target="_blank"
        class="btn youtube-btn">

        ▶ VISIT MY YOUTUBE

      </a>

    </div>

  </div>

</section>


<!-- BOOKING -->

<section class="booking" id="booking">

  <div class="container">

    <div class="section-title">
      <h2>BOOK <span>DJ AMBROY</span></h2>
    </div>

    <div class="booking-box">

      <h3>
        LET'S MAKE SOME NOISE 🔥
      </h3>

      <p>
        Looking for a DJ for your party, wedding,
        club night, birthday or special event?
      </p>

      <p>
        Contact DJ Ambroy for bookings and events.
      </p>

      <!-- CHANGE NUMBER -->

      <a
        href="https://wa.me/256700000000"
        target="_blank"
        class="btn primary">

        📲 BOOK VIA WHATSAPP

      </a>

    </div>

  </div>

</section>


<!-- CONTACT -->

<section class="contact" id="contact">

  <div class="container">

    <div class="section-title">

      <h2>
        CONNECT WITH <span>ME</span>
      </h2>

      <p>
        Follow DJ Ambroy and stay connected.
      </p>

    </div>


    <div class="contact-links">

      <a href="#" target="_blank">
        YouTube
      </a>

      <a href="#" target="_blank">
        Instagram
      </a>

      <a href="#" target="_blank">
        TikTok
      </a>

      <a href="#" target="_blank">
        Facebook
      </a>

    </div>

  </div>

</section>


<!-- FOOTER -->

<footer>

  <p>
    © 2026 <strong>DJ AMBROY UG</strong> —
    MR 5 STAR ⭐
  </p>

  <p>
    No skipping • No stopping • Pure Ugandan vibes
  </p>

</footer>


<!-- WHATSAPP FLOATING BUTTON -->

<a
  class="whatsapp"
  href="https://wa.me/256700000000"
  target="_blank"
  title="Chat with DJ Ambroy">

  ☎

</a>

</body>
</html>
