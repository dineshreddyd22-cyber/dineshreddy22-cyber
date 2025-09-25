
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Dinesh Reddy — AI Architect & Developer</title>
  <meta name="description" content="Portfolio of Dinesh Reddy — AI Architect & Developer" />

  <style>
    :root{
      --bg1:#0b0011;
      --bg2:#1b002d;
      --neon-cyan: #24f0ff;
      --neon-magenta: #b04bff;
      --muted: #9fc8d8;
      --glass: rgba(255,255,255,0.03);
      --glass-2: rgba(255,255,255,0.02);
      --white: #e8fbff;
      --card: rgba(255,255,255,0.03);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,'Helvetica Neue',Arial;color:var(--white);background:linear-gradient(180deg,var(--bg1),var(--bg2));-webkit-font-smoothing:antialiased;}
    a{color:inherit;text-decoration:none}
    /* container */
    .container{max-width:1200px;margin:28px auto;padding:26px;border-radius:14px;border:1px solid rgba(255,255,255,0.03);background:linear-gradient(180deg,rgba(255,255,255,0.01),rgba(255,255,255,0.00));position:relative;overflow:hidden;}
    /* nav */
    header{display:flex;align-items:center;gap:20px;padding-bottom:18px;border-bottom:1px solid var(--glass-2)}
    .logo{font-weight:800;letter-spacing:0.6px;font-size:18px;display:flex;align-items:center;gap:12px}
    .logo .dot{width:10px;height:10px;border-radius:50%;background:linear-gradient(90deg,var(--neon-cyan),var(--neon-magenta));box-shadow:0 0 14px rgba(36,240,255,0.18)}
    nav{margin-left:auto;display:flex;gap:12px;align-items:center}
    nav a{padding:8px 12px;border-radius:8px;color:var(--muted);font-size:13px;border:1px solid transparent}
    nav a:hover{color:var(--white);border:1px solid rgba(36,240,255,0.06);box-shadow:0 6px 20px rgba(36,240,255,0.03)}
    .cta{border:1px solid rgba(255,255,255,0.06);padding:8px 12px;border-radius:8px;font-size:13px}
    /* two-col hero */
    .hero{display:grid;grid-template-columns:360px 1fr;gap:28px;padding-top:20px;align-items:start}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.00));border-radius:12px;padding:18px;border:1px solid var(--card);box-shadow:0 8px 30px rgba(0,0,0,0.6)}
    .profile{
      text-align:center;position:relative;
    }
    .ring{width:220px;height:220px;margin:6px auto;border-radius:50%;padding:7px;border:3px solid rgba(36,240,255,0.18);box-shadow:0 0 48px rgba(36,240,255,0.06), inset 0 0 20px rgba(176,75,255,0.03);display:flex;align-items:center;justify-content:center;background:radial-gradient(circle at 20% 20%, rgba(36,240,255,0.03), transparent 30%)}
    .ring img{width:196px;height:196px;border-radius:50%;object-fit:cover;display:block}
    .hname{font-size:28px;font-weight:800;margin-top:10px;letter-spacing:0.8px}
    .hrole{font-size:13px;color:var(--muted);margin-top:6px}
    .contact-list{display:flex;flex-direction:column;gap:8px;margin-top:14px;align-items:center}
    .chip{padding:8px 12px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);color:var(--muted);font-size:13px;background:linear-gradient(180deg, rgba(255,255,255,0.005),transparent)}
    /* right column hero */
    .intro{display:flex;flex-direction:column;gap:12px;min-height:260px}
    .intro .title{display:flex;align-items:center;gap:12px}
    .intro h1{font-size:34px;margin:0;letter-spacing:0.6px}
    .intro p.lead{margin:0;color:var(--muted);max-width:860px;line-height:1.5}
    .socials{display:flex;gap:12px;margin-top:10px}
    .socials a{padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);font-size:13px;color:var(--muted)}
    /* sections */
    section{margin-top:22px}
    .section-title{display:flex;align-items:center;gap:12px;margin-bottom:12px}
    .section-title h2{margin:0;font-size:18px}
    .accent{height:3px;width:64px;border-radius:6px;background:linear-gradient(90deg,var(--neon-cyan),var(--neon-magenta));box-shadow:0 8px 30px rgba(176,75,255,0.06)}
    /* skills */
    .skills-grid{display:flex;gap:12px;flex-wrap:wrap}
    .skill{min-width:120px;padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.03);background:linear-gradient(180deg, rgba(255,255,255,0.01),transparent);text-align:center;transition:transform .25s ease}
    .skill:hover{transform:translateY(-6px);box-shadow:0 20px 40px rgba(2,6,12,0.6)}
    .skill .k{font-weight:700}
    .skill .v{font-size:12px;color:var(--muted);margin-top:6px}
    /* projects grid */
    .projects-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .project-card{position:relative;border-radius:10px;overflow:hidden;border:1px solid rgba(255,255,255,0.03);cursor:pointer;background:linear-gradient(180deg, rgba(255,255,255,0.01),transparent);transition:transform .22s ease}
    .project-card:hover{transform:translateY(-6px)}
    .project-thumb{width:200px;height:200px;object-fit:cover;display:block}
    .project-info{padding:12px}
    .project-info h3{margin:0;font-size:15px}
    .project-info p{margin:6px 0 0;color:var(--muted);font-size:13px}
    /* gallery */
    .gallery-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
    .gallery-grid img{width:200px;height:200px;object-fit:cover;border-radius:8px;cursor:pointer;transition:transform .18s ease}
    .gallery-grid img:hover{transform:scale(1.04)}
    /* contact */
    .contact-grid{display:flex;gap:12px;flex-wrap:wrap}
    .contact-card{flex:1;min-width:220px;padding:14px;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}
    .footer{margin-top:18px;font-size:13px;color:var(--muted);display:flex;justify-content:space-between;align-items:center}
    /* modal */
    .modal{position:fixed;inset:0;background:rgba(0,0,0,0.6);display:flex;align-items:center;justify-content:center;z-index:999;opacity:0;pointer-events:none;transition:opacity .18s ease}
    .modal.open{opacity:1;pointer-events:auto}
    .modal .box{max-width:900px;width:94%;background:linear-gradient(180deg, rgba(8,6,12,0.95), rgba(8,6,12,0.98));border-radius:12px;padding:12px;border:1px solid rgba(255,255,255,0.04)}
    .modal img{width:100%;height:auto;border-radius:8px;display:block}
    /* responsive */
    @media (max-width:1050px){.projects-grid{grid-template-columns:repeat(2,1fr)} .gallery-grid{grid-template-columns:repeat(3,1fr)} .hero{grid-template-columns:1fr}}
    @media (max-width:700px){.gallery-grid{grid-template-columns:repeat(2,1fr)} header{flex-direction:column;align-items:flex-start} nav{margin-left:0;gap:8px;overflow:auto;padding-top:8px}}
    @media (max-width:420px){.projects-grid{grid-template-columns:1fr} .gallery-grid{grid-template-columns:1fr}}
    /* small decorative particle glow top right */
    .glow-deco{position:absolute;right:-120px;top:-120px;width:360px;height:360px;border-radius:50%;background:radial-gradient(circle at 30% 30%, rgba(36,240,255,0.08), transparent 20%);filter:blur(26px);pointer-events:none;opacity:0.8}
  </style>
</head>
<body>

  <div class="container" id="page">
    <div class="glow-deco" aria-hidden="true"></div>

    <header>
      <div class="logo"><span class="dot" aria-hidden="true"></span> DINESH REDDY</div>
      <nav>
        <a href="#home" class="nav-link">Home</a>
        <a href="#about" class="nav-link">About</a>
        <a href="#skills" class="nav-link">Skills</a>
        <a href="#projects" class="nav-link">Projects</a>
        <a href="#gallery" class="nav-link">Gallery</a>
        <a href="#contact" class="nav-link">Contact</a>
        <a class="cta" href="mailto:dineshreddyd22@gmail.com">Email Me</a>
      </nav>
    </header>

    <!-- HERO / HOME -->
    <main id="home" class="hero">
      <aside class="card profile" aria-labelledby="profile-title">
        <div class="ring" aria-hidden="true">
          <img src="C:\Users\HP\Pictures\dinesh5.jpg" alt="Dinesh Reddy — Profile photo">
        </div>
        <div id="profile-title" class="hname">DINESH REDDY</div>
        <div class="hrole">AI Architect & Developer</div>

        <div class="contact-list" role="list">
          <div class="chip" role="listitem">📧 <a href="mailto:dineshreddyd22@gmail.com">dineshreddyd22@gmail.com</a></div>
          <div class="chip" role="listitem">📱 <a href="tel:+917337242989">+91 7337242989</a></div>
          <div class="chip" role="listitem">📍 IT Hub: Hyderabad — AI & Dev Community</div>
          <div class="chip" role="listitem">💼 Open to freelance & full-time</div>
        </div>
      </aside>

      <section class="card intro" aria-labelledby="intro-title">
        <div class="title">
          <h1 id="intro-title">Building scalable AI systems & delightful products</h1>
        </div>
        <p class="lead">
          I am an AI Architect & Software Developer specializing in production-grade ML systems,
          model deployment, and end-to-end solutions. I work with teams to design robust
          architectures, optimize inference pipelines, and build interfaces that help products
          deliver real value.
        </p>

        <div class="socials" aria-label="social links">
          <a href="#" title="LinkedIn">LinkedIn</a>
          <a href="#" title="GitHub">GitHub</a>
          <a href="#" title="Resume">Resume</a>
        </div>

        <div style="margin-top:auto">
          <div class="section-title"><h2>Quick Bio</h2><div class="accent"></div></div>
          <p style="color:var(--muted);line-height:1.5">
            Part of the growing AI & Software Development hub — focusing on research-driven product engineering,
            real-time inference, and human-centered AI systems. Experienced in Python, TensorFlow/PyTorch,
            cloud deployment (AWS/GCP), and frontend integrations.
          </p>
        </div>
      </section>
    </main>

    <!-- ABOUT -->
    <section id="about" class="card" aria-labelledby="about-title">
      <div class="section-title"><h2 id="about-title">About</h2><div class="accent"></div></div>
      <div style="display:flex;gap:18px;flex-wrap:wrap">
        <div style="flex:1;min-width:260px">
          <h3 style="margin-top:0">Who I am</h3>
          <p style="color:var(--muted);line-height:1.6">
            I design and build AI systems that scale. My work covers model research, data pipelines,
            deployment automation, and front-end integrations. I love converting prototypes into
            production services and mentoring teams to adopt best practices.
          </p>
        </div>
        <div style="flex:1;min-width:260px">
          <h3>IT Hub Information</h3>
          <p style="color:var(--muted);line-height:1.6">
            Located at Hyderabad's tech ecosystem — I collaborate with startups and research groups.
            If your team needs mentorship, architecture reviews, or help to ship model-backed features,
            contact me using the form below or email directly.
          </p>
          <div style="margin-top:10px;display:flex;gap:8px;flex-wrap:wrap">
            <div class="chip">Cloud: AWS / GCP</div>
            <div class="chip">Modeling: PyTorch, TF</div>
            <div class="chip">Frontend: React / JS</div>
            <div class="chip">DevOps: Docker, K8s</div>
          </div>
        </div>
      </div>
    </section>

    <!-- SKILLS -->
    <section id="skills" class="card" aria-labelledby="skills-title">
      <div class="section-title"><h2 id="skills-title">Skills</h2><div class="accent"></div></div>
      <div class="skills-grid" role="list">
        <div class="skill" role="listitem"><div class="k">AI Research</div><div class="v">Model prototyping & evaluation</div></div>
        <div class="skill" role="listitem"><div class="k">ML Engineering</div><div class="v">Pipelines, inference & scaling</div></div>
        <div class="skill" role="listitem"><div class="k">Python</div><div class="v">Scripting & architecture</div></div>
        <div class="skill" role="listitem"><div class="k">Frontend</div><div class="v">React, JS, D3</div></div>
        <div class="skill" role="listitem"><div class="k">DevOps</div><div class="v">Docker, Kubernetes</div></div>
        <div class="skill" role="listitem"><div class="k">Data</div><div class="v">ETL, Feature Stores</div></div>
      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects" class="card" aria-labelledby="projects-title">
      <div class="section-title"><h2 id="projects-title">Projects</h2><div class="accent"></div></div>
      <div class="projects-grid">
        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\3.jpg" alt="AI Driven Vehicle Design">
          <div class="project-info">
            <h3>AI Driven Vehicle Design</h3>
            <p>Generative design + CAD export pipeline.</p>
          </div>
        </article>

        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\2.jpg" alt="3D Mesh Research">
          <div class="project-info">
            <h3>3D Mesh Research</h3>
            <p>Point-cloud reconstruction & evaluation.</p>
          </div>
        </article>

        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\1.jpg" alt="Neural Face Models">
          <div class="project-info">
            <h3>Neural Face Models</h3>
            <p>Real-time expression transfer system.</p>
          </div>
        </article>

        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\4.jpg" alt="Interactive Visualizations">
          <div class="project-info">
            <h3>Interactive Visualizations</h3>
            <p>Dashboards & model explainability tools.</p>
          </div>
        </article>

        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\5.jpg" alt="Research Papers">
          <div class="project-info">
            <h3>Research Papers</h3>
            <p>Published & preprints on ML methods.</p>
          </div>
        </article>

        <article class="project-card" tabindex="0">
          <img class="project-thumb" src="C:\Users\HP\Pictures\6.jpg" alt="Generative Art">
          <div class="project-info">
            <h3>Generative Art</h3>
            <p>Creative experiments with generative models.</p>
          </div>
        </article>
      </div>
    </section>

    <!-- GALLERY -->
    <section id="gallery" class="card" aria-labelledby="gallery-title">
      <div class="section-title"><h2 id="gallery-title">Gallery</h2><div class="accent"></div></div>
      <div class="gallery-grid">
        <img src="C:\Users\HP\Pictures\dinesh1.jpg" alt="Gallery image 1" data-full="gallery1.jpg">
        <img src="C:\Users\HP\Pictures\dinesh2.jpg" alt="Gallery image 2" data-full="gallery2.jpg">
        <img src="C:\Users\HP\Pictures\dinesh4.jpg" alt="Gallery image 3" data-full="gallery3.jpg">
        <img src= "C:\Users\HP\Pictures\dinesh6.jpg"alt="Gallery image 4" data-full="gallery4.jpg">
        <img src="C:\Users\HP\Pictures\dinesh9.jpg" alt="Gallery image 5" data-full="gallery5.jpg">
        <img src= "C:\Users\HP\Pictures\dinesh8.jpg"alt="Gallery image 6" data-full="gallery6.jpg">
        <img src="C:\Users\HP\Pictures\dinesh10.jpg" alt="Gallery image 7" data-full="gallery7.jpg">
        <img src="C:\Users\HP\Pictures\dinesh3.jpg"alt="Gallery image 8" data-full="gallery8.jpg">
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="card" aria-labelledby="contact-title">
      <div class="section-title"><h2 id="contact-title">Contact</h2><div class="accent"></div></div>

      <div style="display:flex;gap:14px;flex-wrap:wrap">
        <div class="contact-card">
          <h3>Reach out</h3>
          <p style="color:var(--muted)">Email or call me for opportunities, collaborations, or consulting.</p>
          <p style="margin-top:12px"><strong>Email:</strong> <a href="mailto:dineshreddyd22@gmail.com">dineshreddyd22@gmail.com</a></p>
          <p><strong>Phone:</strong> <a href="tel:+917337242989">+91 7337242989</a></p>
          <div style="margin-top:14px">
            <a class="chip" href="#" aria-label="LinkedIn">LinkedIn</a>
            <a class="chip" href="#" aria-label="GitHub">GitHub</a>
          </div>
        </div>

        <div class="contact-card">
          <h3>Send a message</h3>
          <form id="contactForm" onsubmit="return false" style="display:flex;flex-direction:column;gap:8px">
            <input type="text" id="name" placeholder="Your name" required style="padding:10px;border-radius:8px;border:1px solid var(--glass-2);background:transparent;color:var(--white)">
            <input type="email" id="email" placeholder="Your email" required style="padding:10px;border-radius:8px;border:1px solid var(--glass-2);background:transparent;color:var(--white)">
            <textarea id="message" rows="4" placeholder="Message" style="padding:10px;border-radius:8px;border:1px solid var(--glass-2);background:transparent;color:var(--white)"></textarea>
            <div style="display:flex;gap:8px">
              <button id="sendBtn" style="padding:10px 14px;border-radius:8px;border:1px solid rgba(255,255,255,0.05);background:linear-gradient(90deg,var(--neon-cyan),var(--neon-magenta));color:#05101a;cursor:pointer">Send</button>
              <button type="reset" style="padding:10px 14px;border-radius:8px;border:1px solid rgba(255,255,255,0.05);background:transparent;color:var(--white);cursor:pointer">Reset</button>
            </div>
          </form>
          <p id="formMsg" style="color:var(--muted);font-size:13px;margin-top:8px"></p>
        </div>
      </div>
    </section>

    <div class="footer">
      <div>© Dinesh Reddy — AI Architect & Developer</div>
      <div style="color:var(--muted)">Built with HTML • CSS • JavaScript</div>
    </div>
  </div>

  <!-- gallery modal -->
  <div id="modal" class="modal" role="dialog" aria-hidden="true">
    <div class="box">
      <button id="modalClose" style="float:right;background:none;border:none;color:var(--muted);font-size:18px;cursor:pointer">✕</button>
      <img id="modalImg" src="" alt="Expanded gallery image">
    </div>
  </div>

  <!-- lightweight JS for interactions -->
  <script>
    // Smooth scroll for nav links
    document.querySelectorAll('.nav-link').forEach(link=>{
      link.addEventListener('click', (e)=>{
        e.preventDefault();
        const id = link.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el){
          window.scrollTo({top: el.getBoundingClientRect().top + window.scrollY - 20, behavior:'smooth'});
        }
      });
    });

    // Contact form "send" (demo) — doesn't actually send email; you can integrate with email service or backend
    const contactForm = document.getElementById('contactForm');
    const sendBtn = document.getElementById('sendBtn');
    const formMsg = document.getElementById('formMsg');
    sendBtn.addEventListener('click', ()=>{
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const msg = document.getElementById('message').value.trim();
      if(!name || !email || !msg){ formMsg.textContent = 'Please fill all fields.'; return; }
      formMsg.textContent = 'Thanks — message noted locally (demo). To enable email sending integrate an API or mailto handler.';
      // demo: build mailto link (opens user's mail client)
      const mailto = mailto:dineshreddyd22@gmail.com?subject=${encodeURIComponent('Portfolio message from ' + name)}&body=${encodeURIComponent(msg + '\\n\\nFrom: ' + name + ' — ' + email)};
      window.location.href = mailto;
    });

    // Gallery modal
    const modal = document.getElementById('modal');
    const modalImg = document.getElementById('modalImg');
    const modalClose = document.getElementById('modalClose');
    document.querySelectorAll('.gallery-grid img').forEach(img=>{
      img.addEventListener('click', ()=>{
        const src = img.dataset.full || img.src;
        modalImg.src = src;
        modal.classList.add('open');
        modal.setAttribute('aria-hi 
  
