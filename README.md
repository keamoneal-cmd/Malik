<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>M&J Embroidery — Premium Embroidery Services in Kampala</title>
  <meta name="description" content="M&J Embroidery — custom embroidery for corporate, schools, sports teams and special events. Located on Nasser Road, Kampala.">

  <!-- Fonts & Icons -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Playfair+Display:wght@600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    /* --------------------
       Branding variables
       -------------------- */
    :root{
      --gold: #D4AF37;
      --black: #0b0b0b;
      --white: #ffffff;
      --grey: #888888;
      --light-grey: #F6F6F7;
      --text: #2b2b2b;
      --max-width: 1200px;
      --header-height: 78px;
    }

    /* Reset + base */
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: 'Poppins', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
      background:var(--light-grey);
      color:var(--text);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
    }

    a{color:inherit}
    img{max-width:100%;display:block}

    /* Skip link */
    .skip-link{
      position:absolute;left:8px;top:8px;padding:8px 12px;background:#000;color:#fff;border-radius:6px;z-index:2000;
      transform:translateY(-120%);transition:transform .2s ease;outline:0
    }
    .skip-link:focus{transform:none}

    /* Header */
    header{
      position:fixed;inset:0 0 auto 0;height:var(--header-height);background:linear-gradient(90deg,var(--black), #111);color:var(--white);
      display:flex;align-items:center;z-index:1200;width:100%;box-shadow:0 6px 18px rgba(0,0,0,.18);
    }
    .header-inner{width:100%;max-width:var(--max-width);margin:0 auto;padding:0 5%;display:flex;align-items:center;justify-content:space-between}

    .brand{display:flex;align-items:center;gap:14px}
    .brand img{height:52px;width:52px;border-radius:8px;object-fit:cover}
    .brand h1{font-family:'Playfair Display';font-size:1.05rem;margin:0;background:linear-gradient(90deg,var(--gold),#F5D062);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
    .brand p{margin:0;font-size:.78rem;color:var(--grey)}

    nav{display:flex;align-items:center;gap:20px}
    .nav-list{display:flex;gap:20px;list-style:none;margin:0;padding:0}
    .nav-list a{color:var(--white);text-decoration:none;padding:8px 10px;border-radius:8px;font-weight:600;font-size:.95rem}
    .nav-list a:hover, .nav-list a:focus{background:rgba(212,175,55,.08);color:var(--gold);outline:none}

    .mobile-toggle{display:none;background:none;border:0;color:var(--white);font-size:1.25rem;padding:8px;border-radius:8px}

    /* Hero */
    .hero{
      min-height:calc(100vh - var(--header-height));
      display:flex;align-items:center;padding-top:var(--header-height);background-image:url('https://images.unsplash.com/photo-1618354691373-d851c5c3a990?auto=format&fit=crop&w=1900&q=80');background-size:cover;background-position:center;position:relative
    }
    .hero::after{content:'';position:absolute;inset:0;background:linear-gradient(180deg,rgba(0,0,0,.55),rgba(0,0,0,.25))}
    .hero-inner{position:relative;z-index:2;width:100%;max-width:var(--max-width);margin:0 auto;padding:6% 5%;display:flex;gap:40px;align-items:center}

    .hero-text{flex:1;color:var(--white)}
    .eyebrow{display:inline-block;padding:6px 12px;background:rgba(255,255,255,.06);border-radius:999px;font-weight:600;margin-bottom:14px}
    .hero-text h2{font-size:2.6rem;line-height:1.05;margin:0 0 12px;font-family:'Playfair Display'}
    .hero-text p{max-width:680px;margin:0 0 20px;color:rgba(255,255,255,.9)}
    .cta-row{display:flex;gap:12px;flex-wrap:wrap}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 20px;border-radius:999px;border:2px solid transparent;font-weight:700;cursor:pointer;text-decoration:none}
    .btn-primary{background:var(--gold);color:var(--black);border-color:var(--gold)}
    .btn-outline{background:transparent;color:var(--white);border-color:rgba(255,255,255,.12)}

    /* Card spotlight on right */
    .hero-card{flex:0 0 360px;background:var(--white);border-radius:12px;box-shadow:0 12px 40px rgba(11,11,11,.25);padding:18px}
    .hero-card h4{margin:0 0 8px;font-size:1.05rem}
    .hero-card p{margin:0 0 12px;color:var(--grey)}
    .price-row{display:flex;justify-content:space-between;align-items:center}
    .price{font-weight:800;color:var(--gold);font-size:1.05rem}

    /* Sections */
    section{padding:72px 5%}
    .container{max-width:var(--max-width);margin:0 auto}
    .section-title{font-size:1.95rem;margin-bottom:12px;display:inline-block}
    .section-sub{color:var(--grey);margin-bottom:28px}

    /* About */
    .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:28px;align-items:center}
    .about-grid img{border-radius:12px;box-shadow:0 12px 30px rgba(11,11,11,.06)}
    .stats{display:flex;gap:20px;flex-wrap:wrap;margin-top:18px}
    .stat{background:linear-gradient(180deg,rgba(212,175,55,.06),transparent);padding:12px;border-radius:10px;min-width:120px}

    /* Services */
    .services-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:20px}
    .card{background:var(--white);border-radius:12px;overflow:hidden;box-shadow:0 6px 24px rgba(11,11,11,.06);transition:transform .3s ease,box-shadow .3s ease}
    .card:hover{transform:translateY(-10px);box-shadow:0 28px 60px rgba(11,11,11,.12)}
    .card .media{height:180px;background-size:cover;background-position:center}
    .card .body{padding:18px}
    .price-tag{font-weight:800;color:var(--gold)}

    /* Portfolio */
    .portfolio-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .portfolio-item{position:relative;border-radius:10px;overflow:hidden;height:220px}
    .portfolio-overlay{position:absolute;inset:0;background:linear-gradient(180deg,transparent,rgba(0,0,0,.6));display:flex;align-items:flex-end;padding:14px;color:#fff}

    /* Testimonials */
    .testi-wrap{display:grid;grid-template-columns:1fr 320px;gap:24px;align-items:start}
    .testi{background:linear-gradient(180deg,var(--white),#fff);padding:20px;border-radius:12px;box-shadow:0 8px 30px rgba(11,11,11,.06)}
    .testimonial-avatar{width:68px;height:68px;border-radius:50%;object-fit:cover;border:3px solid var(--gold)}

    /* Contact */
    .contact-grid{display:grid;grid-template-columns:1fr 420px;gap:28px}
    .contact-card{background:var(--white);padding:20px;border-radius:12px;box-shadow:0 8px 30px rgba(11,11,11,.06)}
    .form-group{margin-bottom:14px}
    label{display:block;font-weight:600;margin-bottom:6px}
    input,textarea,select{width:100%;padding:10px;border-radius:8px;border:1px solid #e6e6e6;font-size:1rem}
    textarea{min-height:120px}
    .form-success{display:none;padding:12px;border-radius:8px;background:rgba(212,175,55,.08);color:var(--text);font-weight:600}

    /* Footer */
    footer{background:var(--black);color:var(--white);padding:56px 5%}
    .footer-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:20px}
    .footer a{color:var(--grey);text-decoration:none}

    /* Responsive */
    @media (max-width:1000px){.hero-inner{flex-direction:column;align-items:flex-start}.about-grid{grid-template-columns:1fr}.testi-wrap{grid-template-columns:1fr}.contact-grid{grid-template-columns:1fr}}
    @media (max-width:700px){.nav-list{display:none}.mobile-toggle{display:inline-flex}.hero-text h2{font-size:1.6rem}}

    /* small utilities */
    .muted{color:var(--grey)}

    /* anchor offset fix */
    [id]{scroll-margin-top:calc(var(--header-height) + 18px)}
  </style>
</head>
<body>
  <a class="skip-link" href="#main">Skip to content</a>

  <header>
    <div class="header-inner">
      <div class="brand">
        <img src="https://via.placeholder.com/120x120.png?text=M%26J" alt="M&amp;J Embroidery logo">
        <div>
          <h1>M&amp;J Embroidery</h1>
          <p class="muted">Nasser Road — Opp. SAL Building, Kampala</p>
        </div>
      </div>

      <nav aria-label="Primary navigation">
        <ul class="nav-list" id="navList">
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#portfolio">Portfolio</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>

        <button class="mobile-toggle" id="menuToggle" aria-expanded="false" aria-controls="navList">
          <i class="fas fa-bars" aria-hidden="true"></i>
          <span class="sr-only">Menu</span>
        </button>
      </nav>
    </div>
  </header>

  <!-- HERO -->
  <main id="main">
    <section class="hero" id="home" aria-label="Intro">
      <div class="hero-inner container">
        <div class="hero-text">
          <span class="eyebrow">Premium • Local • Trusted</span>
          <h2>Elevate your brand with <span style="color:var(--gold)">handcrafted embroidery</span></h2>
          <p>We turn logos and ideas into lasting stitches — corporate uniforms, school badges, sports kits, wedding favours and bespoke gifts. Fast turnaround, quality threading, unbeatable local knowledge.</p>

          <div class="cta-row">
            <a class="btn btn-primary" href="#contact"><i class="fas fa-envelope"></i> Get a Free Quote</a>
            <a class="btn btn-outline" href="#portfolio">See Our Work</a>
          </div>
        </div>

        <aside class="hero-card" aria-hidden="false">
          <h4>Quick starting prices</h4>
          <p class="muted">Indicative — final price depends on design & qty.</p>
          <div class="price-row" style="margin-top:10px;">
            <div class="muted">School badge</div>
            <div class="price">From UGX 30,000</div>
          </div>
          <div class="price-row" style="margin-top:8px;">
            <div class="muted">Corporate polo (logo)</div>
            <div class="price">From UGX 50,000</div>
          </div>
          <div style="margin-top:12px;display:flex;gap:8px">
            <a class="btn btn-primary" href="#contact">Request a quote</a>
            <a class="btn btn-outline" href="tel:+256712345678"><i class="fas fa-phone"></i> +256 712 345 678</a>
          </div>
        </aside>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about">
      <div class="container">
        <h2 class="section-title">About M&amp;J</h2>
        <p class="section-sub">Founded by <strong>Musinga Martin</strong> and managed by <strong>Jazirah</strong> — two machines, many orders, one obsession: excellent stitchwork.</p>

        <div class="about-grid">
          <div>
            <img src="https://images.unsplash.com/photo-1539109136888-8c8a5a0b87b8?auto=format&fit=crop&w=1400&q=60" alt="Embroidery close-up" loading="lazy">
          </div>
          <div>
            <p>From small bespoke gifts to bulk corporate runs, our team brings precision and care to every project. We use industry-grade machines, quality threads and multiple quality checks so your logo looks crisp on first wear and after many washes.</p>
            <div class="stats">
              <div class="stat"><strong>5+</strong><div class="muted">Years experience</div></div>
              <div class="stat"><strong>500+</strong><div class="muted">Happy clients</div></div>
              <div class="stat"><strong>10,000+</strong><div class="muted">Pieces embroidered</div></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" style="background:transparent">
      <div class="container">
        <h2 class="section-title">Services</h2>
        <p class="section-sub">What we do — clear, professional and tailored to your needs.</p>

        <div class="services-grid">
          <article class="card" aria-labelledby="s1">
            <div class="media" style="background-image:url('https://images.unsplash.com/photo-1556909114-44e5b18b68e6?auto=format&fit=crop&w=1200&q=60')" role="img" aria-label="corporate branding"></div>
            <div class="body">
              <h3 id="s1">Corporate Branding</h3>
              <p class="muted">Logo embroidery for polos, jackets, caps and corporate merch. Vector digitizing included for clean results.</p>
              <div class="price-tag">From UGX 50,000</div>
            </div>
          </article>

          <article class="card" aria-labelledby="s2">
            <div class="media" style="background-image:url('https://images.unsplash.com/photo-1598033129183-c4f50c736f10?auto=format&fit=crop&w=1200&q=60')" role="img" aria-label="school uniforms"></div>
            <div class="body">
              <h3 id="s2">School Uniforms</h3>
              <p class="muted">Badges, crests and names — consistent sizing and durable stitching built to last through wash cycles.</p>
              <div class="price-tag">From UGX 30,000</div>
            </div>
          </article>

          <article class="card" aria-labelledby="s3">
            <div class="media" style="background-image:url('https://images.unsplash.com/photo-1547347298-4074fc3086f0?auto=format&fit=crop&w=1200&q=60')" role="img" aria-label="sports kits"></div>
            <div class="body">
              <h3 id="s3">Sports Teams</h3>
              <p class="muted">Name & number embroidery, custom fonts and specialist threads for performance wear.</p>
              <div class="price-tag">From UGX 60,000</div>
            </div>
          </article>

          <article class="card" aria-labelledby="s4">
            <div class="media" style="background-image:url('https://images.unsplash.com/photo-1516762689617-e1cffcef479d?auto=format&fit=crop&w=1200&q=60')" role="img" aria-label="special events"></div>
            <div class="body">
              <h3 id="s4">Special Events & Gifts</h3>
              <p class="muted">Wedding favours, personalised gifts and limited-edition runs with careful finishing touches.</p>
              <div class="price-tag">Custom pricing</div>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- PORTFOLIO -->
    <section id="portfolio">
      <div class="container">
        <h2 class="section-title">Portfolio</h2>
        <p class="section-sub">A small selection of recent work for local clients.</p>

        <div class="portfolio-grid" id="portfolioGrid">
          <!-- each item has data-category to allow simple filtering if needed -->
          <div class="portfolio-item" data-category="corporate">
            <img src="https://images.unsplash.com/photo-1529374255404-311a2a4f1fd9?auto=format&fit=crop&w=1200&q=60" alt="Corporate polo shirts" loading="lazy">
            <div class="portfolio-overlay">
              <div>
                <strong>Corporate Polo Shirts</strong>
                <div class="muted">Kampala Business Solutions</div>
              </div>
            </div>
          </div>

          <div class="portfolio-item" data-category="school">
            <img src="https://images.unsplash.com/photo-1627552245715-77d79bbf6fe2?auto=format&fit=crop&w=1200&q=60" alt="School badges" loading="lazy">
            <div class="portfolio-overlay">
              <div>
                <strong>School Uniforms</strong>
                <div class="muted">Greenhill Academy</div>
              </div>
            </div>
          </div>

          <div class="portfolio-item" data-category="sports">
            <img src="https://images.unsplash.com/photo-1547347298-4074fc3086f0?auto=format&fit=crop&w=1200&q=60" alt="Sports jerseys" loading="lazy">
            <div class="portfolio-overlay">
              <div>
                <strong>Basketball Jerseys</strong>
                <div class="muted">Kampala City Titans</div>
              </div>
            </div>
          </div>

          <div class="portfolio-item" data-category="special">
            <img src="https://images.unsplash.com/photo-1516762689617-e1cffcef479d?auto=format&fit=crop&w=1200&q=60" alt="Wedding favours" loading="lazy">
            <div class="portfolio-overlay">
              <div>
                <strong>Wedding Favours</strong>
                <div class="muted">Personalised handkerchiefs</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- TESTIMONIALS -->
    <section aria-label="Testimonials">
      <div class="container">
        <h2 class="section-title">What clients say</h2>
        <div class="testi-wrap">
          <div>
            <div class="testi">
              <img class="testimonial-avatar" src="https://randomuser.me/api/portraits/women/43.jpg" alt="Sarah Kintu">
              <p style="margin:12px 0;font-style:italic">"M&J transformed our company uniforms. Attention to detail is unmatched in Kampala."</p>
              <strong>Sarah Kintu</strong>
              <div class="muted">HR Manager — Kampala Business Solutions</div>
            </div>

            <div style="height:14px"></div>

            <div class="testi">
              <img class="testimonial-avatar" src="https://randomuser.me/api/portraits/men/32.jpg" alt="Robert Mugisha">
              <p style="margin:12px 0;font-style:italic">"Reliable service for school uniforms — the embroidery holds up after many washes."</p>
              <strong>Robert Mugisha</strong>
              <div class="muted">Principal — Greenhill Academy</div>
            </div>
          </div>

          <aside>
            <div class="contact-card">
              <h3>Contact</h3>
              <p class="muted">Nasser Road, Opp. SAL Building, Kampala</p>
              <p><strong>Phone</strong><br>+256 712 345 678</p>
              <p><strong>Email</strong><br><a href="mailto:info@mjembroidery.ug">info@mjembroidery.ug</a></p>
              <div style="margin-top:8px">
                <a class="btn btn-primary" href="#contact">Request a quote</a>
              </div>
            </div>
          </aside>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <div class="container">
        <h2 class="section-title">Get in touch</h2>
        <p class="section-sub">Tell us about your project — we respond quickly.</p>

        <div class="contact-grid">
          <div>
            <div class="contact-card">
              <h3>Visit or call</h3>
              <p class="muted">Nasser Road, Opp. SAL Building, Kampala</p>

              <p><i class="fas fa-phone"></i> <a href="tel:+256712345678">+256 712 345 678</a></p>
              <p><i class="fas fa-envelope"></i> <a href="mailto:info@mjembroidery.ug">info@mjembroidery.ug</a></p>

              <h4 style="margin-top:14px">Follow us</h4>
              <div style="display:flex;gap:8px;margin-top:8px">
                <a class="btn btn-outline" href="#"><i class="fab fa-facebook-f"></i></a>
                <a class="btn btn-outline" href="#"><i class="fab fa-instagram"></i></a>
                <a class="btn btn-outline" href="#"><i class="fab fa-whatsapp"></i></a>
              </div>
            </div>
          </div>

          <form id="contactForm" class="contact-card" aria-label="Contact form">
            <div class="form-success" id="formSuccess">Thanks — your message has been received. We usually reply within 24 hours.</div>

            <div class="form-group">
              <label for="name">Your name</label>
              <input id="name" name="name" required>
            </div>

            <div class="form-group">
              <label for="email">Email</label>
              <input id="email" name="email" type="email" required>
            </div>

            <div class="form-group">
              <label for="phone">Phone</label>
              <input id="phone" name="phone" type="tel">
            </div>

            <div class="form-group">
              <label for="service">Service</label>
              <select id="service" name="service">
                <option>Corporate Branding</option>
                <option>School Uniforms</option>
                <option>Sports Teams</option>
                <option>Special Events</option>
                <option>Other</option>
              </select>
            </div>

            <div class="form-group">
              <label for="message">Message</label>
              <textarea id="message" name="message" required></textarea>
            </div>

            <button type="submit" class="btn btn-primary" style="width:100%">Send Message</button>
          </form>
        </div>
      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer>
    <div class="container footer-grid">
      <div>
        <h3>M&amp;J Embroidery</h3>
        <p class="muted">Premium embroidery services in Kampala. Crafted with care since 2018.</p>
      </div>
      <div>
        <h4>Quick links</h4>
        <ul style="list-style:none;padding:0;margin:0">
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#services">Services</a></li>
        </ul>
      </div>
      <div>
        <h4>Contact</h4>
        <p class="muted"><i class="fas fa-map-marker-alt"></i> Nasser Road, Opp. SAL Building, Kampala</p>
        <p class="muted"><i class="fas fa-phone"></i> +256 712 345 678</p>
      </div>
    </div>

    <div style="text-align:center;margin-top:28px;color:var(--grey);font-size:.95rem">&copy; 2025 M&amp;J Embroidery — Designed with <i class="fas fa-heart" style="color:var(--gold)"></i> by Musinga Martin</div>
  </footer>

  <script>
    // Accessible mobile nav toggle
    const menuToggle = document.getElementById('menuToggle');
    const navList = document.getElementById('navList');

    menuToggle.addEventListener('click', () => {
      const expanded = menuToggle.getAttribute('aria-expanded') === 'true';
      menuToggle.setAttribute('aria-expanded', String(!expanded));
      navList.style.display = expanded ? '' : 'flex';
    });

    // Smooth scroll with offset for fixed header
    document.querySelectorAll('a[href^="#"]').forEach(link => {
      link.addEventListener('click', function(e){
        const targetId = this.getAttribute('href');
        if (!targetId || targetId === '#') return;
        const targetEl = document.querySelector(targetId);
        if (!targetEl) return;
        e.preventDefault();

        const headerOffset = parseInt(getComputedStyle(document.documentElement).getPropertyValue('--header-height')) || 78;
        const elementPosition = targetEl.getBoundingClientRect().top + window.pageYOffset;
        const offsetPosition = elementPosition - headerOffset - 12;

        window.scrollTo({top: offsetPosition, behavior: 'smooth'});

        // close mobile menu on selection
        if (window.innerWidth < 700 && navList){
          navList.style.display = '';
          menuToggle.setAttribute('aria-expanded','false');
        }
      })
    });

    // Simple contact form handling (demo)
    const contactForm = document.getElementById('contactForm');
    const formSuccess = document.getElementById('formSuccess');
    contactForm.addEventListener('submit', (e) => {
      e.preventDefault();
      // Here: send data via fetch to your backend or integration (e.g. Formspree/SendGrid)
      formSuccess.style.display = 'block';
      contactForm.reset();
      setTimeout(()=>{formSuccess.style.display = 'none'},5000);
    });

    // Small graceful fallback: ensure nav shows on wider screens
    function handleResize(){ if (window.innerWidth >= 700){ navList.style.display = ''; menuToggle.setAttribute('aria-expanded','false'); } }
    window.addEventListener('resize', handleResize);
  </script>
</body>
</html>

