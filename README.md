<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="My personal web development portfolio">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="site-header">
    <nav class="navbar" aria-label="Main navigation">
      <a class="logo" href="#home">My Portfolio</a>
      <div class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="hero-content">
        <p class="eyebrow">WELCOME TO MY WEBSITE</p>
        <h1>Hello, I'm a Web Developer.</h1>
        <p>
          I'm learning to create clean, accessible, and
          responsive websites using HTML and CSS.
        </p>
        <a class="button" href="#about">Learn More</a>
      </div>
    </section>

    <section class="section" id="about">
      <h2>About Me</h2>
      <p>
        I enjoy learning new skills and building websites.
        This project demonstrates my understanding of modern
        CSS, page layouts, typography, and responsive design.
      </p>
    </section>

    <section class="section skills-section" id="skills">
      <h2>My Skills</h2>
      <div class="cards">
        <article class="card">
          <h3>HTML</h3>
          <p>Creating meaningful webpage structure.</p>
        </article>
        <article class="card">
          <h3>CSS</h3>
          <p>Styling content with color, spacing, and typography.</p>
        </article>
        <article class="card">
          <h3>Responsive Design</h3>
          <p>Making websites work on phones and computers.</p>
        </article>
      </div>
    </section>

    <section class="section contact-section" id="contact">
      <h2>Contact</h2>
      <p>Thank you for visiting my portfolio!</p>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 My Portfolio | Built with HTML and CSS</p>
  </footer>
</body>
</html>
css

/* General styles and box model */
* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.6;
  color: #263746;
  background-color: #ffffff;
}

a {
  color: inherit;
  text-decoration: none;
}

/* Navigation using Flexbox */
.site-header {
  background-color: #142b3d;
  color: #ffffff;
}

.navbar {
  max-width: 1100px;
  margin: 0 auto;
  padding: 20px 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}

.logo {
  font-size: 1.3rem;
  font-weight: bold;
}

.nav-links {
  display: flex;
  gap: 22px;
}

.nav-links a:hover {
  color: #61d6b5;
}

/* Hero section */
.hero {
  background: linear-gradient(135deg, #142b3d, #28566a);
  color: #ffffff;
  padding: 100px 24px;
  text-align: center;
}

.hero-content {
  max-width: 750px;
  margin: 0 auto;
}

.eyebrow {
  color: #61d6b5;
  font-weight: bold;
  letter-spacing: 2px;
  font-size: 0.85rem;
}

h1 {
  font-size: clamp(2rem, 5vw, 3.5rem);
  line-height: 1.15;
  margin: 18px 0;
}

.hero p {
  font-size: 1.1rem;
}

.button {
  display: inline-block;
  background-color: #61d6b5;
  color: #142b3d;
  padding: 12px 24px;
  margin-top: 18px;
  border-radius: 6px;
  font-weight: bold;
}

.button:hover {
  background-color: #ffffff;
}

/* Main content and spacing */
.section {
  max-width: 1100px;
  margin: 0 auto;
  padding: 60px 24px;
}

.section h2 {
  color: #142b3d;
  font-size: 2rem;
  margin-top: 0;
}

.skills-section {
  max-width: none;
  background-color: #f1f6f8;
  text-align: center;
}

.skills-section h2 {
  margin-bottom: 28px;
}

/* Flexbox cards */
.cards {
  max-width: 1052px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  gap: 24px;
}

.card {
  background-color: #ffffff;
  padding: 26px;
  border-radius: 10px;
  flex: 1;
  text-align: left;
  box-shadow: 0 4px 16px rgba(20, 43, 61, 0.08);
}

.card h3 {
  color: #267d70;
}

.contact-section {
  text-align: center;
}

/* Footer */
footer {
  background-color: #142b3d;
  color: #ffffff;
  text-align: center;
  padding: 22px;
}

/* Keyboard accessibility */
a:focus-visible {
  outline: 3px solid #e49b46;
  outline-offset: 4px;
}

/* Responsive layout for smaller screens */
@media (max-width: 650px) {
  .navbar {
    flex-direction: column;
    gap: 14px;
  }

  .nav-links {
    flex-wrap: wrap;
    justify-content: center;
    gap: 12px 18px;
  }

  .hero {
    padding: 70px 20px;
  }

  .cards {
    flex-direction: column;
  }

  .card {
    width: 100%;
  }

  .section {
    padding: 42px 20px;
  }
}
