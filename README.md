<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KicksxxlandRd – donde el sueño del buen vestir se hace realidad</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Nunito:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --purple: #5B3EC8;
    --blue: #3B8BEB;
    --coral: #E8556D;
    --gold: #E8A93C;
    --dark: #0f0f0f;
    --light: #fafafa;
    --card-bg: #ffffff;
    --border: #ececec;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Nunito', sans-serif;
    background: var(--light);
    color: var(--dark);
    overflow-x: hidden;
  }

  /* HEADER */
  header {
    background: var(--dark);
    padding: 0 2rem;
    position: sticky;
    top: 0;
    z-index: 100;
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 70px;
    box-shadow: 0 2px 20px rgba(0,0,0,0.3);
  }

  .logo-area {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .logo-icon {
    width: 44px;
    height: 44px;
    position: relative;
  }

  .logo-icon svg { width: 100%; height: 100%; }

  .logo-text {
    font-family: 'Bebas Neue', cursive;
    font-size: 1.7rem;
    letter-spacing: 2px;
    background: linear-gradient(135deg, var(--purple), var(--blue), var(--coral), var(--gold));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  nav { display: flex; gap: 2rem; }
  nav a {
    color: #ccc;
    text-decoration: none;
    font-weight: 600;
    font-size: 0.9rem;
    letter-spacing: 1px;
    text-transform: uppercase;
    transition: color 0.2s;
  }
  nav a:hover { color: var(--gold); }

  .cart-btn {
    background: linear-gradient(135deg, var(--purple), var(--coral));
    color: white;
    border: none;
    padding: 8px 18px;
    border-radius: 25px;
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    cursor: pointer;
    font-size: 0.85rem;
    display: flex;
    align-items: center;
    gap: 6px;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .cart-btn:hover { transform: scale(1.05); box-shadow: 0 4px 15px rgba(91,62,200,0.4); }
  .cart-count {
    background: var(--gold);
    color: var(--dark);
    border-radius: 50%;
    width: 20px;
    height: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.75rem;
    font-weight: 800;
  }

  /* HERO */
  .hero {
    background: var(--dark);
    min-height: 520px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 4rem 2rem;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    width: 600px;
    height: 600px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(91,62,200,0.25) 0%, transparent 70%);
    top: -200px;
    left: -150px;
  }

  .hero::after {
    content: '';
    position: absolute;
    width: 500px;
    height: 500px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(232,85,109,0.2) 0%, transparent 70%);
    bottom: -200px;
    right: -100px;
  }

  .hero-content { position: relative; z-index: 2; max-width: 700px; }

  .hero-badge {
    display: inline-block;
    background: rgba(232,169,60,0.15);
    border: 1px solid var(--gold);
    color: var(--gold);
    font-size: 0.75rem;
    font-weight: 700;
    letter-spacing: 3px;
    text-transform: uppercase;
    padding: 6px 18px;
    border-radius: 25px;
    margin-bottom: 1.5rem;
    animation: fadeInDown 0.6s ease;
  }

  .hero h1 {
    font-family: 'Bebas Neue', cursive;
    font-size: clamp(3rem, 8vw, 5.5rem);
    line-height: 1;
    color: white;
    letter-spacing: 4px;
    margin-bottom: 1rem;
    animation: fadeInUp 0.7s ease 0.1s both;
  }

  .hero h1 span {
    background: linear-gradient(135deg, var(--purple), var(--blue), var(--coral));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .hero p {
    color: #aaa;
    font-size: 1rem;
    font-style: italic;
    margin-bottom: 2.5rem;
    animation: fadeInUp 0.7s ease 0.2s both;
  }

  .hero-btns {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
    animation: fadeInUp 0.7s ease 0.3s both;
  }

  .btn-primary {
    background: linear-gradient(135deg, var(--purple), var(--coral));
    color: white;
    border: none;
    padding: 14px 32px;
    border-radius: 30px;
    font-family: 'Nunito', sans-serif;
    font-weight: 800;
    font-size: 1rem;
    cursor: pointer;
    text-decoration: none;
    transition: transform 0.2s, box-shadow 0.2s;
    letter-spacing: 1px;
  }
  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 25px rgba(91,62,200,0.5); }

  .btn-secondary {
    background: transparent;
    color: white;
    border: 2px solid rgba(255,255,255,0.3);
    padding: 14px 32px;
    border-radius: 30px;
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    font-size: 1rem;
    cursor: pointer;
    text-decoration: none;
    transition: border-color 0.2s, color 0.2s;
  }
  .btn-secondary:hover { border-color: var(--gold); color: var(--gold); }

  /* MARQUEE */
  .marquee-bar {
    background: linear-gradient(135deg, var(--purple), var(--blue));
    padding: 10px 0;
    overflow: hidden;
    white-space: nowrap;
  }
  .marquee-inner {
    display: inline-block;
    animation: marquee 20s linear infinite;
    font-weight: 700;
    font-size: 0.85rem;
    letter-spacing: 2px;
    color: white;
    text-transform: uppercase;
  }
  .marquee-inner span { margin: 0 2rem; opacity: 0.7; }

  /* SECTION */
  section { padding: 4rem 2rem; max-width: 1200px; margin: 0 auto; }

  .section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 2.5rem;
    flex-wrap: wrap;
    gap: 1rem;
  }

  .section-title {
    font-family: 'Bebas Neue', cursive;
    font-size: 2.5rem;
    letter-spacing: 3px;
    color: var(--dark);
    position: relative;
  }

  .section-title::after {
    content: '';
    position: absolute;
    bottom: -6px;
    left: 0;
    width: 60px;
    height: 4px;
    border-radius: 2px;
    background: linear-gradient(135deg, var(--purple), var(--coral));
  }

  /* FILTER TABS */
  .filter-tabs {
    display: flex;
    gap: 0.5rem;
    flex-wrap: wrap;
  }

  .filter-tab {
    padding: 7px 18px;
    border-radius: 25px;
    border: 2px solid var(--border);
    background: white;
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    font-size: 0.85rem;
    cursor: pointer;
    transition: all 0.2s;
    color: var(--dark);
  }
  .filter-tab:hover, .filter-tab.active {
    background: var(--purple);
    border-color: var(--purple);
    color: white;
  }

  /* PRODUCT GRID */
  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
    gap: 1.5rem;
  }

  .product-card {
    background: white;
    border-radius: 16px;
    overflow: hidden;
    border: 1px solid var(--border);
    transition: transform 0.25s, box-shadow 0.25s;
    position: relative;
  }

  .product-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 16px 40px rgba(0,0,0,0.12);
  }

  .product-badge {
    position: absolute;
    top: 12px;
    left: 12px;
    background: var(--coral);
    color: white;
    font-size: 0.7rem;
    font-weight: 800;
    letter-spacing: 1px;
    text-transform: uppercase;
    padding: 4px 10px;
    border-radius: 25px;
    z-index: 2;
  }

  .product-badge.new { background: var(--purple); }
  .product-badge.sale { background: var(--coral); }

  .product-img {
    width: 100%;
    height: 220px;
    object-fit: cover;
    background: linear-gradient(135deg, #f0f0f0, #e0e0e0);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 5rem;
    position: relative;
    overflow: hidden;
  }

  .product-img-placeholder {
    width: 100%;
    height: 220px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 5rem;
    position: relative;
  }

  .product-info { padding: 1.2rem; }

  .product-brand {
    font-size: 0.7rem;
    font-weight: 800;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--purple);
    margin-bottom: 4px;
  }

  .product-name {
    font-size: 1rem;
    font-weight: 800;
    color: var(--dark);
    margin-bottom: 6px;
  }

  .product-desc {
    font-size: 0.82rem;
    color: #888;
    margin-bottom: 12px;
    line-height: 1.5;
  }

  .product-footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .product-price {
    font-size: 1.3rem;
    font-weight: 800;
    color: var(--dark);
  }

  .add-to-cart {
    background: linear-gradient(135deg, var(--purple), var(--blue));
    color: white;
    border: none;
    padding: 9px 18px;
    border-radius: 25px;
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    font-size: 0.85rem;
    cursor: pointer;
    transition: transform 0.15s, box-shadow 0.15s;
  }
  .add-to-cart:hover { transform: scale(1.05); box-shadow: 0 4px 15px rgba(91,62,200,0.4); }

  /* SIZE SELECTOR */
  .size-selector { display: flex; gap: 6px; margin-bottom: 12px; flex-wrap: wrap; }
  .size-btn {
    padding: 4px 10px;
    border: 1.5px solid var(--border);
    border-radius: 8px;
    font-size: 0.75rem;
    font-weight: 700;
    cursor: pointer;
    background: white;
    transition: all 0.15s;
  }
  .size-btn:hover, .size-btn.selected { background: var(--dark); color: white; border-color: var(--dark); }

  /* INSTAGRAM SECTION */
  .insta-section {
    background: var(--dark);
    padding: 4rem 2rem;
    text-align: center;
  }

  .insta-section h2 {
    font-family: 'Bebas Neue', cursive;
    font-size: 2.5rem;
    letter-spacing: 3px;
    color: white;
    margin-bottom: 0.5rem;
  }

  .insta-section p { color: #aaa; margin-bottom: 2rem; font-size: 0.95rem; }

  .insta-handle {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: linear-gradient(135deg, #833ab4, #fd1d1d, #fcb045);
    color: white;
    padding: 14px 32px;
    border-radius: 30px;
    font-weight: 800;
    font-size: 1.1rem;
    text-decoration: none;
    transition: transform 0.2s, box-shadow 0.2s;
    letter-spacing: 1px;
  }
  .insta-handle:hover { transform: translateY(-2px); box-shadow: 0 8px 25px rgba(253,29,29,0.4); }

  .insta-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 8px;
    max-width: 600px;
    margin: 2rem auto;
  }

  .insta-placeholder {
    aspect-ratio: 1;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 2rem;
    background: rgba(255,255,255,0.05);
    border: 1px solid rgba(255,255,255,0.1);
    transition: transform 0.2s;
    cursor: pointer;
  }
  .insta-placeholder:hover { transform: scale(1.03); }

  /* CART MODAL */
  .cart-overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.6);
    z-index: 200;
    backdrop-filter: blur(4px);
  }
  .cart-overlay.open { display: flex; justify-content: flex-end; }

  .cart-panel {
    background: white;
    width: min(420px, 100vw);
    height: 100vh;
    overflow-y: auto;
    padding: 2rem;
    transform: translateX(100%);
    transition: transform 0.3s ease;
  }
  .cart-overlay.open .cart-panel { transform: translateX(0); }

  .cart-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
  }

  .cart-title {
    font-family: 'Bebas Neue', cursive;
    font-size: 2rem;
    letter-spacing: 2px;
  }

  .close-cart {
    background: none;
    border: none;
    font-size: 1.8rem;
    cursor: pointer;
    color: var(--dark);
    line-height: 1;
  }

  .cart-items { margin-bottom: 2rem; }

  .cart-item {
    display: flex;
    gap: 12px;
    padding: 1rem 0;
    border-bottom: 1px solid var(--border);
    align-items: center;
  }

  .cart-item-emoji { font-size: 2.5rem; }

  .cart-item-info { flex: 1; }
  .cart-item-name { font-weight: 800; font-size: 0.95rem; }
  .cart-item-size { font-size: 0.78rem; color: #888; }
  .cart-item-price { font-weight: 800; color: var(--purple); }

  .remove-item {
    background: none;
    border: none;
    cursor: pointer;
    color: var(--coral);
    font-size: 1.2rem;
    font-weight: 700;
  }

  .cart-empty {
    text-align: center;
    padding: 3rem 0;
    color: #aaa;
    font-size: 1rem;
  }

  .cart-total {
    display: flex;
    justify-content: space-between;
    font-weight: 800;
    font-size: 1.2rem;
    margin-bottom: 1.5rem;
    padding-top: 1rem;
    border-top: 2px solid var(--dark);
  }

  .checkout-section { display: flex; flex-direction: column; gap: 0.75rem; }

  .checkout-btn {
    width: 100%;
    padding: 14px;
    border-radius: 12px;
    font-family: 'Nunito', sans-serif;
    font-weight: 800;
    font-size: 1rem;
    cursor: pointer;
    transition: transform 0.15s;
    border: none;
  }
  .checkout-btn:hover { transform: scale(1.02); }

  .btn-card {
    background: linear-gradient(135deg, var(--purple), var(--blue));
    color: white;
  }

  .btn-cash { background: var(--gold); color: var(--dark); }
  .btn-venmo { background: #3D95CE; color: white; }

  /* PAYMENT MODAL */
  .modal-overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.7);
    z-index: 300;
    align-items: center;
    justify-content: center;
    backdrop-filter: blur(4px);
    padding: 1rem;
  }
  .modal-overlay.open { display: flex; }

  .modal {
    background: white;
    border-radius: 20px;
    padding: 2rem;
    max-width: 480px;
    width: 100%;
    max-height: 90vh;
    overflow-y: auto;
  }

  .modal h3 {
    font-family: 'Bebas Neue', cursive;
    font-size: 2rem;
    letter-spacing: 2px;
    margin-bottom: 1.5rem;
  }

  .form-group { margin-bottom: 1rem; }
  .form-group label {
    display: block;
    font-weight: 700;
    font-size: 0.85rem;
    margin-bottom: 5px;
    color: #555;
    letter-spacing: 0.5px;
  }
  .form-group input, .form-group select, .form-group textarea {
    width: 100%;
    padding: 11px 14px;
    border: 2px solid var(--border);
    border-radius: 10px;
    font-family: 'Nunito', sans-serif;
    font-size: 0.95rem;
    transition: border-color 0.2s;
    outline: none;
  }
  .form-group input:focus, .form-group select:focus, .form-group textarea:focus {
    border-color: var(--purple);
  }

  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 0.75rem; }

  .order-summary-mini {
    background: #f8f8f8;
    border-radius: 10px;
    padding: 1rem;
    margin-bottom: 1.5rem;
    font-size: 0.9rem;
  }

  .order-summary-mini .total-line {
    display: flex;
    justify-content: space-between;
    font-weight: 800;
    margin-top: 8px;
    padding-top: 8px;
    border-top: 1px solid var(--border);
  }

  .submit-order {
    width: 100%;
    padding: 14px;
    background: linear-gradient(135deg, var(--purple), var(--coral));
    color: white;
    border: none;
    border-radius: 12px;
    font-family: 'Nunito', sans-serif;
    font-weight: 800;
    font-size: 1.05rem;
    cursor: pointer;
    margin-top: 1rem;
    transition: transform 0.15s, box-shadow 0.15s;
  }
  .submit-order:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(91,62,200,0.4); }

  .close-modal-btn {
    background: none;
    border: none;
    color: #888;
    font-size: 0.9rem;
    cursor: pointer;
    font-family: 'Nunito', sans-serif;
    margin-top: 0.5rem;
    width: 100%;
    text-align: center;
  }

  /* SUCCESS */
  .success-modal { text-align: center; padding: 3rem 2rem; }
  .success-modal .check { font-size: 4rem; margin-bottom: 1rem; }
  .success-modal h3 { font-family: 'Bebas Neue', cursive; font-size: 2.5rem; color: var(--purple); letter-spacing: 2px; }
  .success-modal p { color: #666; margin: 0.5rem 0 1.5rem; }

  /* CONTACT */
  .contact-section {
    background: linear-gradient(135deg, var(--purple), var(--blue));
    padding: 4rem 2rem;
    text-align: center;
    color: white;
  }

  .contact-section h2 { font-family: 'Bebas Neue', cursive; font-size: 2.5rem; letter-spacing: 3px; margin-bottom: 0.5rem; }
  .contact-section p { opacity: 0.85; margin-bottom: 2rem; }

  .contact-btns { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }

  .contact-link {
    background: rgba(255,255,255,0.15);
    color: white;
    border: 2px solid rgba(255,255,255,0.3);
    padding: 12px 28px;
    border-radius: 25px;
    font-weight: 700;
    text-decoration: none;
    transition: background 0.2s, border-color 0.2s;
    font-size: 0.95rem;
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .contact-link:hover { background: rgba(255,255,255,0.25); border-color: white; }

  /* FOOTER */
  footer {
    background: var(--dark);
    color: #aaa;
    text-align: center;
    padding: 2rem;
    font-size: 0.85rem;
  }

  footer .footer-brand {
    font-family: 'Bebas Neue', cursive;
    font-size: 1.5rem;
    letter-spacing: 3px;
    background: linear-gradient(135deg, var(--purple), var(--blue), var(--coral));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 0.5rem;
  }

  /* ANIMATIONS */
  @keyframes fadeInDown {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  @keyframes marquee {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }

  /* RESPONSIVE */
  @media (max-width: 768px) {
    nav { display: none; }
    .insta-grid { grid-template-columns: repeat(2, 1fr); }
    .form-row { grid-template-columns: 1fr; }
    .product-grid { grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); }
  }
</style>
</head>
<body>

<!-- HEADER -->
<header>
  <div class="logo-area">
    <div class="logo-icon">
      <svg viewBox="0 0 60 60" fill="none" xmlns="http://www.w3.org/2000/svg">
        <circle cx="22" cy="28" r="18" fill="#5B3EC8" opacity="0.85"/>
        <circle cx="36" cy="28" r="18" fill="#3B8BEB" opacity="0.7"/>
        <circle cx="29" cy="38" r="14" fill="#E8556D" opacity="0.75"/>
        <!-- Pixel sneaker -->
        <rect x="16" y="24" width="4" height="4" fill="white"/>
        <rect x="20" y="20" width="4" height="4" fill="white"/>
        <rect x="24" y="18" width="4" height="4" fill="white"/>
        <rect x="28" y="20" width="4" height="4" fill="white"/>
        <rect x="32" y="22" width="4" height="4" fill="white"/>
        <rect x="14" y="28" width="24" height="4" fill="white"/>
        <rect x="18" y="32" width="20" height="3" fill="white" opacity="0.6"/>
      </svg>
    </div>
    <span class="logo-text">KicksxxlandRd</span>
  </div>
  <nav>
    <a href="#products">Shop</a>
    <a href="#instagram">Instagram</a>
    <a href="#contact">Contact</a>
  </nav>
  <button class="cart-btn" onclick="openCart()">
    🛒 Cart <span class="cart-count" id="cartCount">0</span>
  </button>
</header>

<!-- HERO -->
<div class="hero">
  <div class="hero-content">
    <div class="hero-badge">🔥 New Drops Available</div>
    <h1><span>Kicks</span>xx<span>land</span>Rd</h1>
    <p>donde el sueño del buen vestir se hace realidad</p>
    <div class="hero-btns">
      <a href="#products" class="btn-primary">Shop Now</a>
      <a href="https://www.instagram.com/kicksxxlandrd" target="_blank" class="btn-secondary">Follow Us</a>
    </div>
  </div>
</div>

<!-- MARQUEE -->
<div class="marquee-bar">
  <span class="marquee-inner">
    ✦ JORDAN 3 ✦ JORDAN 4 ✦ JORDAN 11 ✦ PUMA ✦ ADIDAS ✦ FREE SHIPPING ON ORDERS $150+ ✦ DM US FOR 
