<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>E-Shop</title>
 <link href="style.css" rel="stylesheet">
</head>
<body>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, sans-serif;
    }

    body{
      background:#f5f5f5;
    }

    /* Navbar */
    .navbar{
      background:#222;
      color:white;
      padding:15px 40px;
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    .navbar h1{
      color:#00bcd4;
    }

    .nav-links a{
      color:white;
      text-decoration:none;
      margin-left:20px;
      font-size:18px;
    }

    /* Hero Section */
    .hero{
      background:linear-gradient(to right,#00bcd4,#2196f3);
      color:white;
      text-align:center;
      padding:60px 20px;
    }

    .hero h2{
      font-size:40px;
      margin-bottom:10px;
    }

    /* Products */
    .products{
      padding:40px;
    }

    .products h2{
      text-align:center;
      margin-bottom:30px;
    }

    .product-container{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:20px;
    }

    .card{
      background:white;
      border-radius:10px;
      padding:15px;
      text-align:center;
      box-shadow:0 2px 10px rgba(0,0,0,0.1);
      transition:0.3s;
    }

    .card:hover{
      transform:translateY(-5px);
    }

    .card img{
      width:100%;
      height:220px;
      object-fit:cover;
      border-radius:10px;
    }

    .card h3{
      margin:15px 0 10px;
    }

    .price{
      color:green;
      font-size:20px;
      margin-bottom:10px;
    }

    .btn{
      background:#2196f3;
      color:white;
      border:none;
      padding:10px 20px;
      border-radius:5px;
      cursor:pointer;
      font-size:16px;
    }

    .btn:hover{
      background:#0b7dda;
    }

    /* Footer */
    footer{
      background:#222;
      color:white;
      text-align:center;
      padding:15px;
      margin-top:40px;
    }

  </style>
</head>
<body>

  <!-- Navbar -->
  <div class="navbar">
    <h1>E-Shop</h1>

    <div class="nav-links">
      <a href="#">Home</a>
      <a href="#">Products</a>
      <a href="#">Cart</a>
      <a href="#">Contact</a>
    </div>
  </div>

  <!-- Hero -->
  <section class="hero">
    <h2>Welcome to E-Shop</h2>
    <p>Best Online Shopping Website</p>
  </section>

  <!-- Products -->
  <section class="products">
    <h2>Latest Products</h2>

    <div class="product-container">

      <!-- Product 1 -->
      <div class="card">
        <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30" alt="">
        <h3>Smart Watch</h3>
        <p class="price">₹1999</p>
        <button class="btn" onclick="addToCart('Smart Watch')">
          Add to Cart
        </button>
      </div>

      <!-- Product 2 -->
      <div class="card">
        <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e" alt="">
        <h3>Headphones</h3>
        <p class="price">₹1499</p>
        <button class="btn" onclick="addToCart('Headphones')">
          Add to Cart
        </button>
      </div>

      <!-- Product 3 -->
      <div class="card">
        <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9" alt="">
        <h3>Mobile Phone</h3>
        <p class="price">₹12999</p>
        <button class="btn" onclick="addToCart('Mobile Phone')">
          Add to Cart
        </button>
      </div>

      <!-- Product 4 -->
      <div class="card">
        <img src="https://images.unsplash.com/photo-1580910051074-3eb694886505" alt="">
        <h3>Laptop</h3>
        <p class="price">₹45999</p>
        <button class="btn" onclick="addToCart('Laptop')">
          Add to Cart
        </button>
      </div>

    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 E-Shop Website | Designed with HTML CSS JS</p>
  </footer>

  <script>
    function addToCart(product){
      alert(product + " added to cart!");
    }
  </script>

</body>
</html>
