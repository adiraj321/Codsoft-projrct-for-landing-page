<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CodSoft Task 1 - Advanced Landing Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }
    body {
      background-color: #f0f4f8;
      color: #333;
      line-height: 1.6;
    }
    header {
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      padding: 30px 20px;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }
    header h1 {
      font-size: 2.8rem;
      margin-bottom: 10px;
      animation: fadeDown 1s ease-in-out;
    }
    @keyframes fadeDown {
      from { transform: translateY(-20px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
      margin-top: 10px;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 600;
      position: relative;
    }
    nav a::after {
      content: '';
      position: absolute;
      width: 0%;
      height: 2px;
      left: 0;
      bottom: -5px;
      background-color: #ffcc00;
      transition: 0.4s;
    }
    nav a:hover::after {
      width: 100%;
    }
    .hero {
      background: url('https://source.unsplash.com/1600x800/?technology,web') no-repeat center center/cover;
      height: 500px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      position: relative;
      overflow: hidden;
    }
    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0, 0, 0, 0.5);
    }
    .hero h1 {
      font-size: 4rem;
      z-index: 1;
      animation: fadeIn 2s ease-in;
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: scale(1.2); }
      100% { opacity: 1; transform: scale(1); }
    }
    .section {
      padding: 80px 20px;
      max-width: 1100px;
      margin: auto;
    }
    .section h2 {
      text-align: center;
      font-size: 2.5rem;
      color: #2c5364;
      margin-bottom: 30px;
      position: relative;
    }
    .section h2::after {
      content: '';
      display: block;
      width: 60px;
      height: 4px;
      background: #2c5364;
      margin: 10px auto 0;
    }
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }
    .feature {
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
      text-align: center;
    }
    .feature:hover {
      transform: translateY(-10px);
    }
    .feature h3 {
      color: #203a43;
      margin-bottom: 10px;
    }
    .feature p {
      color: #666;
    }
    .section p.centered {
      text-align: center;
      font-size: 1.1rem;
      color: #444;
      max-width: 750px;
      margin: auto;
    }
    .logo {
      width: 60px;
      height: auto;
      margin-bottom: 10px;
    }
    footer {
      background: #0f2027;
      color: white;
      text-align: center;
      padding: 25px;
      margin-top: 50px;
      font-size: 0.95rem;
    }
    @media (max-width: 600px) {
      .hero h1 {
        font-size: 2rem;
        padding: 0 10px;
        text-align: center;
      }
      nav {
        flex-direction: column;
        gap: 15px;
      }
    }
  </style>
</head>
<body>
  <header>
    <img src="https://img.icons8.com/ios-filled/50/ffffff/source-code.png" class="logo" alt="CodSoft Logo">
    <h1>CodSoft Landing Page</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#features">Features</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero" id="home">
    <h1>Your Future in Tech Starts Here</h1>
  </section>

  <section class="section" id="features">
    <h2>Advanced Features</h2>
    <div class="features">
      <div class="feature">
        <h3>Responsive Design</h3>
        <p>Works seamlessly on all devices with dynamic resizing and adaptive layouts.</p>
      </div>
      <div class="feature">
        <h3>Elegant UI</h3>
        <p>Professional interface with intuitive design and modern visual elements.</p>
      </div>
      <div class="feature">
        <h3>Quick Customization</h3>
        <p>Built for flexibility and easy editing to match your brand’s identity.</p>
      </div>
      <div class="feature">
        <h3>Interactive Elements</h3>
        <p>Engaging animations and hover effects to enhance user interaction.</p>
      </div>
    </div>
  </section>

  <section class="section" id="about">
    <h2>About Us</h2>
    <p class="centered">
      CodSoft is a creative tech company passionate about web development and innovation. We build scalable and beautiful digital products tailored for businesses and individuals. Our mission is to shape the future through technology.
    </p>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p class="centered">
      📧 <strong>support@codsoft.com</strong><br />
      🌐 Follow us on social media to explore our portfolio and connect with our team.
    </p>
  </section>

  <footer>
    <p>&copy; 2025 CodSoft. Designed with passion and precision.</p>
  </footer>
</body>
</html>
