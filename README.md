<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Open+Sans&family=Poppins:wght@600&display=swap" rel="stylesheet" />
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    :root {
      --dark1: #0f0f0f;
      --dark2: #1a1a1a;
      --dark3: #2a2a2a;
      --gray: #999999;
      --light: #FAFAFA;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      background: linear-gradient(-45deg, #1a1a1a, #222, #1a1a1a, #111);
      background-size: 400% 400%;
      animation: shineBackground 15s ease infinite;
      color: var(--light);
      font-family: 'Open Sans', sans-serif;
    }

    @keyframes shineBackground {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }

    h1, h2, h3 {
      font-family: 'Poppins', sans-serif;
      color: #00bfff;
      text-align: center;
      margin-bottom: 20px;
    }

    header {
      background-color: var(--dark3);
      padding: 20px 10px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.4);
    }

    nav a {
      color: var(--light);
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #00bfff;
    }

    section {
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
      transition: all 0.5s ease-in-out;
    }

    .intro img {
      width: 150px;
      border-radius: 50%;
      margin-bottom: 20px;
      display: block;
      margin-left: auto;
      margin-right: auto;
      box-shadow: 0 0 15px #00bfff;
    }

    ul {
      list-style: none;
      padding-left: 0;
    }

    ul li {
      margin: 10px 0;
      font-size: 1.1rem;
      padding-left: 30px;
      position: relative;
      transition: transform 0.3s ease;
    }

    ul li:hover {
      transform: translateX(10px);
    }

    ul.numbered {
      counter-reset: item;
    }

    ul.numbered li::before {
      counter-increment: item;
      content: counter(item, decimal-leading-zero) ". ";
      position: absolute;
      left: 0;
      color: #00bfff;
      font-weight: bold;
      font-family: 'Poppins', sans-serif;
    }

    .skills img {
      height: 40px;
      margin-right: 10px;
      vertical-align: middle;
    }

    .contact a {
      color: var(--light);
      margin: 0 10px;
      font-size: 1.5rem;
      transition: color 0.3s;
    }

    .contact a:hover {
      color: #00bfff;
    }

    .download-cv {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      background: var(--dark2);
      border-radius: 5px;
      color: var(--light);
      text-decoration: none;
      transition: background 0.3s ease;
    }

    .download-cv:hover {
      background: #00bfff;
    }

    p {
      text-align: center;
      font-size: 1.1rem;
      line-height: 1.6;
    }
  </style>
</head>
<body>

<header>
  <nav>
    <a href="#intro">Home</a>
    <a href="#qualifications">Qualifications</a>
    <a href="#experience">Experience</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section id="intro" class="intro" data-aos="fade-up">
  <img src="your-image.jpg" alt="Profile Picture" />
  <h1>Parmishan</h1>
  <p>I’m a passionate construction management graduate aspiring to lead innovative projects. My goal is to create large-scale project management consultancies that transform cities.</p>
</section>

<section id="qualifications" data-aos="fade-up">
  <h2>Qualifications</h2>
  <ul class="numbered">
    <li>Master’s in Construction Engineering and Management – XYZ University</li>
    <li>Bachelor’s in Civil Engineering – ABC College</li>
  </ul>
</section>

<section id="experience" data-aos="fade-up">
  <h2>Companies Worked In</h2>
  <ul class="numbered">
    <li>Intern – L&T Construction</li>
    <li>Junior Engineer – XYZ Pvt Ltd</li>
  </ul>
</section>

<section id="skills" class="skills" data-aos="fade-up">
  <h2>Skills</h2>
  <ul class="numbered">
    <li><img src="autocad-logo.png" alt="AutoCAD" /> AutoCAD</li>
    <li><img src="revit-logo.png" alt="Revit" /> Revit</li>
    <li><img src="msproject-logo.png" alt="MS Project" /> MS Project</li>
    <li><img src="primavera-logo.png" alt="Primavera" /> Primavera</li>
  </ul>
</section>

<section id="projects" data-aos="fade-up">
  <h2>College Projects</h2>
  <ul class="numbered">
    <li>Pour Planning and Scheduling of G+10 Building</li>
    <li>Earned Value Management Analysis</li>
    <li>Material and Inventory Management Strategy</li>
  </ul>
</section>

<section id="contact" class="contact" data-aos="fade-up">
  <h2>Contact Me</h2>
  <div style="text-align:center;">
    <a href="mailto:youremail@example.com"><i class="fas fa-envelope"></i></a>
    <a href="https://www.linkedin.com/in/yourprofile" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://www.instagram.com/yourprofile" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="tel:+911234567890"><i class="fas fa-phone"></i></a>
  </div>
  <div style="text-align:center;">
    <a class="download-cv" href="your-cv.pdf" download>Download CV</a>
  </div>
</section>

<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
  AOS.init({
    once: false,
    duration: 1000,
    offset: 120
  });
</script>

</body>
</html>
