<!doctype html>
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Clever Minds — We Deliver What Others Just Promise</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --brand-dark:#004848;
      --brand-mid:#77ddaa;
      --brand-light:#e7f1ed;
      --white:#ffffff;
      --muted:#6b7280;
      --container:1100px;
    }
    *{box-sizing:border-box}
    body{font-family:'Nunito Sans',system-ui,Segoe UI,Roboto,Helvetica,Arial,sans-serif;margin:0;color:#0f172a;line-height:1.5}
    a{color:var(--brand-dark);text-decoration:none}
    .container{max-width:var(--container);margin:0 auto;padding:0 20px}

    /* Header / Nav */
    header{background:linear-gradient(180deg,var(--brand-light),rgba(255,255,255,0));}
    .nav{display:flex;justify-content:space-between;align-items:center;padding:18px 0}
    .logo{font-weight:800;color:var(--brand-dark);font-size:20px}
    nav ul{display:flex;gap:18px;list-style:none;margin:0;padding:0}
    nav li{font-weight:700}
    .cta{background:var(--brand-dark);color:var(--white);padding:10px 16px;border-radius:8px}
    .hamb{display:none;background:transparent;border:0;font-size:22px}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 1fr;gap:30px;align-items:center;padding:60px 0}
    .hero h1{font-size:36px;margin:0 0 12px;color:var(--brand-dark)}
    .hero p{color:var(--muted);margin:0 0 18px}
    .hero .btn{background:var(--brand-mid);color:var(--brand-dark);padding:12px 18px;border-radius:10px;font-weight:700}
    .hero img{width:100%;border-radius:12px;box-shadow:0 8px 30px rgba(0,0,0,0.08)}

    /* Sections */
    section{padding:60px 0}
    h2.section-title{font-size:24px;margin:0 0 12px;color:var(--brand-dark)}
    p.lead{color:var(--muted);max-width:70%}

    /* Services */
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:18px;margin-top:24px}
    .card{background:#fff;border-radius:12px;padding:20px;box-shadow:0 6px 18px rgba(2,6,23,0.06);display:flex;flex-direction:column;align-items:center;text-align:center}
    .card img{width:72px;height:72px;object-fit:cover;margin-bottom:12px}
    .card h3{margin:0 0 8px}
    .card p{color:var(--muted);font-size:14px}

    /* Projects slider */
    .slider{position:relative;background:linear-gradient(0deg,var(--brand-light),#fff);padding:18px;border-radius:12px}
    .slides{display:flex;overflow:hidden}
    .slide{min-width:100%;display:flex;gap:18px;align-items:center}
    .slide img{width:45%;border-radius:10px}
    .slide .meta{flex:1}
    .nav-arrows{position:absolute;right:18px;top:50%;transform:translateY(-50%);display:flex;flex-direction:column;gap:10px}
    .nav-arrows button{background:var(--brand-dark);color:#fff;border:0;padding:8px;border-radius:8px}

    /* Facts */
    .facts{display:flex;gap:18px;align-items:center}
    .stat{flex:1;background:linear-gradient(180deg,var(--brand-mid),#fff);padding:24px;border-radius:12px;text-align:center}
    .stat h3{font-size:32px;margin:0;color:var(--brand-dark)}

    /* Team */
    .team-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:16px}
    .member{background:#fff;padding:12px;border-radius:10px;text-align:center}
    .member img{width:100%;border-radius:8px}

    /* Contact */
    .contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px}
    .contact-card{background:var(--brand-dark);color:#fff;padding:20px;border-radius:12px}
    form .field{margin-bottom:12px}
    input,textarea,select{width:100%;padding:12px;border-radius:8px;border:1px solid #e6eef0}
    button[type=submit]{background:var(--brand-dark);color:#fff;padding:12px 18px;border-radius:10px;border:0}

    footer{border-top:1px solid #e6eef0;padding:24px 0}

    /* Responsive */
    @media (max-width:900px){
      .hero{grid-template-columns:1fr;padding:30px 0}
      nav ul{display:none}
      .hamb{display:inline-block}
      .contact-grid{grid-template-columns:1fr}
      .slide img{width:40%}
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="logo">Clever Minds</div>
      <nav>
        <ul id="menu">
          <li><a href="#hero">Home</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#team">Team</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
        <button class="hamb" id="hamb">☰</button>
      </nav>
      <a class="cta" href="#contact">Get Quote</a>
    </div>
  </header>

  <main class="container">
    <!-- Hero -->
    <section id="hero" class="hero">
      <div>
        <h1>We Design & Build Creative Brands</h1>
        <p class="lead">Digital marketing, brand building, web & app development — hum aapke business ko online grow karvate hain.</p>
        <div style="display:flex;gap:12px;flex-wrap:wrap;margin-top:12px">
          <a class="btn" href="#projects">Our Work</a>
          <a class="btn" style="background:transparent;border:2px solid var(--brand-dark);">Case Studies</a>
        </div>
      </div>
      <div>
        <img src="https://placehold.co/800x600" alt="hero image">
      </div>
    </section>

    <!-- Projects / Slider -->
    <section id="projects">
      <h2 class="section-title">Featured Projects</h2>
      <p class="lead">Kuch selected projects jo humne recently complete kiye hain.</p>
      <div class="slider" style="margin-top:18px">
        <div class="slides" id="slides">
          <div class="slide">
            <img src="https://placehold.co/600x600" alt="proj1">
            <div class="meta">
              <h3>Coloca Branding</h3>
              <p>Brand identity, packaging design aur website development ka complete solution.</p>
              <p><strong>Services:</strong> Branding, UI/UX, Social</p>
            </div>
          </div>
          <div class="slide">
            <img src="https://placehold.co/600x600" alt="proj2">
            <div class="meta">
              <h3>Banking App</h3>
              <p>Secure aur user-friendly mobile banking experience design kiya gaya.</p>
              <p><strong>Services:</strong> App design, Prototyping, Testing</p>
            </div>
          </div>
          <div class="slide">
            <img src="https://placehold.co/600x600" alt="proj3">
            <div class="meta">
              <h3>Root Trekkers</h3>
              <p>Travel booking platform ke liye complete brand aur booking flow build kiya.</p>
              <p><strong>Services:</strong> Web, Booking Flow, Marketing</p>
            </div>
          </div>
        </div>
        <div class="nav-arrows">
          <button id="prev">◀</button>
          <button id="next">▶</button>
        </div>
      </div>
    </section>

    <!-- Services -->
    <section id="services">
      <h2 class="section-title">Services</h2>
      <p class="lead">Hum aapko ek hi jagah poora digital solution dete hain — design se lekar growth tak.</p>
      <div class="services">
        <div class="card">
          <img src="https://placehold.co/120x120" alt="marketing">
          <h3>Digital Marketing</h3>
          <p>Paid ads, organic growth, content aur performance marketing.</p>
        </div>
        <div class="card">
          <img src="https://placehold.co/120x120" alt="branding">
          <h3>Branding</h3>
          <p>Logo, identity, packaging aur brand guidelines.</p>
        </div>
        <div class="card">
          <img src="https://placehold.co/120x120" alt="web">
          <h3>Web & App</h3>
          <p>Websites, landing pages aur mobile apps with clean UX.</p>
        </div>
        <div class="card">
          <img src="https://placehold.co/120x120" alt="video">
          <h3>Video & Motion</h3>
          <p>Reels, product videos aur corporate shoots.</p>
        </div>
      </div>
    </section>

    <!-- About -->
    <section id="about">
      <h2 class="section-title">About Us</h2>
      <p class="lead">Clever Minds ek full-service digital agency hai. Hum long-term partnerships banate hain — clients ke sath milke unke business ko scale karte hain.</p>

      <div style="display:flex;gap:18px;flex-wrap:wrap;margin-top:18px">
        <div style="flex:1;min-width:240px;background:var(--brand-light);padding:18px;border-radius:12px">
          <h3 style="margin-top:0">Mission</h3>
          <p style="margin:0;color:var(--muted)">Simple, measurable aur scalable marketing solutions create karna.</p>
        </div>
        <div style="flex:1;min-width:240px;background:linear-gradient(180deg,var(--brand-mid),#fff);padding:18px;border-radius:12px">
          <h3 style="margin-top:0">Vision</h3>
          <p style="margin:0;color:var(--brand-dark)">Clients ko digital me center-stage pe lana.</p>
        </div>
      </div>
    </section>

    <!-- Facts -->
    <section id="facts">
      <h2 class="section-title">Key Facts</h2>
      <div class="facts" style="margin-top:18px">
        <div class="stat">
          <h3>75</h3>
          <p>Successful Projects</p>
        </div>
        <div class="stat">
          <h3>24</h3>
          <p>Employees</p>
        </div>
        <div class="stat">
          <h3>16</h3>
          <p>Years</p>
        </div>
      </div>
    </section>

    <!-- Team -->
    <section id="team">
      <h2 class="section-title">Our Team</h2>
      <div class="team-grid" style="margin-top:18px">
        <div class="member"><img src="https://placehold.co/400x400" alt="team"><h4 style="margin:8px 0 4px">Usama Seth</h4><p style="color:var(--muted);margin:0">Founder</p></div>
        <div class="member"><img src="https://placehold.co/400x400" alt="team"><h4 style="margin:8px 0 4px">Khalid</h4><p style="color:var(--muted);margin:0">Head - Ads</p></div>
        <div class="member"><img src="https://placehold.co/400x400" alt="team"><h4 style="margin:8px 0 4px">Video Editor</h4><p style="color:var(--muted);margin:0">Production</p></div>
        <div class="member"><img src="https://placehold.co/400x400" alt="team"><h4 style="margin:8px 0 4px">Designer</h4><p style="color:var(--muted);margin:0">UI/UX</p></div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact">
      <h2 class="section-title">Contact</h2>
      <div class="contact-grid" style="margin-top:18px">
        <div class="contact-card">
          <h3 style="margin-top:0;color:var(--brand-light)">Let's talk</h3>
          <p style="color:var(--brand-light)">Phone: <strong>+91 55-873-1234</strong><br>Email: <strong>hello@cleverminds.com</strong></p>
          <p style="color:var(--brand-light)">Address: Vadodara, Gujarat</p>
        </div>
        <div>
          <form id="contactForm" class="contact-form" onsubmit="return submitForm(event)">
            <div class="field"><input required id="name" placeholder="Full Name"></div>
            <div class="field"><input required type="email" id="email" placeholder="Email Address"></div>
            <div class="field">
              <select id="reason"><option>Reason for contacting us</option><option>Quote request</option><option>Collaboration</option><option>Other</option></select>
            </div>
            <div class="field"><textarea id="message" rows="4" placeholder="Message"></textarea></div>
            <div class="field"><button type="submit">Send Message</button></div>
          </form>
        </div>
      </div>
    </section>

  </main>

  <footer class="container">
    <div style="display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:12px">
      <div>
        <strong>Clever Minds</strong>
        <div style="color:var(--muted)">We Deliver What Others Just Promise.</div>
      </div>
      <div style="color:var(--muted)">© " + new Date().getFullYear() + " Clever Minds</div>
    </div>
  </footer>

  <script>
    // Mobile menu
    const hamb=document.getElementById('hamb');
    const menu=document.getElementById('menu');
    hamb.addEventListener('click',()=>{
      if(menu.style.display === 'flex') menu.style.display='none'; else menu.style.display='flex';
      menu.style.flexDirection='column';menu.style.background='#fff';menu.style.padding='12px';menu.style.position='absolute';menu.style.right='18px';menu.style.top='64px';menu.style.borderRadius='8px';menu.style.boxShadow='0 8px 30px rgba(2,6,23,0.08)';
    });

    // Simple slider
    const slidesWrap = document.getElementById('slides');
    const slides = Array.from(slidesWrap.children);
    let index = 0;
    function showSlide(i){
      if(i<0) i = slides.length-1;
      if(i>=slides.length) i = 0;
      index = i;
      slidesWrap.style.transform = 'translateX(' + (-index*100) + '%)';
      slidesWrap.style.transition='transform 450ms ease';
    }
    document.getElementById('prev').addEventListener('click',()=>showSlide(index-1));
    document.getElementById('next').addEventListener('click',()=>showSlide(index+1));
    // auto rotate
    setInterval(()=>showSlide(index+1),6000);

    // Smooth scroll for anchors
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click',function(e){
        const href=this.getAttribute('href');
        if(href.length>1){
          e.preventDefault();
          document.querySelector(href).scrollIntoView({behavior:'smooth',block:'start'});
        }
      })
    })

    // Contact form (local demo)
    function submitForm(e){
      e.preventDefault();
      const name=document.getElementById('name').value.trim();
      const email=document.getElementById('email').value.trim();
      const msg=document.getElementById('message').value.trim();
      if(!name||!email){alert('Please fill name and email');return false}
      alert('Thank you, ' + name + '! Message received. We will contact you soon.');
      document.getElementById('contactForm').reset();
      return false;
    }

    // Footer year fix (since template used JS in string)
    document.addEventListener('DOMContentLoaded',()=>{
      const footer = document.querySelector('footer div div:last-child');
      if(footer) footer.textContent = '© ' + new Date().getFullYear() + ' Clever Minds';
    })
  </script>
</body>
</html>
