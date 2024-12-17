<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Home Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Welcome to Our Website</h1>
      <p>Your journey to success begins here.</p>
      <button onclick="showMessage()">Click Me</button>
    </div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>We are a creative agency that helps businesses grow.</p>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <ul>
      <li>Web Design</li>
      <li>SEO Services</li>
      <li>Digital Marketing</li>
      <li>Consulting</li>
    </ul>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form id="contact-form">
      <label for="name">Your Name:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">Your Email:</label>
      <input type="email" id="email" name="email" required>

      <button type="submit">Submit</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2024 Simple Website. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
