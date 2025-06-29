Name:Akhila Mesupamu
Company:SkillCraft-Technology
ID:SCT/JUN25/5142
Domain:Web Development
Duration:June to July 2025
Mentor:skillcraft


Overview Of The Project
Project:Create an interactive navigation menu that changes color or style when scrolled or when hovering over a menu item.
.Objective
To create an interactive navigation menu for a website that enhances user experience by dynamically changing its style when the user:

Scrolls the page

Hovers over the navigation items

.Key Activities
Design the navigation bar layout using HTML and CSS.

Style the navbar to be responsive and visually appealing.

Implement hover effects on menu items using CSS transitions.

Detect scroll events using JavaScript to dynamically update navbar styling.

Test responsiveness on different screen sizes.

.Technologies Used
HTML: Structure of the navigation menu.

CSS: Styling, hover effects, and transitions.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>CoHost Landing Page</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      scroll-behavior: smooth;
    }

    /* Header/Nav */
    header {
      position: sticky;
      top: 0;
      background: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 60px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
      z-index: 1000;
    }

    .logo {
      font-weight: bold;
      font-size: 1.5rem;
      color: #333;
    }

    nav a {
      margin: 0 12px;
      text-decoration: none;
      color: #333;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover {
      color: #6A1B9A;
    }

    .btn-primary {
      background-color: #6A1B9A;
      color: white;
      padding: 10px 18px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 80px 40px;
      min-height: 100vh;
    }

    /* Section Colors */
    #home     { background: #F3E5F5; }
    #about    { background: #E3F2FD; }
    #domain   { background: #FFF3E0; }
    #hosting  { background: #E8F5E9; }
    #blog     { background: #FCE4EC; }
    #contact  { background: #ECEFF1; }
    #getstart { background: #FBE9E7; }

    .section-content {
      max-width: 1100px;
      margin: auto;
    }

    .hero {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 40px;
    }

    .hero-text {
      flex: 1;
      min-width: 280px;
    }

    .hero-text h1 {
      font-size: 2.5rem;
      margin-bottom: 15px;
    }

    .hero-text p {
      margin-bottom: 20px;
      color: #444;
    }

    .hero-image {
      flex: 1;
      text-align: center;
    }

    .hero-image img {
      width: 100%;
      max-width: 400px;
    }

    .domain-search {
      background-color: #6A1B9A;
      padding: 40px;
      color: white;
      border-radius: 10px;
      text-align: center;
    }

    .domain-search input,
    .domain-search select {
      padding: 12px;
      margin: 10px 5px;/
      border: none;
      border-radius: 5px;
      font-size: 1rem;
    }

    .domain-search button {
      padding: 12px 25px;
      background-color: #00C896;
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .prices {
      margin-top: 15px;
      font-size: 0.9rem;
      color: #ccc;
    }

    h2 {
      font-size: 2rem;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column-reverse;
        text-align: center;
      }

      header {
        flex-direction: column;
        gap: 10px;
        padding: 20px;
      }

      nav {
        flex-wrap: wrap;
        justify-content: center;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="logo">CoHost</div>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#domain">Domain</a>
    <a href="#hosting">Hosting</a>
    <a href="#blog">Blog</a>
    <a href="#contact">Contact</a>
    <a class="btn-primary" href="#getstart">Get Started</a>
  </nav>
</header>

<!-- Home Section -->
<section id="home">
  <div class="section-content hero">
    <div class="hero-text">
      <p style="color:#6A1B9A;font-weight:600;">ISOMETRIC HOSTING</p>
      <h1>Design, Development, Hosting</h1>
      <p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.</p>
      <a href="#contact" class="btn-primary">Get in touch</a>
    </div>
    <div class="hero-image">
      <img src="C:\Users\mesup\OneDrive\Documents\Pictures\cohost-1.jpg"alt="cohost-1">
    </div>
  </div>
</section>

<!-- About Section -->
<section id="about">
  <div class="section-content">
    <h2>About Us</h2>
    <p>We are passionate about modern UI, interactive development, and scalable web hosting.</p>
  </div>
</section>

<!-- Domain Section -->
<section id="domain">
  <div class="section-content">
    <div class="domain-search">
      <h2>Search Your Domain Name</h2>
      <p>A small river named Duden flows by their place</p>
      <input type="text" placeholder="Enter your domain name...">
      <select>
        <option>.com</option>
        <option>.net</option>
        <option>.biz</option>
        <option>.co</option>
        <option>.me</option>
      </select>
      <button>Search</button>
      <div class="prices">
        .com $9.75 &nbsp; | &nbsp; .net $9.50 &nbsp; | &nbsp; .biz $8.95 &nbsp; | &nbsp; .co $7.80 &nbsp; | &nbsp; .me $7.95
      </div>
    </div>
  </div>
</section>

<!-- Hosting Section -->
<section id="hosting">
  <div class="section-content">
    <h2>Hosting Plans</h2>
    <p>Choose from our affordable and scalable cloud hosting packages to get your website online fast.</p>
  </div>
</section>

<!-- Blog Section -->
<section id="blog">
  <div class="section-content">
    <h2>Latest Blog Posts</h2>
    <p>Stay updated with our news, product launches, and tutorials on web development.</p>
  </div>
</section>

<!-- Contact Section -->
<section id="contact">
  <div class="section-content">
    <h2>Contact Us</h2>
    <p>Have questions or want to work together? Drop us a message!</p>
  </div>
</section>

<!-- Get Started Section -->
<section id="getstart">
  <div class="section-content">
    <h2>Get Started Today</h2>
    <p>Launch your idea with confidence. Get in touch and let's build something amazing.</p>
  </div>
</section>

</body>
</html>

JavaScript: Scroll detection and dynamic class toggling.

(Optional: Bootstrap or Tailwind CSS for faster development)


