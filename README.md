<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Responsive Interactive Web Page</title>
  <style>
    /* Reset some default styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      background-color: #f9f9f9;
    }

    header {
      background-color: #333;
      color: #fff;
      padding: 1rem 0;
    }

    nav {
      max-width: 1200px;
      margin: auto;
      padding: 0 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    nav h1 {
      font-size: 1.5rem;
    }

    .nav-links {
      display: flex;
      gap: 1.5rem;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    .nav-links a:hover {
      color: #00bcd4;
    }

    .hero {
      background: linear-gradient(to right, #00bcd4, #2196f3);
      color: white;
      text-align: center;
      padding: 4rem 2rem;
    }

    .hero h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
    }

    .hero button {
      background-color: white;
      color: #2196f3;
      border: none;
      padding: 0.75rem 1.5rem;
      font-size: 1rem;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease, transform 0.2s ease;
    }

    .hero button:hover {
      background-color: #f1f1f1;
      transform: scale(1.05);
    }

    .cards {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 2rem;
      padding: 3rem 2rem;
      max-width: 1200px;
      margin: auto;
    }

    .card {
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      padding: 2rem;
      flex: 1 1 300px;
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card h3 {
      margin-bottom: 1rem;
      color: #333;
    }

    .card p {
      color: #666;
    }

    footer {
      text-align: center;
      padding: 2rem;
      background-color: #333;
      color: white;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      nav {
        flex-direction: column;
        align-items: flex-start;
      }

      .hero h2 {
        font-size: 2rem;
      }

      .hero p {
        font-size: 1rem;
      }
    }

  </style>
</head>
<body>

  <header>
    <nav>
      <h1>My Website</h1>
      <div class="nav-links">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Services</a>
        <a href="#">Contact</a>
      </div>
    </nav>
  </header>

  <section class="hero">
    <h2>Welcome to My Responsive Web Page</h2>
    <p>This page is built using only HTML and CSS</p>
    <button>Learn More</button>
  </section>

  <section class="cards">
    <div class="card">
      <h3>Responsive Design</h3>
      <p>This layout adapts to different screen sizes using media queries.</p>
    </div>
    <div class="card">
      <h3>Interactive Elements</h3>
      <p>Hover over cards and buttons to see interactive animations.</p>
    </div>
    <div class="card">
      <h3>Pure HTML & CSS</h3>
      <p>No JavaScript needed to build this modern responsive layout.</p>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 My Website. All rights reserved.</p>
  </footer>

</body>
</html>
