<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>THE BOYS - Thrift Kicks & Custom Hoodies</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Bebas+Neue&family=Rajdhani:wght@300;500;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --black: #0a0a0a;
            --white: #ffffff;
            --red: #e63946;
            --green: #2ecc71;
            --gray: #1a1a1a;
        }

        body {
            background: var(--black);
            color: var(--white);
            font-family: 'Rajdhani', sans-serif;
            overflow-x: hidden;
        }

        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: var(--black);
        }
        ::-webkit-scrollbar-thumb {
            background: var(--red);
            border-radius: 4px;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 20px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
            background: rgba(10, 10, 10, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 2px solid var(--red);
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.5rem;
            font-weight: 900;
            color: var(--white);
            text-shadow: 0 0 20px var(--red), 0 0 40px var(--red);
            letter-spacing: 5px;
        }

        .logo span {
            color: var(--red);
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            color: var(--white);
            text-decoration: none;
            font-family: 'Bebas Neue', sans-serif;
            font-size: 1.3rem;
            letter-spacing: 3px;
            transition: all 0.3s;
            position: relative;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--red);
            transition: width 0.3s;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .nav-links a:hover {
            color: var(--red);
            text-shadow: 0 0 10px var(--red);
        }

        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
            background: radial-gradient(ellipse at center, #1a1a1a 0%, #0a0a0a 100%);
        }

        .hero-bg-text {
            position: absolute;
            font-family: 'Orbitron', sans-serif;
            font-size: 15vw;
            font-weight: 900;
            color: transparent;
            -webkit-text-stroke: 1px rgba(230, 57, 70, 0.1);
            z-index: 1;
            user-select: none;
            letter-spacing: 20px;
        }

        .shoe-container {
            position: relative;
            z-index: 10;
            width: 600px;
            height: 400px;
            perspective: 1000px;
        }

        .shoe-3d {
            width: 100%;
            height: 100%;
            position: relative;
            transform-style: preserve-3d;
            animation: float 6s ease-in-out infinite;
        }

        .shoe-3d img {
            width: 100%;
            height: auto;
            filter: drop-shadow(0 30px 60px rgba(230, 57, 70, 0.4));
            transform: rotateY(-15deg) rotateX(10deg);
            transition: transform 0.5s;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotateY(0deg); }
            50% { transform: translateY(-30px) rotateY(5deg); }
        }

        .hero-content {
            position: absolute;
            bottom: 100px;
            text-align: center;
            z-index: 20;
        }

        .hero-content h1 {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 5rem;
            letter-spacing: 15px;
            margin-bottom: 20px;
            text-shadow: 0 0 30px var(--red);
        }

        .hero-content p {
            font-size: 1.5rem;
            color: #888;
            letter-spacing: 5px;
            margin-bottom: 30px;
        }

        .scroll-indicator {
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            animation: bounce 2s infinite;
        }

        .scroll-indicator span {
            display: block;
            width: 30px;
            height: 50px;
            border: 2px solid var(--red);
            border-radius: 15px;
            position: relative;
        }

        .scroll-indicator span::before {
            content: '';
            position: absolute;
            top: 8px;
            left: 50%;
            transform: translateX(-50%);
            width: 6px;
            height: 6px;
            background: var(--red);
            border-radius: 50%;
            animation: scrollDown 2s infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateX(-50%) translateY(0); }
            50% { transform: translateX(-50%) translateY(10px); }
        }

        @keyframes scrollDown {
            0% { top: 8px; opacity: 1; }
            100% { top: 30px; opacity: 0; }
        }

        .products-section {
            padding: 100px 50px;
            background: var(--black);
        }

        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 3rem;
            text-align: center;
            margin-bottom: 60px;
            position: relative;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--red), var(--green));
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            max-width: 1400px;
            margin: 0 auto;
        }

        .product-card {
            background: var(--gray);
            border-radius: 20px;
            overflow: hidden;
            border: 2px solid transparent;
            transition: all 0.4s;
            position: relative;
            cursor: pointer;
        }

        .product-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, var(--red), var(--green));
            opacity: 0;
            transition: opacity 0.4s;
            z-index: 0;
        }

        .product-card:hover::before {
            opacity: 0.1;
        }

        .product-card:hover {
            border-color: var(--red);
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(230, 57, 70, 0.3);
        }

        .product-card .click-hint {
            position: absolute;
            top: 10px;
            right: 10px;
            background: var(--green);
            color: var(--black);
            font-family: 'Bebas Neue', sans-serif;
            font-size: 0.8rem;
            padding: 5px 12px;
            border-radius: 20px;
            z-index: 5;
            opacity: 0;
            transition: opacity 0.3s;
            letter-spacing: 2px;
        }

        .product-card:hover .click-hint {
            opacity: 1;
        }

        .product-img {
            height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            z-index: 1;
            overflow: hidden;
        }

        .product-img img {
            max-width: 80%;
            max-height: 80%;
            object-fit: contain;
            transition: transform 0.5s;
        }

        .product-card:hover .product-img img {
            transform: scale(1.1) rotate(-5deg);
        }

        .product-info {
            padding: 25px;
            position: relative;
            z-index: 1;
        }

        .product-tag {
            display: inline-block;
            padding: 5px 15px;
            background: var(--red);
            color: var(--white);
            font-family: 'Bebas Neue', sans-serif;
            font-size: 0.9rem;
            letter-spacing: 2px;
            border-radius: 20px;
            margin-bottom: 10px;
        }

        .product-tag.green {
            background: var(--green);
            color: var(--black);
        }

        .product-name {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.3rem;
            margin-bottom: 10px;
        }

        .product-price {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 2rem;
            color: var(--green);
            letter-spacing: 3px;
        }

        .product-price span {
            color: #666;
            text-decoration: line-through;
            font-size: 1.2rem;
            margin-left: 10px;
        }

        .about-section {
            padding: 100px 50px;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            position: relative;
            overflow: hidden;
        }

        .about-section::before {
            content: 'THE BOYS';
            position: absolute;
            font-family: 'Orbitron', sans-serif;
            font-size: 20vw;
            font-weight: 900;
            color: transparent;
            -webkit-text-stroke: 1px rgba(255, 255, 255, 0.03);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            white-space: nowrap;
            pointer-events: none;
        }

        .about-content {
            max-width: 1000px;
            margin: 0 auto;
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .about-content h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: 2.5rem;
            margin-bottom: 30px;
            color: var(--red);
        }

        .about-content p {
            font-size: 1.2rem;
            line-height: 1.8;
            color: #aaa;
            margin-bottom: 20px;
        }

        .stats {
            display: flex;
            justify-content: center;
            gap: 60px;
            margin-top: 50px;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-family: 'Orbitron', sans-serif;
            font-size: 3rem;
            color: var(--green);
            text-shadow: 0 0 20px var(--green);
        }

        .stat-label {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 1.2rem;
            letter-spacing: 3px;
            color: #888;
        }

        .contact-section {
            padding: 100px 50px;
            background: var(--black);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .contact-card {
            background: var(--gray);
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            border: 2px solid transparent;
            transition: all 0.4s;
            text-decoration: none;
            color: var(--white);
            display: block;
        }

        .contact-card:hover {
            border-color: var(--green);
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(46, 204, 113, 0.2);
        }

        .contact-icon {
            font-size: 3rem;
            margin-bottom: 20px;
        }

        .contact-card h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.3rem;
            margin-bottom: 10px;
        }

        .contact-card p {
            color: #888;
            font-size: 1rem;
        }

        .whatsapp-btn {
            background: linear-gradient(135deg, #25d366, #128c7e);
            border: none;
        }

        .whatsapp-btn:hover {
            border-color: #25d366;
            box-shadow: 0 15px 30px rgba(37, 211, 102, 0.3);
        }

        .instagram-btn {
            background: linear-gradient(135deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888);
            border: none;
        }

        .instagram-btn:hover {
            border-color: #e6683c;
            box-shadow: 0 15px 30px rgba(225, 48, 108, 0.3);
        }

        .call-btn {
            background: linear-gradient(135deg, var(--red), #c0392b);
        }

        .call-btn:hover {
            border-color: var(--red);
        }

        footer {
            background: #050505;
            padding: 40px;
            text-align: center;
            border-top: 2px solid var(--red);
        }

        footer .logo {
            font-size: 2rem;
            margin-bottom: 20px;
        }

        footer p {
            color: #666;
            font-size: 0.9rem;
        }

        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 9999;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: var(--red);
            border-radius: 50%;
            animation: particleFloat 10s infinite;
            opacity: 0.5;
        }

        @keyframes particleFloat {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 0; }
            10% { opacity: 0.5; }
            90% { opacity: 0.5; }
            100% { transform: translateY(-100vh) rotate(720deg); opacity: 0; }
        }

        @media (max-width: 768px) {
            .logo { font-size: 1.5rem; }
            .nav-links { display: none; }
            .hero-content h1 { font-size: 3rem; }
            .shoe-container { width: 300px; height: 200px; }
            .stats { flex-direction: column; gap: 30px; }
            .section-title { font-size: 2rem; }
        }

        .glitch {
            position: relative;
        }

        .glitch::before,
        .glitch::after {
            content: attr(data-text);
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .glitch::before {
            left: 2px;
            text-shadow: -2px 0 var(--green);
            clip: rect(24px, 550px, 90px, 0);
            animation: glitch-anim 3s infinite linear alternate-reverse;
        }

        .glitch::after {
            left: -2px;
            text-shadow: -2px 0 var(--red);
            clip: rect(85px, 550px, 140px, 0);
            animation: glitch-anim 2s infinite linear alternate-reverse;
        }

        @keyframes glitch-anim {
            0% { clip: rect(10px, 9999px, 85px, 0); }
            20% { clip: rect(63px, 9999px, 130px, 0); }
            40% { clip: rect(25px, 9999px, 15px, 0); }
            60% { clip: rect(88px, 9999px, 95px, 0); }
            80% { clip: rect(45px, 9999px, 60px, 0); }
            100% { clip: rect(15px, 9999px, 110px, 0); }
        }

        .neon-text {
            text-shadow: 
                0 0 5px var(--red),
                0 0 10px var(--red),
                0 0 20px var(--red),
                0 0 40px var(--red);
        }

        .neon-green {
            text-shadow: 
                0 0 5px var(--green),
                0 0 10px var(--green),
                0 0 20px var(--green),
                0 0 40px var(--green);
        }

        /* Buy Modal */
        .buy-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 10000;
            display: none;
            align-items: center;
            justify-content: center;
            backdrop-filter: blur(10px);
        }

        .buy-overlay.active {
            display: flex;
        }

        .buy-modal {
            background: linear-gradient(135deg, #1a1a1a, #0a0a0a);
            border: 2px solid var(--red);
            border-radius: 20px;
            padding: 40px;
            max-width: 500px;
            width: 90%;
            text-align: center;
            position: relative;
            animation: modalPop 0.4s ease;
            box-shadow: 0 0 50px rgba(230, 57, 70, 0.3);
        }

        @keyframes modalPop {
            0% { transform: scale(0.8); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }

        .buy-modal .close-btn {
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 2rem;
            color: var(--red);
            cursor: pointer;
            background: none;
            border: none;
        }

        .buy-modal img {
            width: 200px;
            height: 200px;
            object-fit: contain;
            border-radius: 15px;
            margin-bottom: 20px;
            border: 2px solid var(--red);
        }

        .buy-modal h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 10px;
            color: var(--white);
        }

        .buy-modal .modal-price {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 2.5rem;
            color: var(--green);
            letter-spacing: 3px;
            margin-bottom: 20px;
        }

        .buy-modal .modal-desc {
            color: #888;
            margin-bottom: 30px;
            font-size: 1rem;
        }

        .buy-modal .wa-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: linear-gradient(135deg, #25d366, #128c7e);
            color: white;
            text-decoration: none;
            padding: 15px 40px;
            border-radius: 50px;
            font-family: 'Bebas Neue', sans-serif;
            font-size: 1.3rem;
            letter-spacing: 3px;
            transition: all 0.3s;
            border: 2px solid transparent;
        }

        .buy-modal .wa-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.4);
            border-color: #25d366;
        }

        .buy-modal .wa-btn .wa-icon {
            font-size: 1.5rem;
        }
    </style>
<base target="_blank">
</head>
<body>
    <!-- Buy Modal -->
    <div class="buy-overlay" id="buyOverlay">
        <div class="buy-modal">
            <button class="close-btn" onclick="closeBuyModal()">&times;</button>
            <img id="modalImg" src="" alt="Product">
            <h3 id="modalName">Product Name</h3>
            <div class="modal-price" id="modalPrice">Rs. 0</div>
            <p class="modal-desc" id="modalDesc">Product description</p>
            <a id="waLink" href="#" target="_blank" class="wa-btn">
                <span class="wa-icon">💬</span>
                BUY ON WHATSAPP
            </a>
        </div>
    </div>

    <!-- Particles -->
    <div class="particles" id="particles"></div>

    <!-- Navigation -->
    <nav>
        <div class="logo glitch" data-text="THE BOYS">THE <span>BOYS</span></div>
        <ul class="nav-links">
            <li><a href="#home">HOME</a></li>
            <li><a href="#products">KICKS</a></li>
            <li><a href="#hoodies">HOODIES</a></li>
            <li><a href="#about">ABOUT</a></li>
            <li><a href="#contact">CONTACT</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-bg-text">AIR JORDAN</div>
        <div class="shoe-container">
            <div class="shoe-3d" id="shoe3d">
                <img src="https://images.unsplash.com/photo-1549298916-b41d501d3772?w=600&auto=format&fit=crop&q=80" alt="Nike Air Jordan">
            </div>
        </div>
        <div class="hero-content">
            <h1 class="neon-text">THE BOYS</h1>
            <p>THRIFT KICKS & CUSTOM HOODIES</p>
            <div style="font-family: 'Orbitron'; font-size: 1rem; color: var(--green); letter-spacing: 5px;">
                AUTHENTIC. RARE. CUSTOM.
            </div>
        </div>
        <div class="scroll-indicator">
            <span></span>
        </div>
    </section>

    <!-- Thrift Shoes Section -->
    <section class="products-section" id="products">
        <h2 class="section-title glitch" data-text="THRIFT KICKS">THRIFT <span style="color: var(--red);">KICKS</span></h2>
        <div class="products-grid">
            <div class="product-card" onclick="openBuyModal('Air Jordan 1 Retro', 'Rs. 12,500', 'Chicago Colorway - Thrift Find', 'https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?w=400&auto=format&fit=crop&q=80" alt="Air Jordan 1">
                </div>
                <div class="product-info">
                    <span class="product-tag">RARE</span>
                    <h3 class="product-name">Air Jordan 1 Retro</h3>
                    <p style="color: #888; margin-bottom: 10px;">Chicago Colorway - Thrift Find</p>
                    <div class="product-price">Rs. 12,500 <span>Rs. 18,000</span></div>
                </div>
            </div>

            <div class="product-card" onclick="openBuyModal('Air Jordan 4 Bred', 'Rs. 15,000', '1999 Release - OG Box', 'https://images.unsplash.com/photo-1600185365926-3a2ce3cdb9eb?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1600185365926-3a2ce3cdb9eb?w=400&auto=format&fit=crop&q=80" alt="Air Jordan 4">
                </div>
                <div class="product-info">
                    <span class="product-tag">VINTAGE</span>
                    <h3 class="product-name">Air Jordan 4 Bred</h3>
                    <p style="color: #888; margin-bottom: 10px;">1999 Release - OG Box</p>
                    <div class="product-price">Rs. 15,000 <span>Rs. 22,000</span></div>
                </div>
            </div>

            <div class="product-card" onclick="openBuyModal('Air Jordan 11 Concord', 'Rs. 18,000', 'Never Worn - Original', 'https://images.unsplash.com/photo-1605348532760-6753d2c43329?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1605348532760-6753d2c43329?w=400&auto=format&fit=crop&q=80" alt="Air Jordan 11">
                </div>
                <div class="product-info">
                    <span class="product-tag">DEADSTOCK</span>
                    <h3 class="product-name">Air Jordan 11 Concord</h3>
                    <p style="color: #888; margin-bottom: 10px;">Never Worn - Original</p>
                    <div class="product-price">Rs. 18,000 <span>Rs. 25,000</span></div>
                </div>
            </div>

            <div class="product-card" onclick="openBuyModal('Air Jordan 3 White Cement', 'Rs. 9,500', 'Cleaned & Restored', 'https://images.unsplash.com/photo-1556906781-9a412961c28c?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1556906781-9a412961c28c?w=400&auto=format&fit=crop&q=80" alt="Air Jordan 3">
                </div>
                <div class="product-info">
                    <span class="product-tag">THRIFT</span>
                    <h3 class="product-name">Air Jordan 3 White Cement</h3>
                    <p style="color: #888; margin-bottom: 10px;">Cleaned & Restored</p>
                    <div class="product-price">Rs. 9,500 <span>Rs. 14,000</span></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Custom Hoodies Section -->
    <section class="products-section" id="hoodies" style="background: linear-gradient(180deg, #0a0a0a 0%, #111 100%);">
        <h2 class="section-title glitch" data-text="CUSTOM HOODIES">CUSTOM <span style="color: var(--green);">HOODIES</span></h2>
        <div class="products-grid">
            <div class="product-card" onclick="openBuyModal('THE BOYS Signature Hoodie', 'Rs. 3,500', 'Hand-painted Design', 'https://images.unsplash.com/photo-1556821840-3a63f95609a7?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1556821840-3a63f95609a7?w=400&auto=format&fit=crop&q=80" alt="Custom Hoodie">
                </div>
                <div class="product-info">
                    <span class="product-tag green">CUSTOM</span>
                    <h3 class="product-name">THE BOYS Signature Hoodie</h3>
                    <p style="color: #888; margin-bottom: 10px;">Hand-painted Design</p>
                    <div class="product-price">Rs. 3,500</div>
                </div>
            </div>

            <div class="product-card" onclick="openBuyModal('Jordan x THE BOYS Collab', 'Rs. 4,200', 'Limited Edition Print', 'https://images.unsplash.com/photo-1578587018452-892bacefd9f8?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1578587018452-892bacefd9f8?w=400&auto=format&fit=crop&q=80" alt="Jordan Hoodie">
                </div>
                <div class="product-info">
                    <span class="product-tag green">EXCLUSIVE</span>
                    <h3 class="product-name">Jordan x THE BOYS Collab</h3>
                    <p style="color: #888; margin-bottom: 10px;">Limited Edition Print</p>
                    <div class="product-price">Rs. 4,200</div>
                </div>
            </div>

            <div class="product-card" onclick="openBuyModal('Street Legend Hoodie', 'Rs. 3,800', 'Embroidered Logo', 'https://images.unsplash.com/photo-1620799140408-edc6dcb6d633?w=400&auto=format&fit=crop&q=80')">
                <div class="click-hint">CLICK TO BUY</div>
                <div class="product-img">
                    <img src="https://images.unsplash.com/photo-1620799140408-edc6dcb6d633?w=400&auto=format&fit=crop&q=80" alt="Street Hoodie">
                </div>
                <div class="product-info">
                    <span class="product-tag green">NEW DROP</span>
                    <h3 class="product-name">Street Legend Hoodie</h3>
                    <p style="color: #888; margin-bottom: 10px;">Embroidered Logo</p>
                    <div class="product-price">Rs. 3,800</div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about-section" id="about">
        <div class="about-content">
            <h2 class="glitch" data-text="WHO WE ARE">WHO WE <span style="color: var(--green);">ARE</span></h2>
            <p>
                THE BOYS is not just a store - it's a movement. We hunt down the rarest thrift kicks 
                and create custom hoodies that speak your style. Every pair of shoes tells a story, 
                and every hoodie is a canvas of self-expression.
            </p>
            <p>
                From vintage Air Jordans to hand-painted custom pieces, we bring you authenticity 
                that mass-produced brands can't match. Join the culture. Join THE BOYS.
            </p>
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number neon-green">500+</div>
                    <div class="stat-label">KICKS SOLD</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number neon-text">300+</div>
                    <div class="stat-label">HOODIES MADE</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number" style="color: var(--white); text-shadow: 0 0 20px var(--white);">100%</div>
                    <div class="stat-label">AUTHENTIC</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact-section" id="contact">
        <h2 class="section-title glitch" data-text="HIT US UP">HIT US <span style="color: var(--red);">UP</span></h2>
        <div class="contact-grid">
            <a href="tel:03173013526" class="contact-card call-btn">
                <div class="contact-icon">📞</div>
                <h3>CALL NOW</h3>
                <p>0317-3013526</p>
            </a>

            <a href="tel:03712503042" class="contact-card call-btn">
                <div class="contact-icon">📱</div>
                <h3>CALL NOW</h3>
                <p>0371-2503042</p>
            </a>

            <a href="https://wa.me/923153859606" target="_blank" class="contact-card whatsapp-btn">
                <div class="contact-icon">💬</div>
                <h3>WHATSAPP</h3>
                <p>0315-3859606<br><small>Click to Chat Directly</small></p>
            </a>

            <a href="https://wa.me/923153859606" target="_blank" class="contact-card whatsapp-btn">
                <div class="contact-icon">💬</div>
                <h3>WHATSAPP</h3>
                <p>0315-3859606<br><small>Click to Chat Directly</small></p>
            </a>

            <a href="https://www.instagram.com/the_boys_331122?igsh=MWh6cnFlMzRrOGx1aA%3D%3D&utm_source=qr" target="_blank" class="contact-card instagram-btn">
                <div class="contact-icon">📸</div>
                <h3>INSTAGRAM</h3>
                <p>@the_boys_331122<br><small>Follow for Drops</small></p>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="logo">THE <span>BOYS</span></div>
        <p>© 2026 THE BOYS. All Rights Reserved. | Thrift Kicks & Custom Hoodies</p>
        <p style="margin-top: 10px; font-family: 'Orbitron'; font-size: 0.8rem; color: var(--red);">
            STAY FRESH. STAY REAL. STAY THE BOYS.
        </p>
    </footer>

    <script>
        // Buy Modal Functions
        function openBuyModal(name, price, desc, imgUrl) {
            const overlay = document.getElementById('buyOverlay');
            const modalImg = document.getElementById('modalImg');
            const modalName = document.getElementById('modalName');
            const modalPrice = document.getElementById('modalPrice');
            const modalDesc = document.getElementById('modalDesc');
            const waLink = document.getElementById('waLink');

            modalImg.src = imgUrl;
            modalName.textContent = name;
            modalPrice.textContent = price;
            modalDesc.textContent = desc;

            // WhatsApp message with product details
            const waNumber = '923712503042'; // 03712503042 with country code
            const message = `🔥 THE BOYS - ORDER REQUEST 🔥%0A%0A` +
                           `📦 Product: ${name}%0A` +
                           `💰 Price: ${price}%0A` +
                           `📝 Details: ${desc}%0A%0A` +
                           `👤 Customer wants to buy this item!%0A` +
                           `📎 Product Image: ${imgUrl}%0A%0A` +
                           `Please confirm availability!`;

            waLink.href = `https://wa.me/${waNumber}?text=${message}`;

            overlay.classList.add('active');
            document.body.style.overflow = 'hidden';
        }

        function closeBuyModal() {
            const overlay = document.getElementById('buyOverlay');
            overlay.classList.remove('active');
            document.body.style.overflow = 'auto';
        }

        // Close modal on overlay click
        document.getElementById('buyOverlay').addEventListener('click', function(e) {
            if (e.target === this) {
                closeBuyModal();
            }
        });

        // Close on Escape key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeBuyModal();
            }
        });

        // 3D Shoe Scroll Effect
        const shoe3d = document.getElementById('shoe3d');
        const shoeImg = shoe3d.querySelector('img');

        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const rotateY = scrolled * 0.1;
            const rotateX = 10 + (scrolled * 0.05);
            const translateY = -(scrolled * 0.3);

            shoeImg.style.transform = `rotateY(${-15 + rotateY}deg) rotateX(${rotateX}deg) translateY(${translateY}px)`;
            shoe3d.style.animation = 'none';
        });

        // Particle System
        const particlesContainer = document.getElementById('particles');
        for (let i = 0; i < 50; i++) {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.animationDelay = Math.random() * 10 + 's';
            particle.style.animationDuration = (Math.random() * 10 + 10) + 's';
            particle.style.background = Math.random() > 0.5 ? 'var(--red)' : 'var(--green)';
            particlesContainer.appendChild(particle);
        }

        // Smooth Scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Glitch Effect Randomizer
        setInterval(() => {
            const glitches = document.querySelectorAll('.glitch');
            glitches.forEach(el => {
                if (Math.random() > 0.9) {
                    el.style.animation = 'none';
                    setTimeout(() => {
                        el.style.animation = '';
                    }, 100);
                }
            });
        }, 2000);

        // Intersection Observer for animations
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.product-card, .contact-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(50px)';
            el.style.transition = 'all 0.6s ease';
            observer.observe(el);
        });
    </script>
</body>
</html>
