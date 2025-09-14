# Portfolio007
Company profile
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portfolio Landing — Starter Template</title>
  <meta name="description" content="A clean, fast portfolio landing page you can clone and customize in minutes." />
  <meta property="og:title" content="Portfolio Landing — Starter Template" />
  <meta property="og:description" content="Responsive, accessible, single-file portfolio landing page." />
  <meta property="og:type" content="website" />
  <meta name="color-scheme" content="light dark" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Instrument+Sans:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b0c10; --surface:#12131a; --text:#e7eaf0; --muted:#9aa3b2; --primary:#16a34a; --ring:#86efac;
      --lbg:#f8fafc; --lsurface:#ffffff; --ltext:#0b1220; --lmuted:#475569; --primary-2:#0ea5e9;
      --r:18px; --shadow:0 10px 30px rgba(0,0,0,.15); --max:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{margin:0;font-family:"Instrument Sans",system-ui,Segoe UI,Roboto,Helvetica,Arial,sans-serif;background:var(--lbg);color:var(--ltext);line-height:1.6}
    .dark body{background:var(--bg);color:var(--text)}
    a{color:inherit;text-decoration:none}
    img{max-width:100%;display:block}
    .container{max-width:var(--max);margin:0 auto;padding:0 20px}
    header{position:sticky;top:0;z-index:40;backdrop-filter:saturate(180%) blur(10px);background:color-mix(in srgb,var(--lsurface) 85%,transparent);border-bottom:1px solid #e5e7eb}
    .dark header{background:color-mix(in srgb,var(--surface) 85%,transparent);border-bottom-color:#1f2937}
    nav{height:64px;display:flex;align-items:center;justify-content:space-between}
    .brand{font-weight:800;letter-spacing:.2px}
    .nav-links{display:flex;gap:16px;align-items:center}
    .btn{display:inline-flex;align-items:center;gap:8px;padding:10px 14px;border-radius:12px;border:1px solid #e5e7eb;background:var(--lsurface);font-weight:600;transition:.2s}
    .btn:hover{transform:translateY(-1px)}
    .dark .btn{border-color:#1f2937;background:#0e1016}
    .btn.primary{border:none;background:linear-gradient(135deg,var(--primary),var(--primary-2));color:white;box-shadow:0 10px 20px rgba(16,185,129,.25)}
    .theme-toggle{cursor:pointer;border:1px solid #e5e7eb;border-radius:12px;padding:8px 12px}
    .dark .theme-toggle{border-color:#1f2937}

    /* Hero */
    .hero{padding:80px 0 40px}
    .hero-grid{display:grid;grid-template-columns:1.1fr .9fr;gap:36px;align-items:center}
    h1{font-size:clamp(34px,5vw,56px);line-height:1.08;margin:10px 0}
    .lead{font-size:18px;color:var(--lmuted)}
    .dark .lead{color:var(--muted)}
    .pill{display:inline-block;padding:6px 10px;border-radius:999px;border:1px solid #e5e7eb;background:var(--lsurface);font-size:12px}
    .dark .pill{border-color:#1f2937;background:#0e1016}
    .card{border:1px solid #e5e7eb;border-radius:var(--r);padding:18px;background:var(--lsurface);box-shadow:var(--shadow)}
    .dark .card{border-color:#1f2937;background:#0e1016}

    /* Sections */
    section{padding:54px 0}
    .section-head{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px}
    .section-title{font-weight:800;font-size:22px}
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}
    @media (max-width:900px){.hero-grid{grid-template-columns:1fr}.grid.cols-3{grid-template-columns:1fr 1fr}.grid.cols-2{grid-template-columns:1fr}}
    @media (max-width:620px){.grid.cols-3{grid-template-columns:1fr}}
    .tile{border:1px solid #e5e7eb;border-radius:16px;padding:16px;background:var(--lsurface);transition:.2s}
    .tile:hover{transform:translateY(-2px)}
    .dark .tile{border-color:#1f2937;background:#0f1116}
    .eyebrow{font-size:12px;letter-spacing:.3px;color:var(--lmuted)}
    .dark .eyebrow{color:var(--muted)}

    /* Gallery */
    .gallery{display:grid;grid-template-columns:2fr 1fr 1fr;gap:12px}
    .gallery img{border-radius:14px;height:100%;object-fit:cover}
    @media (max-width:900px){.gallery{grid-template-columns:1fr 1fr}}

    /* Footer */
    footer{padding:36px 0;border-top:1px solid #e5e7eb;color:var(--lmuted)}
    .dark footer{border-color:#1f2937;color:var(--muted)}
  </style>
</head>
<body>
  <header>
    <div class="container">
      <nav>
        <span class="brand">Your Name</span>
        <div class="nav-links">
          <a href="#work">Work</a>
          <a href="#services">Services</a>
          <a href="#about">About</a>
          <a href="#contact">Contact</a>
          <button id="themeToggle" class="theme-toggle" aria-label="Toggle theme">🌓</button>
        </div>
      </nav>
    </div>
  </header>

  <main>
    <!-- HERO -->
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="pill">Portfolio Landing Template</span>
          <h1>Designing & building clean, fast websites that feel effortless.</h1>
          <p class="lead">Use this single-file template to launch your portfolio in minutes. Replace the text, drop in your images, and deploy to GitHub Pages — no build tools required.</p>
          <div style="display:flex;gap:12px;flex-wrap:wrap;margin-top:16px">
            <a class="btn primary" href="#contact">Start a project</a>
            <a class="btn" href="#work">See my work</a>
            <a class="btn" href="https://github.com/" target="_blank" rel="noopener">GitHub</a>
          </div>
        </div>
        <div>
          <div class="card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1200&auto=format&fit=crop" alt="Mockup of a clean website design" />
          </div>
        </div>
      </div>
    </section>

    <!-- TRUST / METRICS -->
    <section>
      <div class="container grid cols-3">
        <div class="tile"><div class="eyebrow">Experience</div><div style="font-size:28px;font-weight:800">5+ years</div><p>Design, WordPress, and content.</p></div>
        <div class="tile"><div class="eyebrow">Projects</div><div style="font-size:28px;font-weight:800">120+</div><p>Sites, landings, and brand pages.</p></div>
        <div class="tile"><div class="eyebrow">Clients</div><div style="font-size:28px;font-weight:800">Global</div><p>Portugal, UK, Pakistan, and beyond.</p></div>
      </div>
    </section>

    <!-- WORK / CASES -->
    <section id="work">
      <div class="container">
        <div class="section-head">
          <h2 class="section-title">Featured work</h2>
          <a class="btn" href="https://github.com/" target="_blank">All projects</a>
        </div>
        <div class="grid cols-2">
          <article class="tile">
            <h3 style="margin:6px 0">Conversion-focused SaaS landing</h3>
            <p>Hero with clear value prop, social proof, and crisp CTA. Optimized for speed and readability.</p>
            <div class="gallery" style="margin-top:10px">
              <img src="https://images.unsplash.com/photo-1553532070-9b3b4c2bcb43?q=80&w=800&auto=format&fit=crop" alt="Landing screenshot 1" />
              <img src="https://images.unsplash.com/photo-1519999482648-25049ddd37b1?q=80&w=800&auto=format&fit=crop" alt="Landing screenshot 2" />
              <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?q=80&w=800&auto=format&fit=crop" alt="Landing screenshot 3" />
            </div>
            <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
              <span class="pill">HTML/CSS</span>
              <span class="pill">Accessibility</span>
              <span class="pill">SEO</span>
            </div>
          </article>
          <article class="tile">
            <h3 style="margin:6px 0">WordPress portfolio & blog</h3>
            <p>Custom theme tweaks, navigation revamp, and content architecture that keeps visitors engaged.</p>
            <div class="gallery" style="margin-top:10px">
              <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?q=80&w=800&auto=format&fit=crop" alt="Portfolio screenshot 1" />
              <img src="https://images.unsplash.com/photo-1523906834658-6e24ef2386f9?q=80&w=800&auto=format&fit=crop" alt="Portfolio screenshot 2" />
              <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=800&auto=format&fit=crop" alt="Portfolio screenshot 3" />
            </div>
            <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
              <span class="pill">WordPress</span>
              <span class="pill">UI/UX</span>
              <span class="pill">Performance</span>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services">
      <div class="container">
        <div class="section-head"><h2 class="section-title">Services</h2></div>
        <div class="grid cols-3">
          <div class="tile">
            <h3>Landing Pages</h3>
            <p>High-conversion layouts with clear messaging and strong calls to action.</p>
          </div>
          <div class="tile">
            <h3>WordPress Sites</h3>
            <p>Custom themes, plugins, and speed optimization for business growth.</p>
          </div>
          <div class="tile">
            <h3>UI/UX Design</h3>
            <p>Wireframes to polished interfaces focused on clarity and usability.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about">
      <div class="container grid cols-2">
        <div>
          <h2 class="section-title">About me</h2>
          <p>I’m a designer/developer who loves simple, fast, and thoughtfully crafted web experiences. I combine design clarity with technical execution to ship websites that convert and feel great.</p>
          <p>Available for freelance and full‑time work. Based in Porto, working worldwide.</p>
        </div>
        <div class="tile">
          <h3 style="margin:0 0 8px">Highlights</h3>
          <ul>
            <li>Performance-first approach (Core Web Vitals).</li>
            <li>Accessible by default (semantic HTML, focus states).</li>
            <li>Zero-build workflow — deploy from a single file.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <div class="container grid cols-2">
        <form class="tile" onsubmit="return sendMail(event)">
          <label>Name<br><input class="input" name="name" required style="width:100%;padding:12px 14px;border-radius:12px;border:1px solid #e5e7eb;background:var(--lsurface)"></label>
          <div style="height:12px"></div>
          <label>Email<br><input class="input" name="email" type="email" required style="width:100%;padding:12px 14px;border-radius:12px;border:1px solid #e5e7eb;background:var(--lsurface)"></label>
          <div style="height:12px"></div>
          <label>Message<br><textarea class="input" name="message" required style="width:100%;min-height:120px;padding:12px 14px;border-radius:12px;border:1px solid #e5e7eb;background:var(--lsurface)"></textarea></label>
          <div style="height:12px"></div>
          <button class="btn primary" type="submit">Send message</button>
          <p class="eyebrow" style="margin-top:10px">Demo uses <code>mailto:</code>. Replace with Formspree or your backend for production.</p>
        </form>
        <div class="tile">
          <h3>Find me</h3>
          <p><a href="mailto:your@email.com">your@email.com</a><br>
             <a href="https://www.linkedin.com/" target="_blank" rel="noopener">LinkedIn</a> · <a href="https://github.com/" target="_blank" rel="noopener">GitHub</a>
          </p>
          <h3>Currently</h3>
          <p>Shipping portfolio landings and helping founders launch fast.</p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container" style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap">
      <small>© <span id="year"></span> Your Name</small>
      <a class="btn" href="#top">Back to top ↑</a>
    </div>
  </footer>

  <script>
    // Theme toggle
    const prefDark = window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches;
    const saved = localStorage.getItem('theme');
    if(saved === 'dark' || (!saved && prefDark)) document.documentElement.classList.add('dark');
    document.getElementById('themeToggle').addEventListener('click',()=>{
      document.documentElement.classList.toggle('dark');
      localStorage.setItem('theme', document.documentElement.classList.contains('dark') ? 'dark' : 'light');
    });

    // Year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Mailto handler
    function sendMail(e){
      e.preventDefault();
      const f = new FormData(e.target);
      const subject = encodeURIComponent('New inquiry from ' + f.get('name'));
      const body = encodeURIComponent(`Name: ${f.get('name')}\nEmail: ${f.get('email')}\n\n${f.get('message')}`);
      window.location.href = `mailto:your@email.com?subject=${subject}&body=${body}`;
      alert('Thanks! Your email client should open now.');
      e.target.reset();
      return false;
    }
  </script>
</body>
</html>


