<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gourmet Bites - Fresh. Gourmet. Delivered.</title>
    <style>
        /* CSS RESET & VARIABLES */
        :root {
            --primary-color: #2c5530; /* Hijau Tua Tua */
            --accent-color: #4caf50; /* Hijau Terang */
            --accent-hover: #388e3c;
            --text-dark: #333;
            --text-light: #666;
            --bg-light: #f9f9f9;
            --offer-bg: #d4edda;
            --offer-text: #155724;
            --white: #ffffff;
            --shadow: 0 2px 10px rgba(0,0,0,0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        a { text-decoration: none; color: inherit; transition: var(--transition); }
        ul { list-style: none; }
        img { max-width: 100%; height: auto; display: block; }

        /* UTILITAS */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .btn {
            display: inline-block;
            padding: 10px 25px;
            background-color: var(--accent-color);
            color: var(--white);
            border-radius: 5px;
            font-weight: bold;
            border: none;
            cursor: pointer;
            text-align: center;
        }

        .btn:hover { background-color: var(--accent-hover); }

        .section-title {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: #000;
        }

        /* --- HEADER & NAV --- */
        header {
            background-color: var(--white);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
        }

        .nav-links {
            display: flex;
            gap: 20px;
        }

        .nav-links a {
            font-size: 0.9rem;
            color: var(--text-dark);
        }

        .nav-links a:hover, .nav-links a.active {
            color: var(--accent-color);
            font-weight: 600;
        }

        .nav-icons {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 0.9rem;
        }

        .cart-icon {
            position: relative;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .cart-count {
            background-color: var(--accent-color);
            color: var(--white);
            font-size: 0.7rem;
            padding: 2px 6px;
            border-radius: 50%;
            font-weight: bold;
        }

        /* --- HERO SECTION --- */
        .hero {
            padding: 40px 0;
        }

        .hero-grid {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 20px;
        }

        /* Banner Utama Besar */
        .main-banner {
            background-image: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://via.placeholder.com/800x500?text=Table+Spread+of+Food'); /* GANTI GAMBAR DI SINI */
            background-size: cover;
            background-position: center;
            color: var(--white);
            padding: 60px;
            border-radius: 10px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
        }

        .main-banner h4 { font-size: 0.9rem; text-transform: uppercase; letter-spacing: 1px; margin-bottom: 10px; }
        .main-banner h1 { font-size: 2.5rem; line-height: 1.2; margin-bottom: 15px; font-weight: 700; }
        .main-banner p { font-size: 1rem; margin-bottom: 25px; max-width: 400px; opacity: 0.9; }

        /* Side Specials (Sebelah Hero) */
        .side-specials {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .special-card-mini {
            background: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            position: relative;
            height: calc(50% - 10px);
        }

        .special-card-mini img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .special-card-mini .info {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            padding: 15px;
            background: linear-gradient(to top, rgba(0,0,0,0.7), transparent);
            color: var(--white);
        }
        .special-card-mini h3 { font-size: 1rem; }

        /* --- OFFER BANNER (Summer Deals) --- */
        .offer-banner {
            margin: 20px 0 40px 0;
        }

        .offer-container {
            background-color: #e8f5e9; /* Hijau sangat muda */
            border-radius: 10px;
            padding: 30px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border: 1px solid #c3e6cb;
        }

        .offer-text h3 { color: #cc0000; text-transform: uppercase; font-size: 0.8rem; letter-spacing: 1px; margin-bottom: 5px; }
        .offer-text h2 { font-size: 1.8rem; color: #155724; margin-bottom: 5px; }
        .offer-text p { color: #155724; font-weight: bold; font-size: 1rem; margin-bottom: 15px; }

        .offer-images {
            display: flex;
            gap: 15px;
            align-items: center;
        }
        .offer-images img { height: 100px; } /* Sesuaikan tinggi gambar jus */

        /* --- PRODUCT GRID SYSTEM (Chef's Picks & Drinks) --- */
        .products-section {
            padding: 30px 0;
        }

        .section-header-flex {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        .item-count { font-size: 0.8rem; color: var(--text-light); }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
        }

        .product-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 15px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
        }

        .product-card:hover { transform: translateY(-5px); }

        .product-img-wrapper {
            width: 100%;
            height: 160px;
            overflow: hidden;
            border-radius: 8px;
            margin-bottom: 15px;
        }
        .product-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .product-info h3 {
            font-size: 0.95rem;
            margin-bottom: 5px;
            color: #000;
            height: 40px; /* Menjaga tinggi nama produk sama */
            overflow: hidden;
        }

        .rating-price {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            font-size: 0.85rem;
        }

        .rating { color: #fbc02d; font-weight: bold; }
        .price { font-weight: bold; color: var(--text-dark); }

        .btn-add {
            width: 100%;
            padding: 8px;
            background-color: var(--accent-color);
            color: var(--white);
            border: none;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            font-size: 0.8rem;
            text-transform: uppercase;
        }
        .btn-add:hover { background-color: var(--accent-hover); }

        /* --- HOW IT WORKS --- */
        .how-it-works {
            background-color: var(--white);
            padding: 50px 0;
            margin: 40px 0;
            text-align: center;
        }

        .how-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 30px;
            margin-top: 30px;
        }

        .how-item {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .icon-box {
            font-size: 2rem;
            color: var(--accent-color);
            margin-bottom: 15px;
        }

        .how-item p {
            font-size: 0.85rem;
            color: var(--text-light);
            max-width: 200px;
        }

        /* --- FOOTER --- */
        footer {
            background-color: var(--white);
            padding: 50px 0 20px 0;
            border-top: 1px solid #eee;
            font-size: 0.85rem;
            color: var(--text-light);
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-col h4 {
            color: var(--text-dark);
            margin-bottom: 15px;
            font-size: 0.9rem;
        }

        .footer-col ul li { margin-bottom: 8px; }
        .footer-col ul li a:hover { color: var(--accent-color); padding-left: 5px; }

        .newsletter-input {
            display: flex;
            gap: 5px;
            margin-bottom: 15px;
        }

        .newsletter-input input {
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            flex-grow: 1;
            font-size: 0.8rem;
        }

        .btn-subscribe {
            padding: 8px 15px;
            background-color: var(--accent-color);
            color: var(--white);
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            font-size: 0.8rem;
        }

        .payment-methods {
            display: flex;
            gap: 10px;
            align-items: center;
            margin-top: 10px;
        }
        .payment-methods img { height: 15px; opacity: 0.7; }

        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid #eee;
            font-size: 0.75rem;
        }

        /* --- RESPONSIVE MEDIA QUERIES --- */
        @media (max-width: 1024px) {
            .product-grid { grid-template-columns: repeat(3, 1fr); }
            .how-grid, .footer-grid { grid-template-columns: repeat(2, 1fr); }
            .main-banner { padding: 40px; }
            .main-banner h1 { font-size: 2rem; }
        }

        @media (max-width: 768px) {
            .hero-grid { grid-template-columns: 1fr; }
            .nav-links { display: none; } /* Sembunyikan nav di mobile, butuh JS untuk burger menu asli */
            .offer-container { flex-direction: column; text-align: center; padding: 20px; }
            .offer-images { margin-top: 20px; }
            .product-grid { grid-template-columns: repeat(2, 1fr); }
            .footer-grid { grid-template-columns: 1fr; text-align: center; }
            .newsletter-input { justify-content: center; }
            .payment-methods { justify-content: center; }
        }

        @media (max-width: 480px) {
            .product-grid { grid-template-columns: 1fr; }
            .main-banner h1 { font-size: 1.5rem; }
            .offer-text h2 { font-size: 1.4rem; }
        }
    </style>
</head>
<body>

    <!-- 1. HEADER & NAVIGATION -->
    <header>
        <div class="container nav-container">
            <div class="logo">Gourmet Bites</div>
            <nav>
                <ul class="nav-links">
                    <li><a href="#" class="active">Home</a></li>
                    <li><a href="#">Shop All</a></li>
                    <li><a href="#">Chef's Specials</a></li>
                    <li><a href="#">Offers</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
            <div class="nav-icons">
                <a href="#">🔍</a> <!-- Icon Search -->
                <a href="#">👤</a> <!-- Icon User -->
                <div class="cart-icon">
                    <a href="#">🛒 Cart</a>
                    <span class="cart-count">3</span>
                </div>
                <a href="#">Log in/Sign up</a>
            </div>
        </div>
    </header>

    <main class="container">
        
        <!-- 2. HERO SECTION (Banner Besar + Daily Specials) -->
        <section class="hero">
            <div class="hero-grid">
                <!-- Banner Utama -->
                <div class="main-banner">
                    <h4>Fresh. Gourmet. Delivered.</h4>
                    <h1>Discover Exquisite<br>Meals & Drinks!</h1>
                    <p>Fresh, gourmet meals and drinks to satisfy your cravings with high-quality ingredients.</p>
                    <button class="btn">ORDER NOW</button>
                </div>

                <!-- Daily Specials (Kanan) -->
                <div class="side-specials">
                    <h2 class="section-title">Daily Specials</h2>
                    <!-- Card 1 -->
                    <div class="special-card-mini">
                        <img src="https://via.placeholder.com/400x200?text=Grilled+Steak" alt="Grilled Steak"> <!-- GANTI GAMBAR -->
                        <div class="info">
                            <h3>Grilled Steak</h3>
                        </div>
                    </div>
                    <!-- Card 2 -->
                    <div class="special-card-mini">
                        <img src="https://via.placeholder.com/400x200?text=Avocado+Toast" alt="Avocado Toast"> <!-- GANTI GAMBAR -->
                        <div class="info">
                            <h3>Avocado Toast</h3>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 3. OFFER BANNER (Summer Deals) -->
        <section class="offer-banner">
            <div class="offer-container">
                <div class="offer-text">
                    <h3>Summer Deals!</h3>
                    <h2>20% OFF ALL FRUIT DRINKS!</h2>
                    <p>Code: FRESH20</p>
                    <button class="btn">VIEW ALL</button>
                </div>
                <div class="offer-images">
                    <img src="https://via.placeholder.com/100x100?text=Juice1" alt="Juice 1"> <!-- GANTI GAMBAR -->
                    <img src="https://via.placeholder.com/100x100?text=Juice2" alt="Juice 2"> <!-- GANTI GAMBAR -->
                </div>
            </div>
        </section>

        <!-- 4. CHEF'S PICKS SECTION -->
        <section class="products-section">
            <div class="section-header-flex">
                <h2 class="section-title">CHEF'S PICKS: FRESH GOURMET DISHES</h2>
                <span class="item-count">6 items</span>
            </div>

            <div class="product-grid">
                <!-- Product 1 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Salmon" alt="Seared Salmon"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Seared Salmon with Spinach</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 4.9/5</span>
                            <span class="price">$18.99</span>
                        </div>
                        <button class="btn-add">ADD TO CART</button>
                    </div>
                </div>
                <!-- Product 2 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Pasta" alt="Pasta Pesto"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Pesto Pasta with Tomatoes</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 4.7/5</span>
                            <span class="price">$14.50</span>
                        </div>
                        <button class="btn-add">ADD TO CART</button>
                    </div>
                </div>
                <!-- Product 3 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Salad" alt="Quinoa Salad"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Loaded Quinoa Salad Bowl</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 4.8/5</span>
                            <span class="price">$12.99</span>
                        </div>
                        <button class="btn-add">ADD TO CART</button>
                    </div>
                </div>
                <!-- Product 4 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Burger" alt="Gourmet Burger"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Classic Gourmet Beef Burger</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 5.0/5</span>
                            <span class="price">$16.00</span>
                        </div>
                        <button class="btn-add">ADD TO CART</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- 5. DRINKS SECTION -->
        <section class="products-section">
            <div class="section-header-flex">
                <h2 class="section-title">REFRESHING SIPS: COLORFUL FRUIT DRINKS</h2>
                <span class="item-count">4 items</span>
            </div>

            <div class="product-grid">
                <!-- Drink 1 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Berry+Bliss" alt="Berry Bliss"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Berry Bliss Smoothie</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 4.8/5</span>
                            <span class="price">$7.50</span>
                        </div>
                        <button class="btn-add">ADD TO CART</button>
                    </div>
                </div>
                <!-- Drink 2 -->
                <div class="product-card">
                    <div class="product-img-wrapper">
                        <img src="https://via.placeholder.com/200x160?text=Mango+Splash" alt="Mango Splash"> <!-- GANTI GAMBAR -->
                    </div>
                    <div class="product-info">
                        <h3>Mango Splash Juice</h3>
                        <div class="rating-price">
                            <span class="rating">⭐ 4.9/5</span>
                            <span class="price">$7.50</span>
                        </div>
               
