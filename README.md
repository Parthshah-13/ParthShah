<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>

  <!-- Fonts & Icons -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@500;700&family=Open+Sans&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>
    :root {
      --bg: #E1DFE4;
      --primary: #DF788D;
      --accent: #CD0D32;
      --text: #727272;
      --white: #FFFFFF;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      background-color: var(--bg);
      font-family: 'Open Sans', sans-serif;
      color: var(--text);
    }

    h1, h2, h3 {
      font-family: 'Outfit', sans-serif;
      color: var(--accent);
    }

    nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      background: var(--white);
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      padding: 15px 10%;
      display: flex;
      justify-content: space-between;
      z-index: 1000;
    }

    nav a {
      margin-left: 20px;
      color: var(--accent);
      text-decoration: none;
      font-weight: bold;
      font-family: 'Outfit', sans-serif;
    }

    section {
      padding: 100px 10% 60px;
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.8s ease;
    }

    section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .intro img {
      border-radius: 50%;
      width: 140px;
      margin-bottom: 20px;
    }

    .section-title {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .list-numbered {
      list-style-type: decimal;
      padding-left: 1.2em;
      font-weight: bold;
      font-family: 'Open Sans', sans-serif;
    }

    .skills img {
      height: 40px;
      margin: 10px 15px;
    }

    .contact-icons a {
      color: var(--accent);
      margin: 0 12px;
      font-size: 24px;
    }

    footer {
      background: var(--white);
      text-align: center;
      padding: 40px 10%;
      color: var(--text);
      font-size: 14px;
    }

    @media (max-width: 768px) {
      nav {
        flex-direction: column;
        align-items: flex-start;
      }
      nav a {
        margin: 10px 0;
        display: block;
      }
    }
  </style>
</head>

<body>

  <!-- Navigation -->
  <nav>
    <div><strong>My Portfolio</strong></div>
    <div>
      <a href="#intro">Intro</a>
      <a href="#qualification">Qualification</a>
      <a href="#experience">Experience</a>
      <a href="#skills">Skills</a>
      <a href="#achievements">Achievements</a>
      <a href="#organizations">Organizations</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Sections -->
  <section id="intro" class="fade-scroll">
    <img src="your-photo.jpg" alt="Your Photo">
    <h1 class="section-title">About Me</h1>
    <p>Hello! I’m [Your Name], a construction management professional with a vision to lead large-scale PMC projects. This portfolio showcases my journey and skills.</p>
  </section>

  <section id="qualification" class="fade-scroll">
    <h2 class="section-title">Qualifications</h2>
    <ul class="list-numbered">
      <li>Master’s in Construction Management</li>
      <li>Bachelor’s in Civil Engineering</li>
    </ul>
  </section>

  <section id="experience" class="fade-scroll">
    <h2 class="section-title">Companies I've Worked In</h2>
    <ul class="list-numbered">
      <li>XYZ PMC Solutions</li>
      <li>ABC Constructions</li>
    </ul>
  </section>

  <section id="skills" class="fade-scroll skills">
    <h2 class="section-title">Skills</h2>
    <ul class="list-numbered">
      <li>AutoCAD <img src="autocad-logo.png" alt="AutoCAD"></li>
      <li>Revit <img src="revit-logo.png" alt="Revit"></li>
      <li>MS Project, Primavera</li>
    </ul>
  </section>

  <section id="achievements" class="fade-scroll">
    <h2 class="section-title">Academic Achievements</h2>
    <ul class="list-numbered">
      <li>Topper in Construction Project Planning</li>
      <li>First Prize in Case Study Competition</li>
    </ul>
  </section>

  <section id="organizations" class="fade-scroll">
    <h2 class="section-title">Organizations</h2>
    <ul class="list-numbered">
      <li>Indian Green Building Council – Student Chapter</li>
      <li>ACCE(I) – Young Professionals Wing</li>
    </ul>
  </section>

  <section id="projects" class="fade-scroll">
    <h2 class="section-title">College Projects</h2>
    <ul class="list-numbered">
      <li>Pour Planning for G+11 Residential Tower</li>
      <li>Material Management and Inventory Control Study</li>
      <li>Earned Value Analysis Report – High-Rise Project</li>
    </ul>
  </section>

  <section id="contact" class="fade-scroll">
    <h2 class="section-title">Contact</h2>
    <div class="contact-icons">
      <a href="tel:+91XXXXXXXXXX"><i class="fas fa-phone"></i></a>
      <a href="mailto:yourmail@example.com"><i class="fas fa-envelope"></i></a>
      <a href="https://linkedin.com/in/yourprofile" target="_blank"><i class="fab fa-linkedin"></i></a>
      <a href="https://instagram.com/yourhandle" target="_blank"><i class="fab fa-instagram"></i></a>
      <a href="cv.pdf" download><i class="fas fa-file-download"></i></a>
    </div>
  </section>

  <footer>
    <p>© 2025 Your Name. All rights reserved.</p>
  </footer>

  <!-- Scroll-triggered animation -->
  <script>
    const fadeSections = document.querySelectorAll('.fade-scroll');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        } else {
          entry.target.classList.remove('visible');
        }
      });
    }, { threshold: 0.1 });

    fadeSections.forEach(section => observer.observe(section));
  </script>

</body>
</html>


