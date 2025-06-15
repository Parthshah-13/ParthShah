<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Your Name | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #7dd3fc;
      --accent: #60a5fa;
      --text: #f1f5f9;
      --bg: #0f172a;
      --card-bg: rgba(255, 255, 255, 0.05);
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: var(--text);
      scroll-behavior: smooth;
    }

    nav {
      background: rgba(15, 23, 42, 0.9);
      backdrop-filter: blur(10px);
      padding: 15px 30px;
      position: sticky;
      top: 0;
      z-index: 100;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    nav a {
      color: var(--text);
      margin: 0 15px;
      text-decoration: none;
      font-weight: 500;
    }

    nav a:hover {
      color: var(--accent);
    }

    header {
      text-align: center;
      padding: 60px 20px 20px;
      animation: fadeInDown 1s ease-out;
    }

    header img {
      border-radius: 50%;
      width: 150px;
      height: 150px;
      object-fit: cover;
      margin-bottom: 20px;
      border: 3px solid var(--primary);
    }

    header h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 2.8em;
      margin: 10px 0;
      color: var(--primary);
    }

    header p {
      font-size: 1.2em;
      color: #cbd5e1;
    }

    .intro-text {
      margin-top: 10px;
      font-size: 1.1em;
      color: #d1d5db;
      max-width: 650px;
      margin-left: auto;
      margin-right: auto;
    }

    section {
      max-width: 900px;
      margin: 60px auto;
      background: var(--card-bg);
      backdrop-filter: blur(12px);
      padding: 40px;
      border-radius: 15px;
      border: 1px solid rgba(255, 255, 255, 0.08);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.8s ease-out;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    h2 {
      color: var(--primary);
      margin-top: 0;
      font-family: 'Orbitron', sans-serif;
    }

    ul {
      list-style: none;
      padding: 0;
    }

    li {
      margin-bottom: 12px;
      line-height: 1.6;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .skill-box {
      width: 120px;
      height: 140px;
      text-align: center;
      color: white;
    }

    .skill-box img {
      width: 48px;
      height: 48px;
      filter: grayscale(100%);
      transition: filter 0.3s, transform 0.3s;
    }

    .skill-box:hover img {
      filter: grayscale(0%);
      transform: scale(1.1);
    }

    .cv-button {
      display: inline-block;
      padding: 10px 20px;
      margin-top: 20px;
      background: var(--accent);
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
    }

    .cv-button:hover {
      background: #3b82f6;
    }

    .socials {
      display: flex;
      justify-content: center;
      gap: 30px;
      margin-top: 30px;
    }

    .socials a img {
      width: 32px;
      height: 32px;
      transition: transform 0.3s ease;
    }

    .socials a:hover img {
      transform: scale(1.2);
    }

    footer {
      text-align: center;
      padding: 30px;
      font-size: 0.9em;
      color: #94a3b8;
    }

    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-40px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

<nav>
  <div><a href="#">YourLogo</a></div>
  <div>
    <a href="#qualifications">Qualifications</a>
    <a href="#companies">Companies</a>
    <a href="#skills">Skills</a>
    <a href="#achievements">Achievements</a>
    <a href="#orgs">Organizations</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </div>
</nav>

<header>
  <img src="your-photo.jpg" alt="Your Photo">
  <h1>Your Name</h1>
  <p>Construction Management Professional | Aspiring CEO</p>
  <div class="intro-text">
    I’m a passionate construction management professional who believes in building smarter, faster, and safer. I strive to bring innovation and clarity to every project I take on, from Gantt charts to pouring plans.
  </div>
  <a class="cv-button" href="cv.pdf" download>📄 Download CV</a>
</header>

<section id="qualifications">
  <h2>Qualifications</h2>
  <ul>
    <li>Master's in Construction Engineering & Management – [Your University]</li>
    <li>Bachelor’s in Civil Engineering – [Your University]</li>
  </ul>
</section>

<section id="companies">
  <h2>Companies Worked In</h2>
  <ul>
    <li>Company A – Site Engineer (Jan 2023 – Dec 2023)</li>
    <li>Company B – Intern (Jun 2022 – Aug 2022)</li>
  </ul>
</section>

<section id="skills">
  <h2>Skills</h2>
  <div class="skills">
    <div class="skill-box">
      <img src="autocad.png" alt="AutoCAD">
      <div>AutoCAD</div>
    </div>
    <div class="skill-box">
      <img src="revit.png" alt="Revit">
      <div>Revit</div>
    </div>
    <div class="skill-box">
      <img src="primavera.png" alt="Primavera">
      <div>Primavera</div>
    </div>
  </div>
</section>

<section id="achievements">
  <h2>Academic Achievements</h2>
  <ul>
    <li>Gold Medal – Master’s Program, 2025</li>
    <li>Top 5% – National Civil Engineering Aptitude Test</li>
  </ul>
</section>

<section id="orgs">
  <h2>Organizations & Activities</h2>
  <ul>
    <li>Member – Indian Concrete Institute</li>
    <li>Volunteer – Habitat for Humanity</li>
    <li>Organizer – TechFest 2024</li>
  </ul>
</section>

<section id="projects">
  <h2>College Projects</h2>
  <ul>
    <li><strong>Pour Planning of G+5 RCC Building:</strong> Developed comprehensive pour plan including sequencing, resource scheduling, and safety checklist using MS Project and AutoCAD.</li>
    <li><strong>Material Management Optimization:</strong> Proposed JIT model for concrete works reducing wastage by 18% in simulation study.</li>
    <li><strong>Earned Value Analysis (EVA):</strong> Applied EVA metrics on a simulated infrastructure project; achieved SPI & CPI performance evaluation for cost control.</li>
    <li><strong>BIM Model Integration:</strong> Collaborated in creating a Revit model for a residential structure linked with cost data for 5D visualization.</li>
  </ul>
</section>

<section id="contact">
  <h2>Contact</h2>
  <div class="socials">
    <a href="tel:+911234567890"><img src="phone.png" alt="Phone"></a>
    <a href="mailto:youremail@example.com"><img src="email.png" alt="Email"></a>
    <a href="https://www.linkedin.com/in/yourprofile" target="_blank"><img src="linkedin.png" alt="LinkedIn"></a>
    <a href="https://www.instagram.com/yourusername" target="_blank"><img src="instagram.png" alt="Instagram"></a>
  </div>
</section>

<footer>
  © 2025 Your Name — Built with 💙 using GitHub Pages
</footer>

<script>
  const sections = document.querySelectorAll('section');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  }, { threshold: 0.1 });

  sections.forEach(section => observer.observe(section));
</script>

</body>
</html>

