# Html-code-to-create-a-home-page-having-three-links-about-us-our-services-contact-us-
About us,our services, contact us
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Home - My Website</title>
  <style>
    :root{
      --bg:#f8fafc; --card:#ffffff; --accent:#0066cc; --muted:#666;
      --radius:12px;
    }
    *{box-sizing:border-box}
    body{
      margin:0; font-family:system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background:var(--bg); color:#111;
      -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
    }
    header{
      background:linear-gradient(90deg, rgba(0,102,204,0.06), rgba(0,102,204,0.02));
      padding:18px 20px; display:flex; align-items:center; justify-content:space-between;
      gap:20px;
    }
    .brand{font-weight:700; color:var(--accent); font-size:1.2rem}
    nav a{
      text-decoration:none; margin-left:14px; color:var(--accent); font-weight:600;
    }
    .container{max-width:1000px; margin:28px auto; padding:0 18px;}
    .hero{
      background:var(--card); padding:28px; border-radius:var(--radius); box-shadow:0 6px 18px rgba(11,20,40,0.05);
      display:flex; gap:24px; align-items:center;
    }
    .hero h1{margin:0; font-size:1.6rem}
    .links {display:flex; gap:12px; margin-top:12px}
    .btn{
      display:inline-block; padding:10px 14px; border-radius:10px; text-decoration:none;
      background:transparent; border:2px solid var(--accent); color:var(--accent); font-weight:700;
    }
    main {margin-top:20px; display:grid; gap:18px;}
    .card{background:var(--card); padding:16px; border-radius:12px; box-shadow:0 6px 18px rgba(11,20,40,0.04);}
    footer{margin-top:24px; text-align:center; color:var(--muted); padding:18px 8px;}
    /* Responsive */
    @media (max-width:700px){
      .hero{flex-direction:column; text-align:center}
      nav a{margin-left:8px; display:inline-block}
    }
  </style>
</head>
<body>
  <header>
    <div class="brand">MySite</div>
    <nav aria-label="Main navigation">
      <a href="about.html">About Us</a>
      <a href="services.html">Our Services</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>

  <div class="container">
    <section class="hero" aria-labelledby="welcome">
      <div>
        <h1 id="welcome">Welcome to MySite</h1>
        <p style="color:var(--muted); margin-top:8px">
          We create simple and elegant web experiences. Click the links to learn more.
        </p>
        <div class="links">
          <a class="btn" href="about.html">About Us</a>
          <a class="btn" href="services.html">Our Services</a>
          <a class="btn" href="contact.html">Contact Us</a>
        </div>
      </div>
      <img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='160' height='120'%3E%3Crect fill='%230066cc' rx='12' width='160' height='120'/%3E%3Ctext x='50%25' y='50%25' fill='white' font-size='18' font-family='Arial' dominant-baseline='middle' text-anchor='middle'%3EWelcome%3C/text%3E%3C/svg%3E" alt="" width="160" height="120" style="border-radius:10px; object-fit:cover">
    </section>

    <main>
      <div class="card">
        <h2>Quick Links</h2>
        <p style="color:var(--muted)">Jump to important pages:</p>
        <ul>
          <li><a href="about.html">About Us</a></li>
          <li><a href="services.html">Our Services</a></li>
          <li><a href="contact.html">Contact Us</a></li>
        </ul>
      </div>

      <div class="card">
        <h2>Get started</h2>
        <p style="color:var(--muted)">Want a custom site? Reach out through the contact page and we'll reply within 1–2 business days.</p>
      </div>
    </main>

    <footer>
      © <span id="year"></span> MySite · Built with 
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>