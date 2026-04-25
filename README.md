# Ex01 Portfolio
## Date: 25.04.2025
## Name : Kushma S
## Reg no : 212224040168

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kushma | Experiment-1</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Navbar -->
  <header>
    <h1 class="logo">Kushma</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#tech">Tech Stack</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div class="hero-content">
        <div class="hero-text">
          
        <h2>Hey there, I'm <span>Kushma</span></h2>
        <p>Designer | Full Stack Developer </p>
        <p class="tagline">I build complete web experiences</p>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="section">
    <h2>About Me</h2>
    <p>
      I am a second-year engineering student pursuing Computer Science and Engineering. I am an aspiring and dedicated developer, actively working toward becoming a full-stack developer. I enjoy building web applications and exploring both frontend and backend technologies. I am constantly learning new tools and frameworks to improve my skills and stay updated with industry trends. Passionate about problem-solving, I aim to create efficient, scalable, and user-friendly solutions.
    </p>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="section light">
    <h2>Core Skills</h2>

    <div class="skill-box">
      <h3>Design</h3>
      <div class="skills">
        <span>UI/UX Design</span>
        <span>Canva</span>
        <span>Figma</span>
      </div>
    </div>

    <div class="skill-box">
      <h3>Frontend</h3>
      <div class="skills">
        <span>HTML</span>
        <span>CSS</span>
        <span>JavaScript</span>
        <span>React.js</span>
      </div>
    </div>

    <div class="skill-box">
      <h3>Backend</h3>
      <div class="skills">
        <span>Node.js</span>
        <span>Express.js</span>
        <span>REST APIs</span>
        <span>Authentication</span>
      </div>
    </div>
    <div class="skill-box">
      <h3>Languages</h3>
      <div class="skills">
        <span>JAVA</span>
        <span>Python</span>
        <span>C++</span>
      </div>
    </div>
  </section>

  <!-- Tech Stack Section -->
  <section id="tech" class="section">
    <h2>Tech Stack</h2>
    <div class="stack">
      
      <span>DSA</span>
      <span>MongoDB</span>
      <span>Git & GitHub</span>
      <span>SQL</span>
      <span>API Integration</span>
      <span>Cloud Basics</span>
      <span>Prompt Engineering</span>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section light">
    <h2>Contact Me</h2>
    <p>Email: kushma1523@gmail.com</p>
    <p>Location:Chennai,India</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 Kushma| Web Page Developed using HTML & CSS</p>
  </footer>

</body>
</html>
```

style.css

```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Segoe UI", sans-serif;
}

body {
  background: #126a83;
  color: #ffffff;
  line-height: 1.6;
}

/* Navbar */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 10%;
  background: #364ea1;
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  color: #b8d5e4;
  font-size: 1.6rem;
}

nav a {
  margin-left: 25px;
  text-decoration: none;
  color: #fff;
  font-weight: 500;
  transition: 0.3s;
}

nav a:hover {
  color: #554e79;
}

/* Hero */
.hero {
  height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.hero h2 {
  font-size: 3.2rem;
}

.hero span {
  color: #6798d0;
  
}

.hero p {
  margin-top: 10px;
  font-size: 1.2rem;
  opacity: 0.85;
}

.tagline {
  margin-top: 8px;
  font-size: 1rem;
  opacity: 0.6;
}

.hero-image img {
  border-radius: 20px;
  width: 250px;
  height: 250px;
  object-fit: cover;
}

/* Sections */
.section {
  padding: 80px 10%;
  text-align: center;
}

.section h2 {
  font-size: 2.3rem;
  margin-bottom: 25px;
  color: #6798d0;

}

.section p {
  max-width: 800px;
  margin: auto;
  opacity: 0.85;
}

.light {
  background: #020332;
}

/* Skills */
.skill-box {
  margin-bottom: 40px;
}

.skill-box h3 {
  margin-bottom: 15px;
  color: #fff;
  font-size: 1.3rem;
}

.skills, .stack {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
}

.skills span {
  background: #1f1f1f;
  border: 1px solid #ece3e3;
  color: #fff;
  padding: 10px 18px;
  border-radius: 25px;
  font-size: 0.9rem;
  transition: 0.3s;
}

.skills span:hover {
  background: #447fd1;
  transform: translateY(-3px);
}

/* Tech Stack */
.stack span {
  background: #1f1f1f;
  border: 1px solid #f8f1f1;
  color: #fff;
  padding: 10px 18px;
  border-radius: 25px;
  font-size: 0.9rem;
  transition: 0.3s;
}

.stack span:hover {
  background: #3766a9;
  transform: translateY(-3px);
}

.mern {
  border: 1px solid #ff3c3c !important;
  color: #ff3c3c;
  font-weight: 600;
}

/* Footer */
footer {
  background: #0f0f0f;
  padding: 20px;
  text-align: center;
  font-size: 0.9rem;
  opacity: 0.6;
} join this two code as one html code
```


## OUTPUT
<img width="1600" height="915" alt="web exp1 output1" src="https://github.com/user-attachments/assets/6b67a294-f1e0-4ce7-9c7c-bbc556cc21b9" />

<img width="1600" height="908" alt="web exp1 output2" src="https://github.com/user-attachments/assets/a47d7f74-7af5-41b8-b06b-5d6089ab39cb" />

<img width="1600" height="951" alt="web exp1 output3" src="https://github.com/user-attachments/assets/fa73f1b0-8c5f-4804-a015-d170e466c4a2" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
