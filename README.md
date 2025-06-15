<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Amazon Clone</title>
  <style>
    * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  color: white;
  background: url('amazonbg.jpg') no-repeat center center fixed;
  background-size: cover;
  backdrop-filter: opacity(4.9);
  
}

/* 🔥 Header */
.header {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  background: #131921;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
  animation: logoFade 2s ease-in-out infinite alternate;
}
.logo span {
  color: orange;
}

.nav-links {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
}

.nav-links a {
  color: white;
  text-decoration: none;
  padding: 5px 10px;
  border-radius: 5px;
  transition: 0.3s;
}
.nav-links a:hover {
  background: orange;
  color: #111;
}

.search-bar input {
  padding: 8px 12px;
  border-radius: 50px;
  border: none;
  outline: none;
  width: 160px;
  transition: 0.3s;
}
.search-bar input:focus {
  width: 200px;
}

/* 🔥 Hero */
.hero-banner {
  height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.hero-content {
  background: rgba(0, 0, 0, 0.65);
  padding: 30px;
  border-radius: 12px;
  animation: fadeUp 1.5s ease-in-out;
}

.hero-btn {
  display: inline-block;
  margin-top: 15px;
  padding: 12px 25px;
  background: orange;
  color: #111;
  text-decoration: none;
  border-radius: 5px;
  transition: 0.3s;
}
.hero-btn:hover {
  background: #f90;
}

/* 🔥 Products */
.products {
  padding: 40px 60px;
  text-align: center;
}

.products h2 {
  font-size: 2rem;
  margin-bottom: 30px;
}

.product-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 25px;
  justify-content: center;
}

.product-card {
  background: white;
  color: black;
  padding: 20px;
  border-radius: 8px;
  width: 220px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  transition: 0.3s;
}
.product-card:hover {
  transform: translateY(-10px);
}

.product-card img {
  width: 100%;
  height: 180px;
  object-fit: contain;
}

.product-card h3 {
  margin: 10px 0;
}

.product-card p {
  color: green;
  font-weight: bold;
}
.contact-section {
  background: linear-gradient(to right, #0f0f0f, #1a1a1a);
  padding: 60px 20px;
  text-align: center;
  color: #fff;
  animation: fadeInUp 1.5s ease;
}

.contact-container {
  max-width: 600px;
  margin: auto;
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(8px);
  padding: 40px;
  border-radius: 15px;
  box-shadow: 0 0 15px rgba(255, 255, 255, 0.1);
}

.contact-section h2 {
  font-size: 2.5rem;
  margin-bottom: 30px;
  color: #f0c14b;
}

.contact-container input,
.contact-container textarea {
  width: 100%;
  padding: 15px;
  margin-bottom: 15px;
  border: none;
  border-radius: 8px;
  font-size: 1rem;
  background: #f5f5f5;
  color: #111;
}

.contact-container button {
  background: #f0c14b;
  color: #111;
  border: none;
  padding: 12px 20px;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
}

.contact-container button:hover {
  background: #ddb347;
  transform: scale(1.05);
}

/* Optional animation */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}


.btn {
  display: inline-block;
  margin-top: 10px;
  padding: 8px 12px;
  background: #f0c14b;
  color: #111;
  border-radius: 5px;
  text-decoration: none;
}
.btn:hover {
  background: #ddb347;
}

/* 🔥 Footer */
footer {
  background: #232f3e;
  padding: 20px;
  text-align: center;
  color: white;
}

/* 🔥 Animations */
@keyframes fadeUp {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes logoFade {
  from {
    color: orange;
  }
  to {
    color: white;
  }
}

/* 🔥 Responsive */
@media (max-width: 768px) {
  .nav-links {
    justify-content: center;
    width: 100%;
    margin-top: 10px;
  }

  .search-bar input {
    width: 100%;
    margin-top: 10px;
  }


  .products {
    padding: 20px;
  }
}

  </style>
</head>
<body>

  <!-- 🔥 Creative & Responsive Header -->
  <header class="header">
    <div class="logo">amazon<span>.in</span></div>
    <nav class="nav-links">
      <a href="#">Home</a>
      <a href="#">Deals</a>
      <a href="#">Electronics</a>
      <a href="#">Fashion</a>
      <a href="#">Cart</a>
    </nav>
    <div class="search-bar">
      <input type="text" placeholder="Search Amazon.in"/>
    </div>
  </header>

  <!-- 🔥 Hero Section -->
  <section class="hero-banner">
    <div class="hero-content">
      <h1>Great Deals on Electronics</h1>
      <p>Explore top offers with free delivery</p>
      <a href="#" class="hero-btn">Shop Now</a>
    </div>
  </section>

  <!-- 🔥 Products -->
  <section class="products">
    <h2>Featured Products</h2>
    <div class="product-grid">
      <div class="product-card">
        <img src="https://m.media-amazon.com/images/I/81fPKd-2AYL._AC_UL480_FMwebp_QL65_.jpg" alt="Product"/>
        <h3>Wireless Headphones</h3>
        <p>₹2,499</p>
        <a href="#" class="btn">Add to Cart</a>
      </div>
      <div class="product-card">
        <img src="download.webp" alt="Product"/>
        <h3>Bluetooth Speaker</h3>
        <p>₹1,799</p>
        <a href="#" class="btn">Add to Cart</a>
      </div>
      <div class="product-card">
        <img src="download1.webp" alt="Product"/>
        <h3>Smart Watch</h3>
        <p>₹3,299</p>
        <a href="#" class="btn">Add to Cart</a>
      </div>
    </div>
  </section>
  <section class="contact-section" id="contact">
  <div class="contact-container">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </div>
</section>


  <!-- 🔥 Footer -->
  <footer>
    <p>© 2025 Amazon Clone. Built for practice.</p>
  </footer>

</body>
</html>
