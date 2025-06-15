<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>
  <style>
    /* Reset and base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(145deg, #0A0F22, #1D2233);
      color: #F0F4F8;
      line-height: 1.6;
    }

    a {
      color: #56B2BB;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    a:hover {
      color: #BAC7CC;
    }

    /* Header */
    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: #0A0F22;
      padding: 1rem 2rem;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 4px 6px rgba(0,0,0,0.3);
    }

    header h1 {
      color: #56B2BB;
      font-size: 1.8rem;
    }

    nav a {
      margin-left: 1.5rem;
      font-weight: bold;
      font-size: 1rem;
    }

    /* Sections */
    section {
      padding: 100px 10% 60px;
      transition: all 0.4s ease-in-out;
    }

    section:nth-child(even) {
      background-color: #1D2233;
    }

    section:nth-child(odd) {
      background-color: #0A0F22;
    }

    section h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
      color: #56B2BB;
      border-bottom: 2px solid #56B2BB;
      padding-bottom: 0.5rem;
    }

    ul {
      margin-left: 1.2rem;
    }

    ul li {
      margin-bottom: 0.6rem;
      font-size: 1.1rem;
    }

    .container {
      max-width: 1000px;
      margin: 0 auto;
    }

    .section-number {
      font-weight: bold;
      color: #BAC7CC;
      margin-right: 10px;
    }

    /* Intro spacing below navbar */
    .spacer {
      height: 80px;
    }

    /* Add subtle shine effect */
    body::before {
      content: "";
      position: fixed;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle at center, rgba(255,255,255,0.05), transparent 70%);
      z-index: 0;
      pointer-events: none;
      animation: shine 15s linear infinite;
    }

    @keyframes shine {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

  </style>
</head>
<body>

  <header>
    <h1>Parth Shah</h1>
    <nav>
      <a href="#intro">Intro</a>
      <a href="#qualification">Qualification</a>
      <a href="#experience">Experience</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <div class="spacer"></div>

  <section id="intro">
    <div class="container">
      <h2>Intro</h2>
      <p>Hello! I am Parth Shah, a passionate Construction Management student with a vision to build a leading PMC firm. I aim to lead projects that redefine skylines and grow into a CEO role by 35. Welcome to my portfolio!</p>
    </div>
  </section>

  <section id="qualification">
    <div class="container">
      <h2>Qualification</h2>
      <ul>
        <li><span class="section-number">1.</span> Master’s in Construction Engineering and Management – [Your University]</li>
        <li><span class="section-number">2.</span> Bachelor's in Civil Engineering – [Your College]</li>
        <li><span class="section-number">3.</span> Certifications in MS Project, Primavera, AutoCAD, and more</li>
      </ul>
    </div>
  </section>

  <section id="experience">
    <div class="container">
      <h2>Experience</h2>
      <ul>
        <li><span class="section-number">1.</span> Internship at [PMC Company Name] – Managed 3 sites alongside site engineers</li>
        <li><span class="section-number">2.</span> Assisted in pour planning, material inventory management, and earned value analysis</li>
        <li><span class="section-number">3.</span> Participated in safety analysis and risk identification exercises</li>
      </ul>
    </div>
  </section>

  <section id="skills">
    <div class="container">
      <h2>Skills</h2>
      <ul>
        <li><span class="section-number">1.</span> Project Planning & Scheduling</li>
        <li><span class="section-number">2.</span> Quantity Surveying</li>
        <li><span class="section-number">3.</span> Risk Identification & Safety Management</li>
        <li><span class="section-number">4.</span> Inventory & Material Management</li>
        <li><span class="section-number">5.</span> Earned Value Analysis</li>
      </ul>
    </div>
  </section>

  <section id="projects">
    <div class="container">
      <h2>Projects</h2>
      <ul>
        <li><span class="section-number">1.</span> Studio 2 Portfolio – Pour planning and risk management simulation</li>
        <li><span class="section-number">2.</span> Blog: “What does a Site Engineer actually do?”</li>
        <li><span class="section-number">3.</span> Cost comparison study – AAC Blocks vs Red Bricks</li>
      </ul>
    </div>
  </section>

  <section id="contact">
    <div class="container">
      <h2>Contact</h2>
      <p>Email: yourname@example.com</p>
      <p>Phone: +91 XXXXX XXXXX</p>
      <p>LinkedIn: <a href="https://linkedin.com/in/yourprofile" target="_blank">yourprofile</a></p>
    </div>
  </section>

</body>
</html>
