# Portfolio-Project

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>YADNESH - Portfolio</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: #000;
      color: white;
    }

    a {
      text-decoration: none;
      color: white;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: #000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 60px;
      z-index: 1000;
    }

    header h1 {
      color: #ff3c68;
      font-weight: 700;
      font-size: 24px;
    }

    nav a {
      margin-left: 25px;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ff3c68;
    }

    .hero {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 150px 60px 60px;
      min-height: 100vh;
    }

    .hero-text {
      flex: 1;
      max-width: 600px;
    }

    .hero-text h3 {
      font-weight: 400;
      color: #ccc;
      margin-bottom: 15px;
    }

    .hero-text h1 {
      font-size: 3rem;
      line-height: 1.3;
    }

    .hero-text h1 span {
      color: #ff3c68;
    }

    .hero-image {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    .hero-image img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
    }

    section#about {
      padding: 80px 60px;
      background: #0a0a0a;
      display: flex;
      align-items: center;
      gap: 40px;
      flex-wrap: wrap;
    }

    .about-image {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    .about-image img {
      max-width: 350px;
      border-radius: 20px;
      background: #1a1a1a;
      padding: 10px;
    }

    .about-content {
      flex: 2;
      max-width: 700px;
    }

    .about-content h2 {
      font-size: 2.5rem;
      margin-bottom: 20px;
    }

    .about-content p {
      color: #ccc;
      margin-bottom: 30px;
      line-height: 1.7;
    }

    .tabs {
      display: flex;
      gap: 30px;
      margin-bottom: 20px;
    }

    .tab {
      cursor: pointer;
      font-weight: 500;
      position: relative;
    }

    .tab.active::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 100%;
      height: 2px;
      background: #ff3c68;
    }

    .tab-content {
      display: none;
    }

    .tab-content.active {
      display: block;
    }

    .tab-content h4 {
      color: #ff3c68;
      margin-bottom: 5px;
    }

    @media (max-width: 768px) {
      .hero, #about {
        flex-direction: column;
        text-align: center;
        padding: 120px 20px 40px;
      }

      .hero-text h1 {
        font-size: 2.2rem;
      }

      .tabs {
        justify-content: center;
      }

      .about-image img {
        max-width: 250px;
      }
    }

    /* Style for Hobby Section */
    #hobbies {
      padding: 80px 60px;
      background: #0a0a0a;
      color: white;
    }

    #hobbies h2 {
      font-size: 2.5rem;
      color: #ff3c68;
      margin-bottom: 40px;
      text-align: center;
    }

    .hobby-list {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
    }

    .hobby-item {
      background: #111;
      padding: 25px 30px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
      max-width: 250px;
      text-align: center;
      color: #ccc;
    }

    .hobby-item h4 {
      color: #ff3c68;
      margin-bottom: 10px;
    }

    .hobby-item p {
      color: #ccc;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>Yadnesh</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#about">About</a>
      <a href="#achievements">Achievements</a>
      <a href="#certificate">Certificate</a>
      <a href="#hobbies">Hobbies</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-text">
      <h3>Future Programmer</h3>
      <h1>Hi, I'm <span>Yadnesh Nilkanth Tayade</span><br>From India</h1>
    </div>
    <div class="hero-image">
      <img src="YADNESHTAYADE2.jpg" alt="Yadnesh">
    </div>
  </section>

  <!-- About Section -->
  <section id="about">
    <div class="about-image">
      <img src="ABOUTME.jpg" alt="About Photo">
    </div>
    <div class="about-content">
      <h2>About Me</h2>
      <p>Hello! My name is Yadnesh Nilkanth Tayade, and I’m from Akola, Maharashtra. I am currently a first-year student at MITAOE, Pune, pursuing my passion for technology in the AI-ML batch.</p>
      <div class="tabs">
        <div class="tab active" data-tab="skills">Skills</div>
        <div class="tab" data-tab="experience">Experience</div>
        <div class="tab" data-tab="education">Education</div>
      </div>
      <div class="tab-content active" id="skills">
        <h4>C language</h4>
        <p>I know the basics of the C language and am currently learning more.</p>
        <h4>Python language</h4>
        <p>I have a solid understanding of python programming, though I’m not yet at an advanced level.</p>
        <h4>Data analysis</h4>
        <p>I'm working towards becoming a proficient data analyst.</p>
      </div>
      <div class="tab-content" id="experience">
        <p>I may not have experience yet, but I am eager to learn and embrace new opportunities.</p>
      </div>
      <div class="tab-content" id="education">
        <p>I passed the 10th grade from the ICSE board with over 85% and the 12th grade from the HSC board with over 85%. Now, I'm pursuing my AIML degree at MITAOE, Pune.</p>
      </div>
    </div>
  </section>

  <!-- Hobbies Section -->
  <section id="hobbies">
    <h2>Hobbies</h2>
    <div class="hobby-list">
      <div class="hobby-item">
        <h4>Gaming</h4>
        <p>Gaming is not only fun but also sharpens my problem-solving and strategic thinking abilities.</p>
      </div>
      <div class="hobby-item">
        <h4>Programming</h4>
        <p>Programming is both a hobby and a passion, and I love learning new languages and techniques.</p>
      </div>
      <div class="hobby-item">
        <h4>Volleyball</h4>
        <p>Volleyball helps me stay fit, and I enjoy playing team sports with my friends.</p>
      </div>
    </div>
  </section>

  <!-- Achievements Section -->
  <section id="achievements" style="padding: 80px 60px; background: #000; color: white;">
    <h2 style="font-size: 2.5rem; color: #ff3c68; margin-bottom: 40px; text-align: center;">Achievements</h2>
    <div style="display: flex; flex-direction: column; gap: 25px; max-width: 900px; margin: auto;">
      <div style="background: #111; padding: 20px 25px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.3);">
        <h4 style="color: #ff3c68; margin-bottom: 10px;">Hackathon Participation</h4>
        <p style="color: #ccc;">Participated in my first university-level hackathon and collaborated on a team project that focused on solving real-world problems using AI solutions.</p>
      </div>
      <div style="background: #111; padding: 20px 25px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.3);">
        <h4 style="color: #ff3c68; margin-bottom: 10px;">Python Mini Projects</h4>
        <p style="color: #ccc;">Created several mini projects using Python, including a calculator, number guessing game, and basic data visualizations using Matplotlib and Pandas.</p>
      </div>
      <div style="background: #111; padding: 20px 25px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.3);">
        <h4 style="color: #ff3c68; margin-bottom: 10px;">Course Certifications</h4>
        <p style="color: #ccc;">Earned certifications in Python basics, C programming, and introductory Data Analytics from online platforms like Coursera and Great Learning.</p>
      </div>
    </div>
  </section>

  <!-- Certificate Section -->
  <section id="certificate" style="padding: 80px 60px; background: #000; text-align: center;">
    <h2 style="font-size: 2.5rem; margin-bottom: 40px; color: #ff3c68;">Certificates</h2>
    <div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 30px;">
      <img src="CERTIFICATE1.jpg" alt="Certificate 1" style="max-width: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);" />
      <img src="CERTIFICATE2.jpg" alt="Certificate 2" style="max-width: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);" />
      <img src="CERTIFICATE3.jpg" alt="Certificate 3" style="max-width: 250px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);" />
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills">
    <h2>My Skills</h2>
    <div class="skills-container">
      <div class="skill">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/c-programming.png" alt="C Programming"/>
        <h3>C Language</h3>
        <p>Basic understanding of C programming concepts and syntax.</p>
      </div>
      <div class="skill">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/python.png" alt="Python"/>
        <h3>Python</h3>
        <p>Proficient in Python for data analysis, scripting, and automation.</p>
      </div>
      <div class="skill">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/html-5.png" alt="HTML"/>
        <h3>HTML</h3>
        <p>Understanding of HTML structure for building web pages.</p>
      </div>
      <div class="skill">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/css3.png" alt="CSS"/>
        <h3>CSS</h3>
        <p>Basic styling and layout techniques for web development using CSS.</p>
      </div>
      <div class="skill">
        <img src="https://img.icons8.com/ios-filled/50/ffffff/javascript.png" alt="JavaScript"/>
        <h3>JavaScript</h3>
        <p>Basic JavaScript for adding interactivity to web pages.</p>
      </div>
    </div>
  </section>
  
  <style>
    #skills {
      padding: 80px 60px;
      background: #0a0a0a;
      color: white;
    }
  
    #skills h2 {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 50px;
      color: #ff3c68;
    }
  
    .skills-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
      justify-items: center;
    }
  
    .skill {
      background: #111;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
      text-align: center;
      max-width: 280px;
      width: 100%;
    }
  
    .skill img {
      margin-bottom: 15px;
      max-width: 60px;
    }
  
    .skill h3 {
      font-size: 1.5rem;
      color: #ff3c68;
      margin-bottom: 10px;
    }
  
    .skill p {
      font-size: 1rem;
      color: #ccc;
    }
  
    @media (max-width: 768px) {
      #skills h2 {
        font-size: 2rem;
      }
  
      .skill {
        padding: 15px;
      }
    }
  </style>
  <!-- Alternative Project Section -->
  <section id="projects" style="padding: 80px 60px; background: #0a0a0a; color: white;">
    <h2 style="text-align: center; font-size: 2.5rem; margin-bottom: 50px; color: #ff3c68;">My Projects</h2>
    <p style="text-align: center; font-size: 1.2rem; color: #ccc; margin-bottom: 40px;">Explore some of the projects I have worked on. These projects showcase my programming skills and passion for creating solutions.</p>
    
    <div class="projects-container" style="display: flex; justify-content: space-between; flex-wrap: wrap;">
      <div class="project-card" style="background: #111; padding: 20px; width: 32%; margin-bottom: 30px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5); transition: transform 0.3s ease;">
        <img src="project1.png" alt="Project 1" style="width: 100%; border-radius: 10px; transition: transform 0.3s ease;">
        <h3 style="font-size: 1.8rem; color: #ff3c68; margin: 15px 0;">Project 1</h3>
        <p style="font-size: 1rem; color: #ccc;">A simple website created with HTML, CSS, and JavaScript to showcase basic web development skills.</p>
        <a href="#" style="display: inline-block; margin-top: 10px; color: #ff3c68; text-decoration: none; font-weight: bold;">View Project</a>
      </div>
  
      <div class="project-card" style="background: #111; padding: 20px; width: 32%; margin-bottom: 30px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5); transition: transform 0.3s ease;">
        <img src="project2.png" alt="Project 2" style="width: 100%; border-radius: 10px; transition: transform 0.3s ease;">
        <h3 style="font-size: 1.8rem; color: #ff3c68; margin: 15px 0;">Project 2</h3>
        <p style="font-size: 1rem; color: #ccc;">A data analysis project utilizing Python, Pandas, and Matplotlib to visualize real-world data sets.</p>
        <a href="#" style="display: inline-block; margin-top: 10px; color: #ff3c68; text-decoration: none; font-weight: bold;">View Project</a>
      </div>
  
      <div class="project-card" style="background: #111; padding: 20px; width: 32%; margin-bottom: 30px; border-radius: 15px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5); transition: transform 0.3s ease;">
        <img src="project3.png" alt="Project 3" style="width: 100%; border-radius: 10px; transition: transform 0.3s ease;">
        <h3 style="font-size: 1.8rem; color: #ff3c68; margin: 15px 0;">Project 3</h3>
        <p style="font-size: 1rem; color: #ccc;">A small game created using Python and the Pygame library to showcase my interest in game development.</p>
        <a href="#" style="display: inline-block; margin-top: 10px; color: #ff3c68; text-decoration: none; font-weight: bold;">View Project</a>
      </div>
    </div>
  </section>
  
  <style>
    .project-card:hover {
      transform: translateY(-10px);
    }
  
    .project-card img:hover {
      transform: scale(1.05);
    }
  
    @media (max-width: 768px) {
      .projects-container {
        flex-direction: column;
        align-items: center;
      }
  
      .project-card {
        width: 80%;
      }
    }
  </style>
  

  <!-- Contact Section -->
  <section id="contact" style="padding: 80px 60px; background: #0a0a0a; display: flex; flex-wrap: wrap; justify-content: space-between; align-items: flex-start; color: white;">
    <div style="flex: 1; min-width: 300px; margin-bottom: 30px;">
      <h2 style="font-size: 2.5rem; margin-bottom: 20px;">Contact Me</h2>
      <p style="margin-bottom: 15px;"><span style="color: #ff3c68;">📧</span> yadneshtayade2@gmail.com</p>
      <p style="margin-bottom: 15px;"><span style="color: #ff3c68;">📞</span> 0123456789</p>
      <div style="margin: 20px 0;">
        <a href="#" style="margin-right: 15px;"><img src="https://img.icons8.com/ios-filled/24/ffffff/facebook--v1.png"/></a>
        <a href="#" style="margin-right: 15px;"><img src="https://img.icons8.com/ios-filled/24/ffffff/twitter.png"/></a>
        <a href="#" style="margin-right: 15px;"><img src="https://img.icons8.com/ios-filled/24/ffffff/instagram-new.png"/></a>
        <a href="#"><img src="https://img.icons8.com/ios-filled/24/ffffff/linkedin.png"/></a>
      </div>
      <a href="#" style="display: inline-block; padding: 12px 24px; background: #ff3c68; border-radius: 6px; color: white; font-weight: 600; margin-top: 10px;">Download CV</a>
    </div>
    <div style="flex: 1; min-width: 300px;">
      <form>
        <input type="text" placeholder="Your Name" style="width: 100%; padding: 15px; margin-bottom: 15px; border: none; border-radius: 6px; background: #1e1e1e; color: white;">
        <input type="email" placeholder="Your Email" style="width: 100%; padding: 15px; margin-bottom: 15px; border: none; border-radius: 6px; background: #1e1e1e; color: white;">
        <textarea placeholder="Your Message" rows="5" style="width: 100%; padding: 15px; margin-bottom: 15px; border: none; border-radius: 6px; background: #1e1e1e; color: white;"></textarea>
        <button type="submit" style="padding: 12px 24px; background: #ff3c68; border: none; border-radius: 6px; color: white; font-weight: 600;">Submit</button>
      </form>
    </div>
  </section>

  <!-- JavaScript for Tabs -->
  <script>
    const tabs = document.querySelectorAll('.tab');
    const contents = document.querySelectorAll('.tab-content');

    tabs.forEach(tab => {
      tab.addEventListener('click', () => {
        tabs.forEach(t => t.classList.remove('active'));
        tab.classList.add('active');

        contents.forEach(c => c.classList.remove('active'));
        document.getElementById(tab.dataset.tab).classList.add('active');
      });
    });
  </script>

</body>
</html>
