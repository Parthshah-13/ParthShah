<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Your Name | Portfolio</title>

  <!-- Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500&family=Playfair+Display:wght@600&display=swap" rel="stylesheet">

  <style>
    :root {
      --cream: #E8DFE0;
      --sage: #8D9B6A;
      --blue-grey: #8A9EA7;
      --peach: #DAB692;
      --brown: #8F5B34;
      --text-dark: #2b2b2b;
      --white: #ffffff;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'DM Sans', sans-serif;
      background: var(--cream);
      color: var(--text-dark);
      scroll-behavior: smooth;
    }

    h1, h2 {
      font-family: 'Playfair Display', serif;
      color: var(--brown);
    }

    nav {
      background: rgba(250, 248, 247, 0.8);
      backdrop-filter: blur(8px);
      padding: 15px 30px;
      position: sticky;
      top: 0;
      z-index: 100;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    nav a {
      color: var(--text-dark);
      font-weight: 500;
      text-decoration: none;
      margin: 0 15px;
    }

    nav a:hover {
      color: var(--blue-grey);
    }

    header {
      text-align: center;
      padding: 60px 20px 20px;
    }

    header img {
      border-radius: 50%;
      width: 150px;
      height: 150px;
      object-fit: cover;
      margin-bottom: 20px;
      border: 3px solid var(--brown);
    }

    section {
      max-width: 900px;
      margin: 60px auto;
      background: var(--white);
      padding: 40px;
      border-radius: 16px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.8s ease-out;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .cv-button {
      background-color: var(--blue-grey);
      color: white;
      text-decoration: none;
      padding: 10px 20px;
      border-radius: 8px;
      font-weight: bold;
      display: inline-block;
      margin-top: 20px;
    }

    .cv-button:hover {
      background-color: var(--sage);
    }

    .skill-box img {
      filter: grayscale(100%);
      transition: filter 0.3s, transform 0.3s;
      margin: 10px;
    }

    .skill-box:hover img {
      filter: grayscale(0%);
      transform: scale(1.1);
    }

    .socials a img {
      margin: 0 10px;
      transition: transform 0.3s, filter 0.3s;
    }

    .socials a:hover img {
      transform: scale(1.2);
      filter: brightness(1.2);
    }

    footer {
      text-align: center;
      padding: 30px;
      font-size: 0.9em;
      color: var(--blue-grey);
    }
  </style>
</head>

<body>
  <nav>
    <div><strong>My Portfolio</strong></div>
    <div>
      <a href="#intro">Intro</a>
      <a href="#qualifications">Qualifications</a>
      <a href="#experience">Experience</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <header id="intro">
    <img src="your-photo.jpg" alt="Your Photo"/>
    <h1>Hello, I'm Your Name</h1>
    <p>I'm a passionate Construction Manager with a vision to transform the industry through smart project execution and leadership.</p>
  </header>

  <section id="qualifications">
    <h2>Qualifications</h2>
    <p>M.Tech in Construction Engineering and Management</p>
    <p>B.E. in Civil Engineering</p>
  </section>

  <section id="experience">
    <h2>Companies & Organizations</h2>
    <p>Worked at XYZ Pvt Ltd as Site Engineer</p>
    <p>Interned at ABC Infrastructure</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="skill-box">
      <img src="autocad-logo.png" alt="AutoCAD" width="50"/>
      <img src="revit-logo.png" alt="Revit" width="50"/>
      <img src="msproject-logo.png" alt="MS Project" width="50"/>
    </div>
  </section>

  <section id="projects">
    <h2>College Projects</h2>
    <p>Pour Planning and Management of G+11 Structure</p>
    <p>Inventory Control and Cost Analysis for RCC Buildings</p>
    <p>Use of Drones in Construction Monitoring</p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <div class="socials">
      <a href="https://linkedin.com/in/yourprofile" target="_blank"><img src="linkedin.png" width="30" alt="LinkedIn"/></a>
      <a href="mailto:youremail@example.com"><img src="email.png" width="30" alt="Email"/></a>
      <a href="https://instagram.com/yourprofile" target="_blank"><img src="instagram.png" width="30" alt="Instagram"/></a>
      <a href="tel:+919999999999"><img src="phone.png" width="30" alt="Phone"/></a>
    </div>
    <a class="cv-button" href="YourCV.pdf" target="_blank">Download CV</a>
  </section>

  <footer>© 2025 Your Name. All rights reserved.</footer>

  <script>
    // Reveal sections on scroll
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
