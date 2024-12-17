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
/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  background-color: #f4f4f4;
}

header {
  background: #333;
  color: #fff;
  padding: 10px 0;
}

nav ul {
  list-style-type: none;
  text-align: center;
}

nav ul li {
  display: inline;
  margin: 0 20px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.hero {
  background-color: #4CAF50;
  color: white;
  padding: 100px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 3em;
}

.hero p {
  font-size: 1.2em;
  margin: 20px 0;
}

button {
  padding: 10px 20px;
  background-color: #fff;
  color: #4CAF50;
  border: none;
  cursor: pointer;
  font-size: 1em;
}

button:hover {
  background-color: #ddd;
}

section {
  padding: 40px 20px;
  text-align: center;
}

section h2 {
  font-size: 2em;
  margin-bottom: 20px;
}

ul {
  list-style-type: none;
}

ul li {
  font-size: 1.2em;
  margin: 10px 0;
}

footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 10px;
  position: fixed;
  width: 100%;
  bottom: 0;
}

form {
  max-width: 500px;
  margin: 0 auto;
}

form label {
  display: block;
  margin: 10px 0;
}

form input {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  border: 1px solid #ccc;
}

form button {
  background-color: #4CAF50;
  color: white;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
}

form button:hover {
  background-color: #45a049;
}
// Function to display a message when the button is clicked
function showMessage() {
  alert("Welcome to our website! We are glad to have you here.");
}

// Example of form submission handling
document.getElementById("contact-form").addEventListener("submit", function(event) {
  event.preventDefault(); // Prevent form from actually submitting
  
  const name = document.getElementById("name").value;
  const email = document.getElementById("email").value;
  
  alert(`Thank you, ${name}! We will reach out to you at ${email}.`);
});

