<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Open+Sans&display=swap" rel="stylesheet" />
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <style>
    :root {
      --dark1: #131313;
      --dark2: #292929;
      --dark3: #424242;
      --gray: #686868;
      --light: #FAFAFA;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      background-color: var(--dark1);
      color: var(--light);
      font-family: 'Open Sans', sans-serif;
    }
    h1, h2, h3 {
      font-family: 'Montserrat', sans-serif;
    }
    header {
      background-color: var(--dark3);
      padding: 20px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    nav a {
      color: var(--light);
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }
    section {
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
    }
    .intro img {
      width: 150px;
      border-radius: 50%;
      margin-bottom: 20px;
    }
    ul {
      list-style: none;
      padding-left: 0;
    }
    ul li {
      margin: 10px 0;
      font-size: 1.1rem;
    }
    ul li::before {
      content: counter(item) ". ";
      counter-increment: item;
      font-weight: bold;
      font-family: 'Montserrat', sans-serif;
      color: var(--gray);
    }
    ul.numbered {
      counter-reset: item;
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
      background: var(--gray);
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
  <h1>Your Name</h1>
  <p>Write a short introduction about yourself here. Who you are, what you do, and your aspirations.</p>
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
  <div>
    <a href="mailto:youremail@example.com"><i class="fas fa-envelope"></i></a>
    <a href="https://www.linkedin.com/in/yourprofile" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="https://www.instagram.com/yourprofile" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="tel:+911234567890"><i class="fas fa-phone"></i></a>
  </div>
  <a class="download-cv" href="your-cv.pdf" download>Download CV</a>
</section>

<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
  AOS.init({
    once: false, // Ensures animations trigger every time you scroll
    duration: 1000,
    offset: 120
  });
</script>

</body>
</html>
