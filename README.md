[index.html](https://github.com/user-attachments/files/28168096/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>HDPRO - Creative Studio</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #000;
      color: #fff;
      overflow-x: hidden;
    }

    /* Header */
    header {
      background: rgba(44, 44, 44, 0.95);
      color: white;
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    nav a {
      color: #ffffff;
      margin-left: 20px;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ffd700;
    }

    .logo {
      animation: flicker 2s infinite alternate;
    }

    .brand-name {
      font-size: 36px;
      font-weight: bold;
      color: #ffffff;
      letter-spacing: 2px;
      text-shadow: 0 0 10px #d89216, 0 0 20px #d89216;
    }

    .brand-name .accent {
      color: #ffd700;
    }

    .slogan {
      font-size: 14px;
      font-style: italic;
      color: #cccccc;
    }

    /* Hero section with video background */
    .hero {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
    }

    .hero video {
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: 0;
    }

    .hero::before {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0,0,0,0.5);
      z-index: 1;
    }

    .hero-content {
      position: relative;
      z-index: 2;
    }

    .hero-content h1 {
      font-size: 60px;
      margin: 0;
      animation: fadeInDown 1.5s ease;
    }

    .hero-content p {
      font-size: 20px;
      margin-top: 15px;
      animation: fadeInUp 2s ease;
    }

    .hero-content button {
      margin-top: 25px;
      padding: 12px 30px;
      font-size: 16px;
      background: transparent;
      border: 2px solid #ffd700;
      color: #ffd700;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s, color 0.3s;
    }

    .hero-content button:hover {
      background: #ffd700;
      color: #1f1f1f;
    }

    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-50px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(50px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes flicker {
      from {
        text-shadow: 0 0 5px #d89216, 0 0 10px #d89216, 0 0 15px #ff6600;
      }
      to {
        text-shadow: 0 0 20px #d89216, 0 0 30px #ff6600, 0 0 40px #ff3300;
      }
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #2c2c2c;
      color: #f4f0ec;
      font-size: 14px;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">
      <div class="brand-name">HD<span class="accent">PRO</span></div>
      <div class="slogan">Where Creativity Meets Professionalism</div>
    </div>
    <nav>
      <a href="index.html">Home</a>
      <a href="product.html">Products</a>
      <a href="cart.html">Cart</a>
      <a href="ads.html">Advertise</a>
      <a href="admin.html">Admin</a>
    </nav>
  </header>

  <section class="hero">
    <video autoplay muted loop>
      <source src="Wave.mp4" type="video/mp4">
    </video>
    <div class="hero-content">
      <h1>Welcome to HDPRO</h1>
      <p>Inspiration. Innovation. Identity.</p>
      <button onclick="location.href='product.html'">Explore Our Collection</button>
    </div>
  </section>

  <footer>
    &copy; 2025 HDPRO. All rights reserved.
  </footer>

</body>
</html>
