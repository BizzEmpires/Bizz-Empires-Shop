<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bizz Empires Fashion</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  /* Reset & base */
  * {margin:0; padding:0; box-sizing:border-box;}
  body {font-family:'Montserrat', sans-serif; background:#fff; color:#333; line-height:1.6;}

  /* Header */
  header {display:flex; justify-content:space-between; align-items:center; padding:20px 5%; background:#000; color:#FFD700; position:sticky; top:0; z-index:100;}
  header img {height:50px;}
  nav a {margin-left:20px; color:#FFD700; font-weight:600;}
  nav a:hover {color:#fff;}

  /* Hero */
  .hero {position:relative; text-align:center; color:#fff;}
  .hero img {width:100%; height:500px; object-fit:cover;}
  .hero-text {position:absolute; top:50%; left:50%; transform:translate(-50%, -50%);}
  .hero-text h1 {font-size:48px; margin-bottom:20px; text-shadow:2px 2px 8px rgba(0,0,0,0.7);}
  .hero-text a {background:#FFD700; color:#000; padding:15px 30px; font-weight:700; border-radius:5px; transition:0.3s;}
  .hero-text a:hover {background:#e6c200;}

  /* Categories */
  .categories {padding:50px 5%;}
  .categories h2 {text-align:center; margin-bottom:40px; font-size:36px;}
  .category-grid {display:grid; grid-template-columns:repeat(auto-fit, minmax(250px, 1fr)); gap:25px;}
  .category {position:relative; overflow:hidden; border-radius:15px; cursor:pointer; transition:0.3s;}
  .category img {width:100%; height:300px; object-fit:cover; transition:transform 0.5s;}
  .category:hover img {transform:scale(1.1);}
  .category span {position:absolute; bottom:10px; left:50%; transform:translateX(-50%); background:rgba(0,0,0,0.6); color:#FFD700; padding:10px 20px; border-radius:5px; font-weight:600;}

  /* Product slider */
  .slider {padding:50px 5%; background:#f5f5f5;}
  .slider h2 {text-align:center; margin-bottom:40px; font-size:36px;}
  .slider-container {display:flex; overflow-x:auto; gap:20px; scroll-behavior:smooth; padding-bottom:10px;}
  .slider-container::-webkit-scrollbar {display:none;}
  .product {min-width:250px; background:#fff; border-radius:15px; overflow:hidden; text-align:center; padding-bottom:20px; box-shadow:0 4px 15px rgba(0,0,0,0.1); transition:transform 0.3s;}
  .product:hover {transform:translateY(-5px);}
  .product img {width:100%; height:300px; object-fit:cover;}
  .product h3 {margin:15px 0 10px;}
  .product p {font-weight:700; color:#000;}

  /* About */
  .about {padding:50px 5%;}
  .about h2 {text-align:center; margin-bottom:30px; font-size:36px;}
  .about p {max-width:800px; margin:0 auto; text-align:center; font-size:18px; line-height:1.7;}

  /* Instagram Gallery */
  .gallery {padding:50px 5%;}
  .gallery h2 {text-align:center; margin-bottom:40px; font-size:36px;}
  .gallery-grid {display:grid; grid-template-columns:repeat(auto-fit, minmax(150px, 1fr)); gap:10px;}
  .gallery-grid img {width:100%; height:150px; object-fit:cover; border-radius:10px; transition:transform 0.3s;}
  .gallery-grid img:hover {transform:scale(1.1);}

  /* Footer */
  footer {background:#000; color:#FFD700; padding:30px 5%; text-align:center;}
  footer a {color:#FFD700; margin:0 10px;}
  footer a:hover {color:#fff;}

  /* Responsive */
  @media(max-width:768px){
    .hero-text h1 {font-size:36px;}
    .slider-container {flex-wrap:nowrap;}
  }
</style>
</head>
<body>

  <!-- Header -->
  <header>
    <img src="images/logo.png" alt="Bizz Empires Logo">
    <nav>
      <a href="#">Home</a>
      <a href="#">Shop</a>
      <a href="#">New Arrivals</a>
      <a href="#">Categories</a>
      <a href="#">About Us</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero">
    <img src="images/hero-banner.jpg" alt="Fashion Hero">
    <div class="hero-text">
      <h1>Premium Fashion for Every Woman</h1>
      <a href="#">Shop Now</a>
    </div>
  </section>

  <!-- Categories -->
  <section class="categories">
    <h2>Shop by Category</h2>
    <div class="category-grid">
      <div class="category"><img src="images/dresses.jpg" alt=""><span>Dresses</span></div>
      <div class="category"><img src="images/tops.jpg" alt=""><span>Tops & Blouses</span></div>
      <div class="category"><img src="images/skirts.jpg" alt=""><span>Skirts & Pants</span></div>
      <div class="category"><img src="images/outerwear.jpg" alt=""><span>Outerwear</span></div>
      <div class="category"><img src="images/shoes.jpg" alt=""><span>Shoes</span></div>
      <div class="category"><img src="images/accessories.jpg" alt=""><span>Accessories</span></div>
    </div>
  </section>

  <!-- Featured Products Slider -->
  <section class="slider">
    <h2>Featured Products</h2>
    <div class="slider-container">
      <div class="product">
        <img src="images/product1.jpg" alt="">
        <h3>Evening Gown</h3>
        <p>$49.99</p>
      </div>
      <div class="product">
        <img src="images/product2.jpg" alt="">
        <h3>Summer Dress</h3>
        <p>$39.99</p>
      </div>
      <div class="product">
        <img src="images/product3.jpg" alt="">
        <h3>Casual Top</h3>
        <p>$19.99</p>
      </div>
      <div class="product">
        <img src="images/product4.jpg" alt="">
        <h3>Palazzo Pants</h3>
        <p>$29.99</p>
      </div>
      <div class="product">
        <img src="images/product5.jpg" alt="">
        <h3>Blazer Jacket</h3>
        <p>$59.99</p>
      </div>
    </div>
  </section>

  <!-- About -->
  <section class="about">
    <h2>About Bizz Empires Fashion</h2>
    <p>Located in Kapenguria, West Pokot, Bizz Empires Fashion brings you the latest international ladies’ fashion trends. We offer premium quality clothes, shoes, and accessories for every woman. Our mission is to provide stylish, comfortable, and affordable fashion for all occasions.</p>
  </section>

  <!-- Instagram Gallery -->
  <section class="gallery">
    <h2>Follow Us</h2>
    <div class="gallery-grid">
      <img src="images/gallery1.jpg" alt="">
      <img src="images/gallery2.jpg" alt="">
      <img src="images/gallery3.jpg" alt="">
      <img src="images/gallery4.jpg" alt="">
      <img src="images/gallery5.jpg" alt="">
      <img src="images/gallery6.jpg" alt="">
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 Bizz Empires Fashion | Kapenguria, West Pokot</p>
    <p>
      <a href="#">Facebook</a> | 
      <a href="#">Instagram</a> | 
      <a href="#">WhatsApp</a>
    </p>
  </footer>

</body>
</html>
