o# nexora-labs

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#0B1220">
<meta name="description" content="Nexora Labs builds modern websites, mobile apps and digital experiences for growing businesses.">
<title>Nexora Labs | Innovate. Build. Elevate.</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>
:root {
  --navy: #0B1220;
  --blue: #316BFF;
  --white: #F5F6FA;
  --muted: #858FA5;
}
* { margin:0; padding:0; box-sizing:border-box; }
html { scroll-behavior:smooth; }
body {
  font-family: Inter, sans-serif;
  background:var(--navy);
  color:white;
  overflow-x:hidden;
}
a { text-decoration:none; color:inherit; }
button { font:inherit; }
.container { width:min(1120px,90%); margin:auto; }
nav {
  height:78px; display:flex; align-items:center;
  justify-content:space-between;
  border-bottom:1px solid #ffffff14;
  position:sticky; top:0; z-index:10;
  background:#0B1220ed; backdrop-filter:blur(14px);
  padding:0 5%;
}
.logo { font-size:22px; font-weight:900; letter-spacing:-1px; }
.logo span { color:var(--blue); }
.navlinks { display:flex; gap:30px; align-items:center; }
.navlinks a { color:#c5cada; font-size:13px; }
.navlinks a:hover { color:white; }
.btn {
  display:inline-block; padding:14px 22px;
  background:var(--blue); border-radius:8px;
  color:white; font-size:14px; font-weight:700;
  border:1px solid var(--blue);
  transition:.25s;
}
.btn:hover { transform:translateY(-3px); background:#2057ec; }
.btn-outline { background:transparent; border-color:#ffffff35; }
.menu { display:none; background:none; border:0; color:white; font-size:25px; }
.hero {
  min-height:650px; display:flex; align-items:center;
  position:relative; overflow:hidden;
  background:radial-gradient(ellipse at 75% 45%,#316bff25,transparent 48%);
}
.hero-content { max-width:760px; padding:100px 0; position:relative; z-index:1; }
.eyebrow {
  color:#83a6ff; font-size:12px; letter-spacing:3px;
  font-weight:700; margin-bottom:25px;
}
.hero h1 {
  font-size:clamp(42px,7vw,78px);
  line-height:1.08; letter-spacing:-4px;
  font-weight:900; margin-bottom:25px;
}
.hero h1 span {
  background:linear-gradient(90deg,#316BFF,#8aaaff);
  -webkit-background-clip:text; color:transparent;
}
.hero p {
  max-width:580px; color:var(--muted);
  line-height:1.9; font-size:16px; margin-bottom:32px;
}
.actions { display:flex; gap:14px; flex-wrap:wrap; }
.hero-glow {
  position:absolute; width:350px; height:350px;
  right:5%; top:25%; border-radius:50%;
  background:#316bff20; filter:blur(90px);
}
.section { padding:95px 0; }
.section-label {
  color:#6790ff; font-size:12px;
  letter-spacing:3px; font-weight:800; margin-bottom:15px;
}
.section-title {
  font-size:clamp(30px,5vw,48px);
  letter-spacing:-2px; margin-bottom:18px;
}
.section-desc {
  color:var(--muted); line-height:1.8;
  max-width:650px; margin-bottom:45px;
}
.stats {
  display:grid; grid-template-columns:repeat(3,1fr);
  border-top:1px solid #ffffff1c;
  border-bottom:1px solid #ffffff1c;
}
.stat { padding:30px 20px; text-align:center; }
.stat h3 { color:#7fa0ff; font-size:30px; }
.stat p { color:var(--muted); font-size:13px; margin-top:8px; }
.services {
  display:grid; grid-template-columns:repeat(3,1fr); gap:20px;
}
.card {
  background:#111c30; border:1px solid #ffffff12;
  padding:30px; border-radius:14px;
  transition:.3s;
}
.card:hover {
  transform:translateY(-7px);
  border-color:#316BFF80;
}
.card .number { color:#6991ff; font-size:13px; font-weight:800; }
.card h3 { font-size:20px; margin:23px 0 13px; }
.card p { color:var(--muted); font-size:14px; line-height:1.8; }
.about {
  background:#101a2d;
  border-top:1px solid #ffffff10;
  border-bottom:1px solid #ffffff10;
}
.about-grid {
  display:grid; grid-template-columns:1fr 1fr;
  gap:55px; align-items:center;
}
.about-box {
  min-height:300px; border-radius:18px;
  background:linear-gradient(140deg,#316BFF,#13264c);
  display:flex; align-items:center; justify-content:center;
  text-align:center; padding:30px;
}
.about-box h2 { font-size:42px; font-weight:900; }
.about-box span { display:block; font-size:13px; letter-spacing:4px; margin-top:12px; }
.check { color:#82a4ff; margin:14px 0; font-size:14px; }
.projects {
  display:grid; grid-template-columns:repeat(2,1fr); gap:20px;
}
.project {
  background:#111c30; border:1px solid #ffffff15;
  border-radius:14px; overflow:hidden;
}
.project-art {
  height:190px; display:flex; align-items:center;
  justify-content:center; font-size:32px; font-weight:900;
  background:radial-gradient(circle,#316bff60,#111c30 70%);
}
.project-info { padding:24px; }
.project-info p { color:var(--muted); margin-top:9px; font-size:14px; }
.cta {
  text-align:center; padding:75px 25px;
  border:1px solid #316BFF60; border-radius:20px;
  background:radial-gradient(ellipse at top,#316bff24,transparent 70%),#111c30;
}
.cta h2 { font-size:clamp(30px,5vw,46px); margin-bottom:15px; }
.cta p { color:var(--muted); margin-bottom:27px; line-height:1.8; }
.contact-grid {
  display:grid; grid-template-columns:1fr 1fr; gap:35px;
}
.contact-card { padding:26px; background:#111c30; border-radius:14px; }
.contact-card p { color:var(--muted); margin-top:12px; line-height:1.8; }
form { display:grid; gap:14px; }
input, textarea {
  width:100%; padding:15px; background:#111c30;
  color:white; border:1px solid #ffffff20;
  border-radius:8px; font:inherit; outline:none;
}
input:focus,textarea:focus { border-color:var(--blue); }
textarea { min-height:130px; resize:vertical; }
footer {
  border-top:1px solid #ffffff15;
  padding:30px 5%; color:var(--muted);
  font-size:13px; text-align:center;
}
.whatsapp {
  position:fixed; right:22px; bottom:22px; z-index:20;
  background:#20c66b; color:white; border-radius:50px;
  padding:15px 19px; font-size:14px; font-weight:800;
  box-shadow:0 5px 25px #0006;
}
@media(max-width:750px) {
  .navlinks {
    display:none; position:absolute; top:78px;
    left:0; width:100%; padding:25px;
    background:#0B1220; flex-direction:column;
  }
  .navlinks.open { display:flex; }
  .menu { display:block; }
  nav>.btn { display:none; }
  .hero { min-height:570px; }
  .hero h1 { letter-spacing:-2px; }
  .services { grid-template-columns:1fr; }
  .about-grid,.contact-grid { grid-template-columns:1fr; }
  .projects { grid-template-columns:1fr; }
  .stats { grid-template-columns:1fr; }
  .stat { border-bottom:1px solid #ffffff15; }
  .section { padding:70px 0; }
}
</style>
</head>

<body>
<nav>
  <a class="logo" href="#home">NEXORA<span> LABS.</span></a>
  <div class="navlinks" id="navlinks">
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </div>
  <a class="btn" href="#contact">Let's Talk ↗</a>
  <button class="menu" onclick="toggleMenu()" aria-label="Open menu">☰</button>
</nav>

<main>
<section class="hero" id="home">
  <div class="hero-glow"></div>
  <div class="container">
    <div class="hero-content">
      <div class="eyebrow">✦ DIGITAL INNOVATION STUDIO</div>
      <h1>We Build Digital<br><span>Experiences.</span></h1>
      <p>
        We transform ambitious ideas into powerful websites,
        mobile applications and digital experiences that help
        businesses grow and stand out.
      </p>
      <div class="actions">
        <a class="btn" href="#contact">Start Your Project ↗</a>
        <a class="btn btn-outline" href="#services">Explore Services</a>
      </div>
    </div>
  </div>
</section>

<section class="container section">
  <div class="stats">
    <div class="stat"><h3>01</h3><p>Creative Thinking</p></div>
    <div class="stat"><h3>02</h3><p>Modern Technology</p></div>
    <div class="stat"><h3>03</h3><p>Future Focused</p></div>
  </div>
</section>

<section class="container section" id="services">
  <div class="section-label">WHAT WE DO</div>
  <h2 class="section-title">Our Digital Services</h2>
  <p class="section-desc">
    Everything you need to build, launch and grow your digital presence.
  </p>
  <div class="services">
    <article class="card">
      <div class="number">01 / DEVELOPMENT</div>
      <h3>Website Development</h3>
      <p>Modern, responsive and high-performance websites designed to make your brand stand out.</p>
    </article>
    <article class="card">
      <div class="number">02 / APPLICATIONS</div>
      <h3>App Development</h3>
      <p>Smart mobile application experiences built around your business goals and customer needs.</p>
    </article>
    <article class="card">
      <div class="number">03 / DESIGN</div>
      <h3>UI/UX Design</h3>
      <p>Beautiful, intuitive and user-friendly interfaces that turn ideas into meaningful experiences.</p>
    </article>
    <article class="card">
      <div class="number">04 / BRANDING</div>
      <h3>Brand Identity</h3>
      <p>Consistent digital visuals and brand experiences that help businesses build recognition.</p>
    </article>
    <article class="card">
      <div class="number">05 / DIGITAL</div>
      <h3>Digital Solutions</h3>
      <p>Practical technology solutions to simplify workflows and improve online experiences.</p>
    </article>
    <article class="card">
      <div class="number">06 / SUPPORT</div>
      <h3>Website Maintenance</h3>
      <p>Updates, improvements and ongoing support to keep your website running smoothly.</p>
    </article>
  </div>
</section>

<section class="about section" id="about">
  <div class="container about-grid">
    <div class="about-box">
      <div>
        <h2>NEXORA<br>LABS.</h2>
        <span>INNOVATE. BUILD. ELEVATE.</span>
      </div>
    </div>
    <div>
      <div class="section-label">WHO WE ARE</div>
      <h2 class="section-title">Ideas Into Digital Reality.</h2>
      <p class="section-desc">
        Nexora Labs is a digital technology studio focused on
        creating modern websites, applications and creative
        digital solutions. Our goal is to combine innovation,
        design and technology to build meaningful experiences.
      </p>
      <div class="check">✓ Modern & user-focused design</div>
      <div class="check">✓ Quality-driven development</div>
      <div class="check">✓ Mobile-first experiences</div>
    </div>
  </div>
</section>

<section class="container section" id="projects">
  <div class="section-label">OUR WORK</div>
  <h2 class="section-title">Selected Projects</h2>
  <p class="section-desc">A glimpse of the digital experiences we aim to create.</p>
  <div class="projects">
    <article class="project">
      <div class="project-art">WEB<span style="color:#316BFF">.</span></div>
      <div class="project-info">
        <h3>Business Website</h3>
        <p>Modern digital presence for growing businesses.</p>
      </div>
    </article>
    <article class="project">
      <div class="project-art">APP<span style="color:#316BFF">.</span></div>
      <div class="project-info">
        <h3>Mobile Application</h3>
        <p>Simple and intuitive mobile-first experiences.</p>
      </div>
    </article>
  </div>
</section>

<section class="container section">
  <div class="cta">
    <div class="section-label">HAVE AN IDEA?</div>
    <h2>Let's Build Something<br>Extraordinary.</h2>
    <p>Your next big idea deserves a powerful digital presence.</p>
    <a class="btn" href="#contact">Let's Get Started ↗</a>
  </div>
</section>

<section class="container section" id="contact">
  <div class="section-label">GET IN TOUCH</div>
  <h2 class="section-title">Let's Talk About Your Project.</h2>
  <p class="section-desc">Tell us about your idea and let's create something great together.</p>
  <div class="contact-grid">
    <div class="contact-card">
      <h3>NEXORA LABS.</h3>
      <p>INNOVATE. BUILD. ELEVATE.</p>
      <p>Have a project in mind? Contact us and let's discuss how we can bring your idea to life.</p>
      <p><strong>Email:</strong> YOUR_EMAIL_HERE</p>
      <p><strong>WhatsApp:</strong> YOUR_NUMBER_HERE</p>
    </div>
    <form onsubmit="sendMessage(event)">
      <input id="name" placeholder="Your Name" required>
      <input id="email" type="email" placeholder="Your Email" required>
      <textarea id="message" placeholder="Tell us about your project..." required></textarea>
      <button class="btn" type="submit">Send Message ↗</button>
    </form>
  </div>
</section>
</main>

<footer>
  © <span id="year"></span> Nexora Labs. All Rights Reserved.
  <br><br>INNOVATE. BUILD. ELEVATE.
</footer>

<a class="whatsapp" href="https://wa.me/YOUR_NUMBER_HERE" target="_blank" rel="noopener">WhatsApp ↗</a>

<script>
function toggleMenu() {
  document.getElementById('navlinks').classList.toggle('open');
}
document.querySelectorAll('.navlinks a').forEach(link => {
  link.addEventListener('click', () => {
    document.getElementById('navlinks').classList.remove('open');
  });
});
document.getElementById('year').textContent = new Date().getFullYear();

function sendMessage(event) {
  event.preventDefault();
  const name = document.getElementById('name').value;
  const email = document.getElementById('email').value;
  const message = document.getElementById('message').value;

  const phone = "YOUR_NUMBER_HERE";
  const text = `Hello Nexora Labs!
Name: ${name}
Email: ${email}
Project: ${message}`;

  if (phone === "YOUR_NUMBER_HERE") {
    alert("Please add your WhatsApp number in the website code first.");
    return;
  }
  window.open(`https://wa.me/${phone}?text=${encodeURIComponent(text)}`, "_blank");
}
</script>
</body>
</html>
