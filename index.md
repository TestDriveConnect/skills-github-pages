<!DOCTYPE html> 
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TestDrive Connect</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #000000;
      --secondary: #ffffff;
      --accent: #f4d35e;
      --grey: #f5f5f5;
      --text-dark: #333333;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--secondary);
      color: var(--text-dark);
      line-height: 1.6;
    }

    html {
      scroll-behavior: smooth;
    }

    .navbar {
      background-color: var(--secondary);
      border-bottom: 1px solid #ddd;
      position: sticky;
      top: 0;
      width: 100%;
      z-index: 1000;
    }

    .nav-container {
      max-width: 1200px;
      margin: auto;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .nav-logo img {
      height: 60px;
    }

    .nav-menu {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    .nav-menu li a {
      color: #000;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s ease;
    }

    .nav-menu li a:hover {
      color: var(--accent);
    }

    .hamburger {
      display: none;
      flex-direction: column;
      cursor: pointer;
    }

    .bar {
      height: 3px;
      width: 25px;
      background-color: #000;
      margin: 4px 0;
      transition: 0.4s;
    }

    @media (max-width: 768px) {
      .nav-menu {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 60px;
        right: 20px;
        background-color: var(--secondary);
        width: 200px;
        padding: 15px;
        border: 1px solid #ddd;
        border-radius: 6px;
      }

      .nav-menu.active {
        display: flex;
      }

      .hamburger {
        display: flex;
      }
    }

    header {
      background-color: var(--primary);
      color: var(--secondary);
      text-align: center;
      padding: 60px 20px;
    }

    header h1 {
      font-size: 3rem;
      font-weight: 700;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.25rem;
      margin-bottom: 20px;
    }

    .cta-btn {
      background-color: var(--accent);
      color: var(--primary);
      text-decoration: none;
      font-weight: 600;
      padding: 12px 30px;
      border-radius: 6px;
      margin: 10px 10px;
      display: inline-block;
      transition: background 0.3s;
    }

    .cta-btn:hover {
      background-color: #e6c64a;
    }

    section {
      padding: 60px 20px;
      text-align: center;
    }

    section h2 {
      font-size: 2rem;
      margin-bottom: 20px;
    }

    .features {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 30px;
    }

    .feature-box {
      background-color: var(--grey);
      padding: 20px;
      border-radius: 8px;
      width: 260px;
      text-align: center;
    }

    .form {
      margin-top: 20px;
    }

    .form input, .form select, .form textarea {
      padding: 12px;
      width: 90%;
      max-width: 400px;
      border: 1px solid #ccc;
      border-radius: 6px;
      margin: 8px 0;
      font-size: 1rem;
    }

    .form textarea {
      resize: vertical;
    }

    .form input[type="submit"] {
      background-color: var(--primary);
      color: var(--secondary);
      border: none;
      padding: 12px 20px;
      border-radius: 6px;
      cursor: pointer;
      font-weight: 600;
    }

    .form input[type="submit"]:hover {
      background-color: #333333;
    }

    footer {
      background-color: var(--primary);
      color: var(--secondary);
      text-align: center;
      padding: 20px;
    }

    footer a {
      color: var(--accent);
      text-decoration: none;
    }
  </style>
</head>

<body>

  <nav class="navbar">
    <div class="nav-container">
      <a href="index.html" class="nav-logo">
        <img src="TestDriveConnectLogo.png" alt="TestDrive Connect Logo">
      </a>
      <ul class="nav-menu" id="navMenu">
        <li><a href="#how-it-works">How It Works</a></li>
        <li><a href="#for-dealerships">For Dealerships</a></li>
        <li><a href="#for-drivers">For Drivers</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="hamburger" id="hamburger">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
    </div>
  </nav>

  <header>
    <h1>TestDrive Connect</h1>
    <p>Your trusted eyes behind the wheel.</p>
    <a href="#contact" class="cta-btn">Request a Test Drive</a>
    <a href="#contact" class="cta-btn">Become a Test Driver</a>
  </header>

    <section id="how-it-works">
    <h2>How It Works</h2>
    <div class="features">
      <div class="feature-box">
        <h3>1. Submit Your Request</h3>
        <p>Tell us the car, the dealership, and what you want checked.</p>
      </div>
      <div class="feature-box">
        <h3>2. Local Driver Test Drives</h3>
        <p>Our vetted driver inspects, drives, and films the car for you.</p>
      </div>
      <div class="feature-box">
        <h3>3. Get a Full Report</h3>
        <p>Receive a video, photos, checklist, and driver notes.</p>
      </div>
      <div class="feature-box">
        <h3>4. Buy with Confidence</h3>
        <p>Decide with peace of mind, knowing the car inside out.</p>
      </div>
    </div>
  </section>

  <section id="for-dealerships">
    <h2>For Dealerships</h2>
    <p>Offer TestDrive Connect to your customers and unlock sales from out-of-town buyers. Build trust, reduce returns, and close more deals.</p>
  </section>

  <section id="for-drivers">
    <h2>For Drivers</h2>
    <p>Get paid to test drive cars in your area. Flexible gigs for car enthusiasts, students, retirees, and mechanics alike.</p>
  </section>

  <section id="contact">
    <h2>Request a Test Drive</h2>
    <p>Fill out the form below to get started!</p>
    <form action="https://formspree.io/f/your-form-id" method="POST" class="form">
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="email" name="email" placeholder="Your Email" required>
      <input type="tel" name="phone" placeholder="Your Phone Number (optional)">
      <select name="service" required>
        <option value="">Select a Service</option>
        <option value="test-drive">Request a Test Drive</option>
        <option value="driver-signup">Become a Test Driver</option>
      </select>
      <textarea name="message" rows="4" placeholder="Tell us about the car, dealership, and what you'd like checked." required></textarea>

      <label style="font-size: 0.9rem; display: block; margin: 10px 0;">
        <input type="checkbox" required>
        I acknowledge that TestDrive Connect provides a preliminary test drive service by a third-party driver and is not a professional inspection. I understand that purchasing decisions are solely my responsibility, and I agree to release TestDrive Connect and the dealership from any liability or dissatisfaction after purchase.
      </label>

      <input type="submit" value="Submit">
    </form>
  </section>

  <footer>
    <p>&copy; 2025 TestDrive Connect. All rights reserved.</p>
    <p><a href="terms.html">Terms & Conditions</a> | Contact us at <a href="mailto:info@testdriveconnect.com">info@testdriveconnect.com</a></p>
  </footer>

  <script>
    const hamburger = document.getElementById('hamburger');
    const navMenu = document.getElementById('navMenu');
    hamburger.addEventListener('click', () => {
      navMenu.classList.toggle('active');
    });
  </script>

</body>
</html>
