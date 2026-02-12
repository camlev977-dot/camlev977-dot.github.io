<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Blossom Social</title>
  <meta name="description" content="Blossom Social — social media + Google Business Profile management for small businesses." />
  <style>
    :root{
      --bg:#fff7fb;
      --panel: rgba(255,255,255,.78);
      --text:#1c1020;
      --muted:#5b4a61;
      --pink:#ff4fa3;
      --pink2:#ff7bc2;
      --border: rgba(28,16,32,.12);
      --shadow: 0 18px 60px rgba(28,16,32,.12);
      --radius: 18px;
      --max: 980px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
      color:var(--text);
      background:
        radial-gradient(900px 500px at 15% 10%, rgba(255,79,163,.20), transparent 60%),
        radial-gradient(800px 450px at 85% 20%, rgba(255,123,194,.18), transparent 60%),
        radial-gradient(900px 550px at 50% 100%, rgba(255,79,163,.12), transparent 65%),
        var(--bg);
      line-height:1.5;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max); margin:0 auto; padding: 0 18px;}
    header{
      position:sticky; top:0; z-index:50;
      backdrop-filter: blur(10px);
      background: rgba(255,247,251,.75);
      border-bottom: 1px solid var(--border);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between;
      padding: 14px 0;
      gap: 12px;
    }
    .brand{
      display:flex; align-items:center; gap:10px;
      font-weight:900; letter-spacing:.2px;
    }
    .mark{
      width:12px;height:12px;border-radius:999px;
      background: linear-gradient(135deg, var(--pink), var(--pink2));
      box-shadow: 0 0 18px rgba(255,79,163,.35);
    }
    .links{display:flex; gap:14px; color:var(--muted); font-weight:700;}
    .links a{padding:8px 10px;border-radius:12px}
    .links a:hover{background: rgba(28,16,32,.06); color:var(--text)}
    .cta{
      display:inline-flex; align-items:center; justify-content:center;
      padding: 10px 14px;
      border-radius: 14px;
      border: 1px solid rgba(255,79,163,.35);
      background: linear-gradient(135deg, var(--pink), var(--pink2));
      color:#fff;
      font-weight:900;
      box-shadow: 0 12px 40px rgba(255,79,163,.18);
      white-space:nowrap;
    }
    .cta:hover{filter:brightness(1.03)}
    .card{
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .hero{padding: 42px 0 18px;}
    h1{
      margin: 0 0 10px;
      font-size: clamp(34px, 4.2vw, 54px);
      line-height:1.05;
      letter-spacing:-.6px;
    }
    .lead{margin: 0 0 18px; color:var(--muted); font-size: 16.5px; max-width: 56ch;}
    .hero-inner{padding: 26px;}
    .badges{display:flex; gap:10px; flex-wrap:wrap; margin-bottom: 12px;}
    .badge{
      font-size: 12px; font-weight:900; letter-spacing:.3px;
      padding: 6px 10px; border-radius: 999px;
      border: 1px solid rgba(255,79,163,.28);
      background: rgba(255,79,163,.10);
    }
    .actions{display:flex; gap:12px; flex-wrap:wrap}
    .ghost{
      display:inline-flex; align-items:center; justify-content:center;
      padding: 10px 14px; border-radius: 14px;
      border: 1px solid rgba(28,16,32,.16);
      background: rgba(255,255,255,.55);
      font-weight:900;
    }
    .ghost:hover{background: rgba(255,255,255,.85)}
    .grid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 14px;
      padding: 14px 0;
    }
    @media (max-width: 860px){
      .links{display:none}
      .grid{grid-template-columns: 1fr}
    }
    h2{margin: 0 0 10px; font-size: 20px;}
    .mini{padding: 18px; min-height: 140px}
    .mini h3{margin: 0 0 6px; font-size: 16px}
    .mini p{margin:0; color:var(--muted)}
    .pricing{padding: 18px}
    .price{
      display:flex; align-items:baseline; gap:10px; flex-wrap:wrap;
      margin: 6px 0 10px;
    }
    .amount{
      font-size: 34px; font-weight:1000; letter-spacing:-.3px;
    }
    .per{color:var(--muted); font-weight:800}
    ul{margin: 10px 0 0; padding-left: 18px; color:var(--muted)}
    li{margin: 6px 0}
    .callout{
      margin-top: 12px;
      padding: 12px 14px;
      border-radius: 14px;
      border: 1px dashed rgba(255,79,163,.45);
      background: rgba(255,79,163,.08);
      font-weight:800;
      color: #3a1130;
    }
    .contact{padding: 18px}
    input, textarea{
      width:100%;
      padding: 12px 12px;
      border-radius: 14px;
      border: 1px solid rgba(28,16,32,.16);
      background: rgba(255,255,255,.7);
      color:var(--text);
      outline:none;
      margin-top: 10px;
      font-size: 14.5px;
    }
    textarea{min-height: 110px; resize: vertical}
    input:focus, textarea:focus{
      border-color: rgba(255,79,163,.65);
      box-shadow: 0 0 0 4px rgba(255,79,163,.18);
    }
    .footer{
      padding: 26px 0 36px;
      color:var(--muted);
      border-top: 1px solid var(--border);
      margin-top: 18px;
      font-size: 13px;
    }
    .note{font-size: 12.5px; color: var(--muted); margin-top: 10px}
  </style>
</head>

<body>
  <header>
    <div class="wrap nav">
      <a class="brand" href="#top" aria-label="Blossom Social Home">
        <span class="mark"></span>
        <span>BLOSSOM SOCIAL</span>
      </a>

      <nav class="links" aria-label="Primary">
        <a href="#services">Services</a>
        <a href="#pricing">Pricing</a>
        <a href="#contact">Contact</a>
      </nav>

      <a class="cta" href="#contact">Get Started</a>
    </div>
  </header>

  <main id="top" class="wrap">
    <!-- HERO -->
    <section class="hero">
      <div class="card hero-inner">
        <div class="badges">
          <span class="badge">Google Business Profile</span>
          <span class="badge">Facebook + Instagram</span>
          <span class="badge">Small Business Friendly</span>
        </div>

        <h1>Grow, glow, and blossom online. 🌸</h1>
        <p class="lead">
          Blossom Social helps local businesses stay visible and consistent with clean content + Google updates
          that bring in real customers.
        </p>

        <div class="actions">
          <a class="cta" href="#contact">Request a Quote</a>
          <a class="ghost" href="#pricing">See Pricing</a>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services">
      <h2>What I do</h2>
      <div class="grid">
        <div class="card mini">
          <h3>GBP setup + optimization</h3>
          <p>Fix your info, categories, services, photos, and keywords so you show up locally.</p>
        </div>
        <div class="card mini">
          <h3>Weekly Google posts</h3>
          <p>Offers, updates, photos—so your profile looks active (and trustworthy).</p>
        </div>
        <div class="card mini">
          <h3>FB + IG content</h3>
          <p>Simple, aesthetic posts that match your brand and keep you consistent.</p>
        </div>
      </div>
    </section>

    <!-- PRICING -->
    <section id="pricing" style="padding-top:10px;">
      <h2>Pricing</h2>
      <div class="card pricing">
        <div class="price">
          <div class="amount">$250</div>
          <div class="per">/ month</div>
          <div class="badge" style="border-color:rgba(28,16,32,.12); background:rgba(255,255,255,.55); color:var(--muted);">
            GBP + weekly posts + FB/IG content
          </div>
        </div>

        <ul>
          <li>Google Business Profile setup + optimization</li>
          <li>Weekly Google posts</li>
          <li>Facebook & Instagram content</li>
        </ul>

        <div class="callout">
          🔥 Intro Special: 3 months for $500 (Buy 2, Get 1 FREE!)
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" style="padding: 14px 0 4px;">
      <h2>Contact</h2>
      <div class="card contact">
        <form id="contactForm">
          <label class="note">Name</label>
          <input name="name" placeholder="Your name" required />

          <label class="note">Email</label>
          <input name="email" type="email" placeholder="you@email.com" required />

          <label class="note">What do you need help with?</label>
          <textarea name="message" placeholder="GBP help, posting, full management, etc." required></textarea>

          <div style="display:flex; gap:12px; flex-wrap:wrap; margin-top:12px;">
            <button class="cta" type="submit">Send</button>
            <a class="ghost" href="tel:+10000000000">Call/Text</a>
            <a class="ghost" href="https://instagram.com/" target="_blank" rel="noreferrer">Instagram</a>
          </div>

          <p class="note">Tip: replace the phone + Instagram link with your real info.</p>
        </form>
      </div>
    </section>

    <div class="footer">
      © <span id="year"></span> Blossom Social • Built for small businesses.
    </div>
  </main>

  <script>
    // Set footer year
    document.getElementById("year").textContent = new Date().getFullYear();

    // Tiny "mail to" fallback so the form works without a backend
    document.getElementById("contactForm").addEventListener("submit", function(e){
      e.preventDefault();
      const data = new FormData(e.target);
      const name = encodeURIComponent(data.get("name"));
      const email = encodeURIComponent(data.get("email"));
      const msg = encodeURIComponent(data.get("message"));

      const subject = encodeURIComponent("Blossom Social Inquiry");
      const body = encodeURIComponent(
        `Name: ${decodeURIComponent(name)}\nEmail: ${decodeURIComponent(email)}\n\nMessage:\n${decodeURIComponent(msg)}`
      );

      // Replace with your email:
      const yourEmail = "you@yourdomain.com";
      window.location.href = `mailto:${yourEmail}?subject=${subject}&body=${body}`;
    });
  </script>
</body>
</html>
