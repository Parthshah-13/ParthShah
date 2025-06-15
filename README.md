<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>

  <!-- Fonts and Icons -->
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@500;700&family=Open+Sans&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>

  <style>
    :root {
      --bg-dark: #0A0F22;
      --card-dark: #1D2233cc;
      --primary: #56B2BB;
      --light: #F0F4F8;
      --text: #BAC7CC;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Open Sans', sans-serif;
      background: linear-gradient(135deg, #0A0F22, #12172C, #0A0F22);
      background-size: 400% 400%;
      animation: shine 15s ease infinite;
      color: var(--text);
    }

    @keyframes shine {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }

    h1, h2 {
      font-family: 'Outfit', sans-serif;
      color: var(--primary);
    }

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(13, 18, 36, 0.9);
      backdrop-filter: blur(8px);
      display: flex;
      justify-content: space-between;
      padding: 15px 10%;
      z-index: 1000;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }

    nav a {
      color: var(--primary);
      margin-left: 20px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 120px 10% 60px;
      transition: all 1s ease;
    }

    .card {
      background: var(--card-dark);
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.4);
      margin-bottom: 60px;
      opacity: 0;
      transform: translateY(40px);
      transition: all 1s ease;
    }

    .visible {
      opacity: 1 !important;
      transform: translateY(0) !important;
    }

    .section-title {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .list-numbered {
      list-style: decimal;
      padding-left: 1.5rem;
      font-weight: 500;
      color: var(--light);
      font-family: 'Open Sans', sans-serif;
    }

    .skills img {
      height: 40px;
      margin: 8px 15px;
    }

    .contact-icons a {
      color: var(--primary);
      margin: 0 15px;
      font-size: 24px;
    }

    footer {
      text-align: center;
      padding: 40px 10%;
      font-size: 14px;
      color: var(--text);
      border-top: 1px solid #2d3145;
    }

    .profile-pic {
      width: 120px;
      border-radius: 50%;
      margin-bottom: 20px;
      border: 2px solid var(--primary);
    }

    @media(max-width: 768px) {
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

  <!-- NAVIGATION -->
  <nav>
    <div><strong>My Portfolio</strong></div>
    <div>
      <a href="#intro">Intro</a>
      <a href="#qualification">Qualification</a>
      <a href="#experience">Experience</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- INTRO -->
  <section id="intro" class="fade-section">
    <div class="card">
      <img src="your-photo.jpg" class="profile-pic" alt="Your Photo">
      <h1 class="section-title">Hello, I'm [Your Name]</h1>
      <p>A passionate construction manager aiming to lead high-impact PMC projects and build a firm of 200+ employees. Here's a glimpse into my journey.</p>
    </div>
  </section>

  <!-- QUALIFICATION -->
  <section id="qualification" class="fade-section">
    <div class="card">
      <h2 class="section-title">1. Qualifications</h2>
      <ul class="list-numbered">
        <li>Master’s in Construction Engineering and Management</li>
        <li>Bachelor’s in Civil Engineering</li>
      </ul>
    </div>
  </section>

  <!-- EXPERIENCE -->
  <section id="experience" class="fade-section">
    <div class="card">
      <h2 class="section-title">2. Work Experience</h2>
      <ul class="list-numbered">
        <li>Site Engineer – XYZ PMC</li>
        <li>Intern – ABC Constructions</li>
      </ul>
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="fade-section">
    <div class="card">
      <h2 class="section-title">3. Skills</h2>
      <ul class="list-numbered">
        <li>AutoCAD <img src="autocad-logo.png" alt="AutoCAD Logo"></li>
        <li>Revit <img src="revit-logo.png" alt="Revit Logo"></li>
        <li>Primavera / MS Project</li>
      </ul>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects" class="fade-section">
    <div class="card">
      <h2 class="section-title">4. College Projects</h2>
      <ul class="list-numbered">
        <li>Pour Planning for a G+11 Residential Tower</li>
        <li>Material Management & Inventory System Study</li>
        <li>Earned Value Analysis on Live Project</li>
      </ul>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="fade-section">
    <div class="card">
      <h2 class="section-title">5. Contact</h2>
      <p>Let's connect:</p>
      <div class="contact-icons">
        <a href="tel:+91XXXXXXXXXX"><i class="fas fa-phone"></i></a>
        <a href="mailto:you@example.com"><i class="fas fa-envelope"></i></a>
        <a href="https://linkedin.com/in/yourprofile" target="_blank"><i class="fab fa-linkedin"></i></a>
        <a href="cv.pdf" download><i class="fas fa-file-download"></i></a>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>© 2025 Your Name. All rights reserved.</p>
  </footer>

  <!-- SCROLL TRIGGER ANIMATION -->
  <script>
    const fadeSections = document.querySelectorAll('.fade-section');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if(entry.isIntersecting){
          entry.target.classList.add('visible');
        }
      });
    }, {threshold: 0.1});

    fadeSections.forEach(section => observer.observe(section));
  </script>

</body>
</html>
