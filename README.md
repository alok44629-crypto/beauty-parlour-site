# beauty-parlour-site
<!DOCTYPE html>
<html lang="en-IN">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Radiant Glow Beauty Parlour — Gadarpur, Uttarakhand</title>
  <meta name="description" content="Radiant Glow Beauty Parlour in Gadarpur offers bridal makeup, facials, hair styling, manicure & pedicure, waxing, and spa treatments. Book your appointment online or WhatsApp us." />
  <meta name="theme-color" content="#e91e63" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
  <meta property="og:title" content="Radiant Glow Beauty Parlour — Gadarpur" />
  <meta property="og:description" content="Bridal makeup, facials, hair, nails, and spa. Book your glow." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="images/og-image.jpg" />
  <meta property="og:url" content="https://your-domain.com/" />
  <style>
    :root{
      --accent:#e91e63;
      --accent-2:#ff7aa2;
      --dark:#1b1b1f;
      --text:#2a2a2f;
      --muted:#6a6a73;
      --bg:#fff9fb;
      --card:#ffffff;
      --ring: rgba(233,30,99,.35);
      --radius:14px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;color:var(--text);background:var(--bg);scroll-behavior:smooth}
    a{color:var(--accent);text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1100px,92%);margin-inline:auto}
    .btn{display:inline-block;padding:12px 18px;border-radius:999px;background:var(--accent);color:#fff;font-weight:600;border:2px solid var(--accent);transition:.2s}
    .btn:hover{transform:translateY(-1px);box-shadow:0 8px 24px -8px var(--ring)}
    .btn.outline{background:transparent;color:var(--accent)}
    /* header */
    header{position:sticky;top:0;z-index:50;background:#ffffffcc;backdrop-filter:blur(10px);border-bottom:1px solid #f1d9e3}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
    .brand{display:flex;align-items:center;gap:10px}
    .logo{width:36px;height:36px;border-radius:50%;background: radial-gradient(120% 100% at 0 0,var(--accent),var(--accent-2));box-shadow:0 6px 20px -8px var(--ring)}
    .brand h1{font-size:18px;margin:0}
    .menu{display:flex;gap:18px;align-items:center}
    .menu a{color:var(--text);font-weight:500}
    .hamburger{display:none;background:none;border:none;font-size:24px}
    @media (max-width: 820px){
      .menu{display:none;position:absolute;top:64px;left:0;right:0;background:#fff;border-bottom:1px solid #f1d9e3;padding:14px;flex-direction:column}
      .menu.open{display:flex}
      .hamburger{display:block}
    }
    /* hero */
    .hero{display:grid;grid-template-columns:1.2fr 1fr;gap:40px;align-items:center;padding:48px 0}
    .hero h2{font-size:42px;line-height:1.15;margin:0 0 12px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .badge{display:inline-flex;align-items:center;gap:8px;padding:6px 12px;border-radius:999px;background:#fff;border:1px solid #fde1ea;color:var(--accent);font-weight:600;margin-bottom:10px}
    .hero-card{background:linear-gradient(160deg,#ffe8f0, #fff);border:1px solid #f8c8d8;border-radius:var(--radius);padding:16px;box-shadow:0 16px 40px -24px var(--ring)}
    .hero-img{aspect-ratio:4/3;border-radius:12px;object-fit:cover}
    .cta-row{display:flex;gap:12px;align-items:center;flex-wrap:wrap;margin-top:8px}
    /* sections */
    section{padding:56px 0}
    .section-title{display:flex;align-items:end;justify-content:space-between;margin-bottom:18px}
    h3{margin:0;font-size:28px}
    .sub{color:var(--muted)}
    .grid{display:grid;gap:16px}
    .grid-3{grid-template-columns:repeat(3,1fr)}
    .grid-2{grid-template-columns:repeat(2,1fr)}
    @media (max-width:900px){.hero{grid-template-columns:1fr}.grid-3{grid-template-columns:1fr}.grid-2{grid-template-columns:1fr}}
    .card{background:var(--card);border:1px solid #f3d2de;border-radius:var(--radius);padding:16px;box-shadow:0 10px 30px -22px var(--ring)}
    .card h4{margin:0 0 6px;font-size:18px}
    .muted{color:var(--muted);font-size:14px}
    .price{font-weight:700;color:var(--accent)}
    .gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
    .gallery img{aspect-ratio:1/1;border-radius:12px;object-fit:cover;border:1px solid #f3d2de}
    @media (max-width:700px){.gallery{grid-template-columns:repeat(2,1fr)}}
    .testimonial{display:flex;gap:12px}
    .avatar{width:44px;height:44px;border-radius:50%;background:#ffe6ef}
    .pill{display:inline-block;padding:4px 10px;border:1px dashed #f3b7cb;border-radius:999px;color:var(--accent);font-size:12px}
    /* booking */
    form{display:grid;gap:12px}
    input,select,textarea{width:100%;padding:12px;border-radius:10px;border:1px solid #f3d2de;background:#fff;outline:none}
    input:focus,select:focus,textarea:focus{border-color:var(--accent);box-shadow:0 0 0 4px var(--ring)}
    textarea{min-height:110px;resize:vertical}
    .two{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    @media (max-width:700px){.two{grid-template-columns:1fr}}
    /* contact */
    .contact-list{display:grid;grid-template-columns:repeat(4,1fr);gap:12px}
    @media (max-width:900px){.contact-list{grid-template-columns:1fr 1fr}}
    @media (max-width:520px){.contact-list{grid-template-columns:1fr}}
    footer{padding:28px 0;color:#8a8a93;text-align:center}
    .floating-whatsapp{position:fixed;right:18px;bottom:18px;background:#25D366;color:#fff;padding:12px 16px;border-radius:999px;font-weight:700;box-shadow:0 12px 28px -16px rgba(0,0,0,.3)}
  </style>
</head>
<body>
  <a href="#main" class="visually-hidden">Skip to content</a>
  <header>
    <div class="container nav" role="navigation" aria-label="Main">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <h1>Radiant Glow</h1>
      </div>
      <button class="hamburger" aria-label="Toggle menu" onclick="document.querySelector('.menu').classList.toggle('open')">☰</button>
      <nav class="menu">
        <a href="#services">Services</a>
        <a href="#gallery">Gallery</a>
        <a href="#testimonials">Reviews</a>
        <a href="#booking">Book</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main id="main">
    <section class="hero container" aria-label="Intro">
      <div>
        <span class="badge">✨ Gadarpur • Since 2017</span>
        <h2>Glow that feels like you.</h2>
        <p>Bridal looks, signature facials, precision hair, and soothing spa rituals. Trusted hands, premium products, and results that last.</p>
        <div class="cta-row">
          <a href="#booking" class="btn">Book an appointment</a>
          <a href="https://wa.me/91XXXXXXXXXX?text=Hi%20Radiant%20Glow%2C%20I%27d%20like%20to%20book%20an%20appointment." class="btn outline" target="_blank" rel="noopener">WhatsApp us</a>
          <span class="pill">Open today 10:00–19:30</span>
        </div>
      </div>
      <div class="hero-card">
        <img src="images/hero.jpg" alt="Makeup artist finishing a soft glam bridal look" class="hero-img">
      </div>
    </section>

    <section id="services" class="container" aria-label="Services">
      <div class="section-title">
        <h3>Our services</h3>
        <span class="sub">Transparent pricing in ₹</span>
      </div>
      <div class="grid grid-3">
        <div class="card">
          <h4>Haircut & Styling</h4>
          <p class="muted">Wash, cut, blow‑dry, and finish.</p>
          <p class="price">₹499–₹1,199</p>
        </div>
        <div class="card">
          <h4>Bridal Makeup</h4>
          <p class="muted">HD/Airbrush with draping & styling.</p>
          <p class="price">₹8,999–₹18,999</p>
        </div>
        <div class="card">
          <h4>Facial Treatments</h4>
          <p class="muted">De‑tan, clean‑up, glow & anti‑ageing.</p>
          <p class="price">₹799–₹3,499</p>
        </div>
        <div class="card">
          <h4>Manicure & Pedicure</h4>
          <p class="muted">Classic, gel, spa rituals.</p>
          <p class="price">₹399–₹1,599</p>
        </div>
        <div class="card">
          <h4>Waxing & Threading</h4>
          <p class="muted">Honey, chocolate, Rica options.</p>
          <p class="price">₹49–₹1,499</p>
        </div>
        <div class="card">
          <h4>Spa & Massage</h4>
          <p class="muted">Head, shoulder, and back relief.</p>
          <p class="price">₹599–₹1,999</p>
        </div>
      </div>
    </section>

    <section id="gallery" class="container" aria-label="Gallery">
      <div class="section-title">
        <h3>Gallery</h3>
        <span class="sub">Real clients. Real glow.</span>
      </div>
      <div class="gallery">
        <img src="images/gallery1.jpg" alt="Soft bridal bun with fresh flowers">
        <img src="images/gallery2.jpg" alt="Glowy natural makeup look">
        <img src="images/gallery3.jpg" alt="Neat gel manicure in blush pink">
        <img src="images/gallery4.jpg" alt="Before and after eyebrow shaping">
        <img src="images/gallery5.jpg" alt="Classic french pedicure close‑up">
        <img src="images/gallery6.jpg" alt="Spa facial treatment in progress">
      </div>
    </section>

    <section id="testimonials" class="container" aria-label="Testimonials">
      <div class="section-title">
        <h3>Client love</h3>
        <span class="sub">4.8/5 average rating</span>
      </div>
      <div class="grid grid-3">
        <div class="card testimonial">
          <div class="avatar" aria-hidden="true"></div>
          <div>
            <h4>Aarushi S.</h4>
            <p class="muted">“Booked my bridal package here — the calm I needed and the look I dreamed of.”</p>
          </div>
        </div>
        <div class="card testimonial">
          <div class="avatar" aria-hidden="true"></div>
          <div>
            <h4>Neha K.</h4>
            <p class="muted">“Facial results lasted weeks. Super hygienic and friendly staff.”</p>
          </div>
        </div>
        <div class="card testimonial">
          <div class="avatar" aria-hidden="true"></div>
          <div>
            <h4>Sakshi R.</h4>
            <p class="muted">“They nailed my haircut and finish. Booking was effortless.”</p>
          </div>
        </div>
      </div>
    </section>

    <section id="booking" class="container" aria-label="Booking">
      <div class="section-title">
        <h3>Book an appointment</h3>
        <span class="sub">We’ll confirm on call or WhatsApp</span>
      </div>
      <form id="bookForm" action="https://formspree.io/f/your-id" method="POST">
        <div class="two">
          <div>
            <label for="name">Full name</label>
            <input id="name" name="name" type="text" required placeholder="Your name" />
          </div>
          <div>
            <label for="phone">Phone (WhatsApp)</label>
            <input id="phone" name="phone" type="tel" required placeholder="+91 98XXXXXXXX" />
          </div>
        </div>
        <div class="two">
          <div>
            <label for="service">Service</label>
            <select id="service" name="service" required>
              <option value="">Select a service</option>
              <option>Haircut & Styling</option>
              <option>Bridal Makeup</option>
              <option>Facial Treatment</option>
              <option>Manicure & Pedicure</option>
              <option>Waxing & Threading</option>
              <option>Spa & Massage</option>
            </select>
          </div>
          <div>
            <label for="date">Preferred date</label>
            <input id="date" name="date" type="date" required />
          </div>
        </div>
        <div class="two">
          <div>
            <label for="time">Preferred time</label>
            <input id="time" name="time" type="time" required />
          </div>
          <div>
            <label for="notes">Notes (optional)</label>
            <input id="notes" name="notes" type="text" placeholder="Any special requests" />
          </div>
        </div>
        <button class="btn" type="submit">Request booking</button>
        <p class="muted">By submitting, you agree to be contacted via phone or WhatsApp for confirmation.</p>
      </form>
    </section>

    <section id="contact" class="container" aria-label="Contact">
      <div class="section-title">
        <h3>Contact & hours</h3>
        <span class="sub">Visit us or reach out</span>
      </div>
      <div class="contact-list">
        <div class="card">
          <h4>Call</h4>
          <p><a href="tel:+91XXXXXXXXXX">+91 XXXXX XXXXX</a></p>
          <p class="muted">Fastest for same‑day slots</p>
        </div>
        <div class="card">
          <h4>WhatsApp</h4>
          <p><a href="https://wa.me/91XXXXXXXXXX" target="_blank" rel="noopener">Chat now</a></p>
          <p class="muted">Share reference photos</p>
        </div>
        <div class="card">
          <h4>Address</h4>
          <p>Near Main Market, Gadarpur<br>Uttarakhand 263152</p>
          <p class="muted"><a href="https://maps.google.com/?q=Gadarpur%20Uttarakhand" target="_blank" rel="noopener">Open in Google Maps</a></p>
        </div>
        <div class="card">
          <h4>Hours</h4>
          <p>Mon–Sun: 10:00–19:30</p>
          <p class="muted">Closed on public holidays</p>
        </div>
      </div>
    </section>
  </main>

  <a class="floating-whatsapp" href="https://wa.me/91XXXXXXXXXX?text=Hi%20Radiant%20Glow" target="_blank" rel="noopener" aria-label="Chat on WhatsApp">WhatsApp</a>

  <footer>
    <div class="container">
      © <span id="year"></span> Radiant Glow Beauty Parlour • Gadarpur
    </div>
  </footer>

  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "BeautySalon",
    "name": "Radiant Glow Beauty Parlour",
    "image": "https://your-domain.com/images/og-image.jpg",
    "telephone": "+91 XXXXX XXXXX",
    "address": {
      "@type": "PostalAddress",
      "addressLocality": "Gadarpur",
      "addressRegion": "Uttarakhand",
      "postalCode": "263152",
      "addressCountry": "IN",
      "streetAddress": "Near Main Market"
    },
    "url": "https://your-domain.com/",
    "priceRange": "₹₹",
    "openingHours": "Mo-Su 10:00-19:30",
    "sameAs": [
      "https://www.instagram.com/yourhandle",
      "https://www.facebook.com/yourpage"
    ],
    "servesCuisine": [],
    "areaServed": "Gadarpur"
  }
  </script>

  <script>
    // set current year
    document.getElementById('year').textContent = new Date().getFullYear();
    // basic validation: ensure future date/time
    const form = document.getElementById('bookForm');
    form.addEventListener('submit', (e)=>{
      const date = document.getElementById('date').value;
      const time = document.getElementById('time').value;
      if(date){
        const selected = new Date(`${date}T${time || '00:00'}`);
        const now = new Date();
        if(selected < now){
          e.preventDefault();
          alert('Please choose a future date/time.');
        }
      }
    });
  </script>
</body>
</html>
