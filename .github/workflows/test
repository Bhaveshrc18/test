<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>SortUs Eco – Crafted by Nature, Designed for Tomorrow</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Jost:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
  /* ─── TOKENS ─────────────────────────────────────────── */
  :root{
    --cream:#F7F2E9;
    --cream2:#EDE6D6;
    --bark:#6B4A2A;
    --bark-light:#A5784A;
    --forest:#2A4D2A;
    --forest-light:#3E7B3E;
    --terra:#C4622D;
    --terra-light:#E08050;
    --sage:#7A9E6A;
    --white:#FFFFFF;
    --text:#2C1E0F;
    --text-muted:#6B5B48;
    --border:#D9CDB8;
    --shadow:0 4px 24px rgba(44,30,15,.10);
    --shadow-lg:0 12px 48px rgba(44,30,15,.15);
    --radius:14px;
    --radius-sm:8px;
    --transition:.22s cubic-bezier(.4,0,.2,1);
  }
  *{box-sizing:border-box;margin:0;padding:0;}
  html{scroll-behavior:smooth;}
  body{
    font-family:'Jost',sans-serif;
    background:var(--cream);
    color:var(--text);
    min-height:100vh;
    overflow-x:hidden;
  }

  /* ─── NOISE TEXTURE OVERLAY ───────────────────────────── */
  body::before{
    content:'';
    position:fixed;inset:0;pointer-events:none;z-index:0;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='300'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.75' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='300' height='300' filter='url(%23n)' opacity='0.035'/%3E%3C/svg%3E");
    opacity:.5;
  }

  /* ─── SCROLLBAR ───────────────────────────────────────── */
  ::-webkit-scrollbar{width:6px;}
  ::-webkit-scrollbar-track{background:var(--cream2);}
  ::-webkit-scrollbar-thumb{background:var(--bark-light);border-radius:99px;}

  /* ─── ANNOUNCEMENT BAR ────────────────────────────────── */
  .announce{
    background:var(--forest);
    color:var(--cream);
    text-align:center;
    font-size:.78rem;
    letter-spacing:.08em;
    padding:.5rem 1rem;
    font-weight:500;
  }
  .announce a{color:var(--sage);text-decoration:none;}

  /* ─── HEADER ──────────────────────────────────────────── */
  header{
    background:var(--white);
    border-bottom:2px solid var(--cream2);
    position:sticky;top:0;z-index:900;
    box-shadow:0 2px 12px rgba(44,30,15,.07);
  }
  .header-inner{
    max-width:1200px;margin:0 auto;
    display:flex;align-items:center;justify-content:space-between;
    padding:.9rem 1.2rem;gap:1rem;
  }
  .logo-area{display:flex;flex-direction:column;line-height:1.1;}
  .logo-name{
    font-family:'Playfair Display',serif;
    font-size:1.6rem;font-weight:700;
    color:var(--forest);
    letter-spacing:-.01em;
  }
  .logo-name span{color:var(--terra);}
  .logo-tag{
    font-size:.65rem;letter-spacing:.14em;
    text-transform:uppercase;color:var(--text-muted);font-weight:500;
  }
  .header-right{display:flex;align-items:center;gap:.8rem;}
  .cart-btn{
    position:relative;background:var(--forest);
    border:none;border-radius:var(--radius-sm);
    color:var(--white);padding:.55rem 1.1rem .55rem .85rem;
    font-family:'Jost',sans-serif;font-size:.9rem;font-weight:600;
    cursor:pointer;display:flex;align-items:center;gap:.45rem;
    transition:background var(--transition);white-space:nowrap;
  }
  .cart-btn:hover{background:var(--forest-light);}
  .cart-btn svg{width:18px;height:18px;flex-shrink:0;}
  .cart-count{
    background:var(--terra);color:var(--white);
    font-size:.68rem;font-weight:700;
    border-radius:99px;padding:.1em .45em;
    min-width:18px;text-align:center;
  }

  /* ─── HERO BANNER ─────────────────────────────────────── */
  .hero{
    width:100%;overflow:hidden;position:relative;
    max-height:400px;
  }
  .hero img{
    width:100%;height:100%;object-fit:cover;
    display:block;max-height:400px;
  }
  .hero-overlay{
    position:absolute;inset:0;
    background:linear-gradient(to right,rgba(42,77,42,.72) 0%,rgba(42,77,42,.1) 70%);
    display:flex;flex-direction:column;justify-content:center;
    padding:2rem 2.5rem;
  }
  .hero-overlay h1{
    font-family:'Playfair Display',serif;
    color:var(--white);font-size:clamp(1.6rem,5vw,3rem);
    line-height:1.15;max-width:480px;
  }
  .hero-overlay h1 em{color:#B8D4A8;font-style:italic;}
  .hero-overlay p{
    color:rgba(255,255,255,.82);margin-top:.7rem;
    font-size:clamp(.85rem,2vw,1.05rem);max-width:360px;font-weight:300;
  }
  .hero-cta{
    display:inline-flex;align-items:center;gap:.4rem;
    margin-top:1.2rem;background:var(--terra);color:var(--white);
    padding:.62rem 1.3rem;border-radius:var(--radius-sm);
    font-weight:600;font-size:.9rem;text-decoration:none;
    transition:background var(--transition);width:fit-content;
  }
  .hero-cta:hover{background:var(--terra-light);}

  /* ─── SECTION TITLE ───────────────────────────────────── */
  .section-title{
    text-align:center;padding:2.2rem 1rem .6rem;
  }
  .section-title h2{
    font-family:'Playfair Display',serif;
    font-size:clamp(1.5rem,4vw,2.2rem);
    color:var(--forest);
  }
  .section-title p{
    color:var(--text-muted);font-size:.92rem;margin-top:.35rem;
  }
  .leaf-divider{
    display:flex;align-items:center;justify-content:center;gap:.6rem;
    margin:.6rem 0 1.4rem;
  }
  .leaf-divider::before,.leaf-divider::after{
    content:'';flex:1;max-width:80px;height:1px;background:var(--border);
  }
  .leaf-divider span{font-size:1rem;}

  /* ─── CATEGORY FILTERS ────────────────────────────────── */
  .filters{
    display:flex;gap:.5rem;overflow-x:auto;
    padding:.2rem 1rem 1rem;max-width:1200px;margin:0 auto;
    scrollbar-width:none;
    -ms-overflow-style:none;
  }
  .filters::-webkit-scrollbar{display:none;}
  .filter-btn{
    flex-shrink:0;padding:.45rem 1.1rem;
    border:1.5px solid var(--border);
    background:var(--white);border-radius:99px;
    font-family:'Jost',sans-serif;font-size:.82rem;font-weight:500;
    cursor:pointer;color:var(--text-muted);
    transition:all var(--transition);
  }
  .filter-btn.active,.filter-btn:hover{
    background:var(--forest);border-color:var(--forest);
    color:var(--white);
  }

  /* ─── PRODUCT GRID ────────────────────────────────────── */
  .products{
    display:grid;
    grid-template-columns:repeat(auto-fill,minmax(230px,1fr));
    gap:1.2rem;padding:0 1.2rem 2rem;
    max-width:1200px;margin:0 auto;
  }
  .card{
    background:var(--white);border-radius:var(--radius);
    overflow:hidden;box-shadow:var(--shadow);
    transition:transform var(--transition),box-shadow var(--transition);
    display:flex;flex-direction:column;
    animation:fadeUp .5s ease both;
  }
  @keyframes fadeUp{from{opacity:0;transform:translateY(22px);}to{opacity:1;transform:none;}}
  .card:hover{transform:translateY(-5px);box-shadow:var(--shadow-lg);}
  .card-img-wrap{
    position:relative;overflow:hidden;
    background:var(--cream2);aspect-ratio:1/1;
  }
  .card-img-wrap img{
    width:100%;height:100%;object-fit:cover;
    transition:transform .38s ease;display:block;
  }
  .card:hover .card-img-wrap img{transform:scale(1.06);}
  .card-badge{
    position:absolute;top:.6rem;left:.6rem;
    background:var(--sage);color:var(--white);
    font-size:.62rem;font-weight:600;letter-spacing:.06em;
    padding:.22em .6em;border-radius:4px;text-transform:uppercase;
  }
  .card-body{
    padding:1rem;flex:1;display:flex;flex-direction:column;gap:.35rem;
  }
  .card-cat{
    font-size:.68rem;letter-spacing:.1em;text-transform:uppercase;
    color:var(--bark-light);font-weight:600;
  }
  .card-name{
    font-family:'Playfair Display',serif;
    font-size:1rem;font-weight:600;color:var(--text);line-height:1.28;
  }
  .card-desc{
    font-size:.78rem;color:var(--text-muted);line-height:1.5;flex:1;
  }
  .card-footer{
    display:flex;align-items:center;justify-content:space-between;
    margin-top:.7rem;padding-top:.7rem;border-top:1px solid var(--cream2);
  }
  .card-price{
    font-size:1.1rem;font-weight:700;color:var(--forest);
    font-family:'Playfair Display',serif;
  }
  .add-btn{
    background:var(--terra);color:var(--white);
    border:none;border-radius:var(--radius-sm);
    padding:.42rem .85rem;font-size:.8rem;font-weight:600;
    font-family:'Jost',sans-serif;cursor:pointer;
    transition:background var(--transition),transform var(--transition);
  }
  .add-btn:hover{background:var(--terra-light);}
  .add-btn:active{transform:scale(.95);}
  .add-btn.added{background:var(--forest);}

  /* ─── CART DRAWER ─────────────────────────────────────── */
  .backdrop{
    display:none;position:fixed;inset:0;z-index:1000;
    background:rgba(44,30,15,.45);backdrop-filter:blur(2px);
  }
  .backdrop.open{display:block;}
  .drawer{
    position:fixed;top:0;right:0;height:100%;z-index:1010;
    width:min(420px,100vw);
    background:var(--white);
    box-shadow:-8px 0 40px rgba(44,30,15,.18);
    display:flex;flex-direction:column;
    transform:translateX(100%);
    transition:transform .32s cubic-bezier(.4,0,.2,1);
  }
  .drawer.open{transform:none;}
  .drawer-header{
    display:flex;align-items:center;justify-content:space-between;
    padding:1.2rem 1.4rem;border-bottom:2px solid var(--cream2);
    background:var(--forest);color:var(--white);
  }
  .drawer-header h3{
    font-family:'Playfair Display',serif;font-size:1.2rem;
  }
  .close-btn{
    background:none;border:none;color:var(--white);
    font-size:1.6rem;cursor:pointer;line-height:1;
  }
  .drawer-body{flex:1;overflow-y:auto;padding:1rem;}
  .empty-cart{
    text-align:center;padding:3rem 1rem;color:var(--text-muted);
  }
  .empty-cart svg{opacity:.3;margin-bottom:1rem;}
  .cart-item{
    display:grid;grid-template-columns:64px 1fr;gap:.8rem;
    padding:.9rem 0;border-bottom:1px solid var(--cream2);
    animation:fadeUp .25s ease;
  }
  .cart-item-img{
    width:64px;height:64px;object-fit:cover;
    border-radius:var(--radius-sm);border:1px solid var(--cream2);
  }
  .cart-item-info{display:flex;flex-direction:column;gap:.25rem;}
  .cart-item-name{
    font-size:.88rem;font-weight:600;color:var(--text);line-height:1.25;
  }
  .cart-item-price{font-size:.8rem;color:var(--text-muted);}
  .cart-item-controls{
    display:flex;align-items:center;justify-content:space-between;
    margin-top:.25rem;
  }
  .qty-controls{display:flex;align-items:center;gap:.4rem;}
  .qty-btn{
    background:var(--cream2);border:none;border-radius:5px;
    width:26px;height:26px;font-size:1rem;cursor:pointer;
    color:var(--text);display:flex;align-items:center;justify-content:center;
    font-weight:700;transition:background var(--transition);
  }
  .qty-btn:hover{background:var(--border);}
  .qty-val{font-size:.88rem;font-weight:600;min-width:18px;text-align:center;}
  .remove-btn{
    background:none;border:none;color:#C44;
    font-size:.72rem;cursor:pointer;font-weight:500;
    font-family:'Jost',sans-serif;
  }
  .cart-item-subtotal{font-size:.82rem;font-weight:700;color:var(--forest);}
  .drawer-footer{
    padding:1.2rem 1.4rem;border-top:2px solid var(--cream2);
    background:var(--cream);
  }
  .grand-total{
    display:flex;justify-content:space-between;align-items:center;
    margin-bottom:1rem;
  }
  .grand-total span:first-child{font-weight:500;color:var(--text-muted);}
  .grand-total strong{
    font-family:'Playfair Display',serif;font-size:1.35rem;color:var(--forest);
  }
  .checkout-btn{
    width:100%;background:var(--terra);color:var(--white);
    border:none;border-radius:var(--radius-sm);
    padding:.85rem;font-family:'Jost',sans-serif;
    font-size:.95rem;font-weight:700;cursor:pointer;
    letter-spacing:.04em;
    transition:background var(--transition);
  }
  .checkout-btn:hover{background:var(--terra-light);}

  /* ─── CHECKOUT MODAL ──────────────────────────────────── */
  .modal-overlay{
    display:none;position:fixed;inset:0;z-index:1100;
    background:rgba(44,30,15,.55);backdrop-filter:blur(4px);
    align-items:center;justify-content:center;padding:1rem;
  }
  .modal-overlay.open{display:flex;}
  .modal{
    background:var(--white);border-radius:var(--radius);
    width:100%;max-width:480px;max-height:90vh;overflow-y:auto;
    box-shadow:var(--shadow-lg);
    animation:popIn .3s cubic-bezier(.34,1.56,.64,1) both;
  }
  @keyframes popIn{from{opacity:0;transform:scale(.92);}to{opacity:1;transform:none;}}
  .modal-header{
    background:var(--forest);color:var(--white);
    padding:1.3rem 1.5rem;display:flex;justify-content:space-between;align-items:center;
    border-radius:var(--radius) var(--radius) 0 0;
  }
  .modal-header h3{font-family:'Playfair Display',serif;font-size:1.2rem;}
  .modal-body{padding:1.5rem;}
  .form-row{display:flex;flex-direction:column;gap:.35rem;margin-bottom:1.1rem;}
  .form-row label{font-size:.8rem;font-weight:600;color:var(--text-muted);letter-spacing:.05em;text-transform:uppercase;}
  .form-row input,.form-row textarea{
    border:1.5px solid var(--border);border-radius:var(--radius-sm);
    padding:.65rem .85rem;font-family:'Jost',sans-serif;font-size:.9rem;
    background:var(--cream);color:var(--text);
    transition:border var(--transition);outline:none;
    width:100%;
  }
  .form-row input:focus,.form-row textarea:focus{border-color:var(--forest);}
  .form-row textarea{min-height:80px;resize:vertical;}
  .order-summary-box{
    background:var(--cream2);border-radius:var(--radius-sm);
    padding:1rem;margin-bottom:1.2rem;
  }
  .order-summary-box h4{
    font-family:'Playfair Display',serif;font-size:.95rem;
    margin-bottom:.7rem;color:var(--forest);
  }
  .summary-row{display:flex;justify-content:space-between;font-size:.82rem;padding:.2rem 0;}
  .summary-row.total{font-weight:700;font-size:.92rem;border-top:1px solid var(--border);padding-top:.5rem;margin-top:.3rem;}
  .place-order-btn{
    width:100%;background:var(--terra);color:var(--white);
    border:none;border-radius:var(--radius-sm);
    padding:.9rem;font-family:'Jost',sans-serif;font-size:1rem;
    font-weight:700;cursor:pointer;letter-spacing:.04em;
    transition:background var(--transition);
  }
  .place-order-btn:hover{background:var(--terra-light);}

  /* ─── SUCCESS SCREEN ──────────────────────────────────── */
  .success-screen{
    text-align:center;padding:2.5rem 1.5rem;display:none;
  }
  .success-screen.show{display:block;}
  .success-icon{font-size:3.5rem;margin-bottom:.8rem;}
  .success-screen h3{
    font-family:'Playfair Display',serif;
    font-size:1.4rem;color:var(--forest);margin-bottom:.5rem;
  }
  .success-screen p{color:var(--text-muted);font-size:.9rem;margin-bottom:1.2rem;}
  .wa-link{
    display:inline-flex;align-items:center;gap:.5rem;
    background:#25D366;color:var(--white);
    padding:.7rem 1.5rem;border-radius:var(--radius-sm);
    text-decoration:none;font-weight:600;font-size:.9rem;
    transition:background var(--transition);
  }
  .wa-link:hover{background:#1ebe5b;}

  /* ─── FLOATING BUTTONS ────────────────────────────────── */
  .float-zone{
    position:fixed;bottom:1.5rem;right:1.2rem;z-index:800;
    display:flex;flex-direction:column;align-items:flex-end;gap:.7rem;
  }
  .float-cart{
    background:var(--forest);color:var(--white);
    width:54px;height:54px;border-radius:99px;border:none;
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 4px 18px rgba(42,77,42,.45);cursor:pointer;
    font-size:1.3rem;position:relative;
    transition:background var(--transition),transform var(--transition);
  }
  .float-cart:hover{background:var(--forest-light);transform:scale(1.08);}
  .float-cart-count{
    position:absolute;top:-4px;right:-4px;
    background:var(--terra);color:var(--white);
    font-size:.65rem;font-weight:700;border-radius:99px;
    padding:.1em .4em;min-width:18px;text-align:center;
    border:2px solid var(--white);
  }
  .float-wa{
    background:#25D366;color:var(--white);
    width:54px;height:54px;border-radius:99px;
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 4px 18px rgba(37,211,102,.4);
    text-decoration:none;font-size:1.5rem;
    transition:background var(--transition),transform var(--transition);
  }
  .float-wa:hover{background:#1ebe5b;transform:scale(1.08);}

  /* ─── TOAST ───────────────────────────────────────────── */
  .toast{
    position:fixed;bottom:6rem;right:1.2rem;z-index:1500;
    background:var(--forest);color:var(--white);
    padding:.7rem 1.1rem;border-radius:var(--radius-sm);
    font-size:.85rem;font-weight:500;
    box-shadow:var(--shadow);
    opacity:0;transform:translateY(10px);
    transition:all .25s ease;pointer-events:none;
  }
  .toast.show{opacity:1;transform:none;}

  /* ─── ABOUT STRIP ─────────────────────────────────────── */
  .about-strip{
    background:var(--forest);color:var(--cream);
    padding:2.5rem 1.5rem;margin-top:2rem;
    text-align:center;
  }
  .about-strip h3{
    font-family:'Playfair Display',serif;font-size:1.5rem;
    margin-bottom:.6rem;
  }
  .about-strip p{font-size:.88rem;opacity:.8;max-width:480px;margin:0 auto;}
  .about-perks{
    display:flex;flex-wrap:wrap;justify-content:center;gap:1.5rem;
    margin-top:1.6rem;
  }
  .perk{display:flex;flex-direction:column;align-items:center;gap:.3rem;}
  .perk span.icon{font-size:1.6rem;}
  .perk span.label{font-size:.75rem;letter-spacing:.07em;text-transform:uppercase;opacity:.75;}

  /* ─── FOOTER ──────────────────────────────────────────── */
  footer{
    background:var(--text);color:rgba(247,242,233,.7);
    padding:1.5rem 1.2rem;text-align:center;font-size:.8rem;
  }
  footer a{color:var(--sage);text-decoration:none;}
  footer strong{color:var(--cream);}

  /* ─── RESPONSIVE ──────────────────────────────────────── */
  @media(max-width:600px){
    .products{grid-template-columns:repeat(2,1fr);gap:.8rem;padding:0 .8rem 1.5rem;}
    .hero-overlay{padding:1.5rem;}
    .hero-cta{font-size:.8rem;padding:.5rem 1rem;}
    .drawer{width:100%;}
    .card-name{font-size:.9rem;}
    .card-body{padding:.8rem;}
  }
  @media(max-width:360px){
    .products{grid-template-columns:1fr;}
  }
</style>
</head>
<body>

<!-- ANNOUNCEMENT BAR -->
<div class="announce">
  🌿 Free consultation on bulk/gifting orders &nbsp;·&nbsp; Call us: <a href="tel:9322933545">9322933545</a>
</div>

<!-- HEADER -->
<header>
  <div class="header-inner">
    <div class="logo-area">
      <div class="logo-name">Sort<span>Us</span> Eco</div>
      <div class="logo-tag">Crafted by Nature, Designed for Tomorrow</div>
    </div>
    <div class="header-right">
      <button class="cart-btn" id="cartToggle" aria-label="Open cart">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <path d="M6 2L3 6v14a2 2 0 002 2h14a2 2 0 002-2V6l-3-4z"/><line x1="3" y1="6" x2="21" y2="6"/><path d="M16 10a4 4 0 01-8 0"/>
        </svg>
        Cart <span class="cart-count" id="cartCount">0</span>
      </button>
    </div>
  </div>
</header>

<!-- HERO BANNER -->
<section class="hero">
  <img src="https://i.ibb.co/prwS0ZRg/images.jpg" alt="SortUs Eco – Crafted by Nature" loading="eager"/>
  <div class="hero-overlay">
    <h1>Nature-Crafted <em>Cork</em> Products for Modern Living</h1>
    <p>Sustainable planters, desk accessories &amp; thoughtful gifts — made from nature's finest material.</p>
    <a class="hero-cta" href="#products">Shop Collection ↓</a>
  </div>
</section>

<!-- SECTION TITLE -->
<div class="section-title" id="products">
  <h2>Our Collection</h2>
  <p>Handpicked eco-friendly products for your home &amp; workspace</p>
</div>
<div class="leaf-divider"><span>🌿</span></div>

<!-- CATEGORY FILTERS -->
<div class="filters" id="filters">
  <button class="filter-btn active" data-cat="All">All</button>
  <button class="filter-btn" data-cat="Planters">Planters</button>
  <button class="filter-btn" data-cat="Desk Accessories">Desk Accessories</button>
  <button class="filter-btn" data-cat="Accessories">Accessories</button>
  <button class="filter-btn" data-cat="Gifts">Gifts</button>
  <button class="filter-btn" data-cat="Decoration">Decoration</button>
</div>

<!-- PRODUCT GRID -->
<div class="products" id="productGrid"></div>

<!-- ABOUT STRIP -->
<div class="about-strip">
  <h3>Why SortUs Eco?</h3>
  <p>We craft sustainable products from natural cork — a material that's harvested without harming trees, biodegradable, and beautifully unique.</p>
  <div class="about-perks">
    <div class="perk"><span class="icon">🌳</span><span class="label">Eco-Friendly</span></div>
    <div class="perk"><span class="icon">✋</span><span class="label">Handcrafted</span></div>
    <div class="perk"><span class="icon">📦</span><span class="label">Pune Delivery</span></div>
    <div class="perk"><span class="icon">💚</span><span class="label">Sustainable</span></div>
    <div class="perk"><span class="icon">🎁</span><span class="label">Gift-Ready</span></div>
  </div>
</div>

<!-- FOOTER -->
<footer>
  <p>
    <strong>SortUs Eco</strong> &nbsp;·&nbsp; Pune, Maharashtra &nbsp;·&nbsp;
    <a href="tel:9322933545">9322933545</a> &nbsp;·&nbsp;
    <a href="mailto:sortuseco@gmail.com">sortuseco@gmail.com</a>
  </p>
  <p style="margin-top:.4rem;opacity:.55;">© 2024 SortUs Eco. All rights reserved.</p>
</footer>

<!-- ─── CART DRAWER ─────────────────────────────────── -->
<div class="backdrop" id="backdrop"></div>
<div class="drawer" id="cartDrawer" role="dialog" aria-label="Shopping cart">
  <div class="drawer-header">
    <h3>🛒 Your Cart</h3>
    <button class="close-btn" id="closeCart" aria-label="Close cart">×</button>
  </div>
  <div class="drawer-body" id="cartBody">
    <div class="empty-cart" id="emptyCart">
      <svg width="56" height="56" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M6 2L3 6v14a2 2 0 002 2h14a2 2 0 002-2V6l-3-4z"/><line x1="3" y1="6" x2="21" y2="6"/><path d="M16 10a4 4 0 01-8 0"/></svg>
      <p>Your cart is empty.<br/>Add some nature to your life!</p>
    </div>
    <div id="cartItemsWrap"></div>
  </div>
  <div class="drawer-footer" id="cartFooter" style="display:none;">
    <div class="grand-total">
      <span>Grand Total</span>
      <strong id="grandTotal">₹0</strong>
    </div>
    <button class="checkout-btn" id="checkoutBtn">Proceed to Order →</button>
  </div>
</div>

<!-- ─── CHECKOUT MODAL ─────────────────────────────── -->
<div class="modal-overlay" id="checkoutModal">
  <div class="modal">
    <div class="modal-header">
      <h3>Place Your Order</h3>
      <button class="close-btn" id="closeModal">×</button>
    </div>
    <div class="modal-body" id="modalBody">
      <!-- Order summary injected by JS -->
      <div class="order-summary-box" id="modalSummary"></div>

      <!-- Formspree form -->
      <form id="orderForm" action="https://formspree.io/f/mkokggqv" method="POST">
        <!-- Hidden fields for email body -->
        <input type="hidden" name="_subject" id="f_subject"/>
        <input type="hidden" name="Order_Summary" id="f_summary"/>
        <input type="hidden" name="Grand_Total" id="f_total"/>

        <div class="form-row">
          <label>Full Name *</label>
          <input type="text" name="Customer_Name" id="f_name" placeholder="Your name" required/>
        </div>
        <div class="form-row">
          <label>Phone Number *</label>
          <input type="tel" name="Phone_Number" id="f_phone" placeholder="+91 XXXXX XXXXX" required/>
        </div>
        <div class="form-row">
          <label>Delivery Address *</label>
          <textarea name="Delivery_Address" id="f_address" placeholder="Flat / Street / Area, City, PIN" required></textarea>
        </div>
        <div class="form-row">
          <label>Special Instructions (optional)</label>
          <textarea name="Special_Instructions" id="f_notes" placeholder="Gift message, timing preference, etc."></textarea>
        </div>
        <button type="submit" class="place-order-btn" id="placeOrderBtn">🌿 Place Order</button>
      </form>

      <!-- Success screen -->
      <div class="success-screen" id="successScreen">
        <div class="success-icon">🎉</div>
        <h3>Order Placed Successfully!</h3>
        <p>Thank you! <strong>SortUs Eco</strong> will contact you on WhatsApp to confirm your order, availability &amp; delivery details.</p>
        <a class="wa-link" href="https://wa.me/919322933545" target="_blank" rel="noopener">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51a13 13 0 00-.57-.01c-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
          Chat on WhatsApp
        </a>
      </div>
    </div>
  </div>
</div>

<!-- ─── FLOATING BUTTONS ────────────────────────────── -->
<div class="float-zone">
  <a class="float-wa" href="https://wa.me/919322933545" target="_blank" rel="noopener" aria-label="Chat on WhatsApp">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51a13 13 0 00-.57-.01c-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
  </a>
  <button class="float-cart" id="floatCartBtn" aria-label="Open cart">
    🛒 <span class="float-cart-count" id="floatCount">0</span>
  </button>
</div>

<!-- TOAST -->
<div class="toast" id="toast"></div>

<script>
/* ═══════════════════════════════════════════════════════
   DATA
═══════════════════════════════════════════════════════ */
const PRODUCTS = [
  {id:1, name:"3 Hole Cork Table Planter with Glass Tubes", price:899, cat:"Planters", img:"https://i.ibb.co/qLsp3gDH/3-HOLE-CORK-TABLE-PLANTER-WITH-GLASS-TUBES-300x300.webp", desc:"Minimalist cork planter with triple glass tubes for hydro plants."},
  {id:2, name:"Holder Granco Cork Organizer", price:499, cat:"Desk Accessories", img:"https://i.ibb.co/G4sXtZRy/HOLDER-GRANCO-300x300.webp", desc:"Compact cork holder for organizing desk essentials neatly."},
  {id:3, name:"Cork Coin Holder Pouch", price:299, cat:"Accessories", img:"https://i.ibb.co/JFFzTGY4/CORK-COIN-HOLDER-POUCH-300x300.webp", desc:"Eco-friendly cork pouch ideal for coins and small items."},
  {id:4, name:"Cork Calendar with Eco Case", price:699, cat:"Desk Accessories", img:"https://i.ibb.co/PZXb436N/CORK-CALENDER-WITH-ECO-CASE-300x300.webp", desc:"Reusable cork calendar with sustainable protective case."},
  {id:5, name:"Bark Planter with Test Tube", price:799, cat:"Planters", img:"https://i.ibb.co/ZRRKrPhX/BARK-PLANTER-WITH-TEST-TUBE-300x300.webp", desc:"Rustic bark-style cork planter with single glass test tube."},
  {id:6, name:"Chocochip Printed Table Cork Planter", price:649, cat:"Planters", img:"https://i.ibb.co/SDg3jnCC/CHOCOCHIP-PRINTED-TABLE-CORK-PLANTER-300x300.webp", desc:"Stylish cork planter with unique chocochip print finish."},
  {id:7, name:"Box Print Cork Planter", price:599, cat:"Planters", img:"https://i.ibb.co/twRq7fxT/BOX-PRINT-CORK-PLANTER-300x300.webp", desc:"Modern box print cork planter for aesthetic desk décor."},
  {id:8, name:"Bohemian Print Cork Table Planter", price:699, cat:"Planters", img:"https://i.ibb.co/MDP34ybQ/BOHEMIAN-PRINT-CORK-TABLE-PLANTER-300x300.webp", desc:"Boho-style printed cork planter for vibrant interiors."},
  {id:9, name:"Abstract Texture Cork Table Planter", price:649, cat:"Planters", img:"https://i.ibb.co/JFn0KDS2/ASBTRACT-TEXTURE-CORK-TABLE-PLANTER-300x300.webp", desc:"Textured abstract design cork planter with premium finish."},
  {id:10, name:"Abstract Square Cork Planter", price:579, cat:"Planters", img:"https://i.ibb.co/sdCLLq33/ABSTRACT-SQUARE-CORK-PLANTER-300x300.webp", desc:"Square-shaped cork planter with modern abstract styling."},
  {id:11, name:"Cork Frame Planter with 3 Glass Beakers", price:999, cat:"Planters", img:"https://i.ibb.co/LXZfbFDB/CORK-FRAME-PLANTER-WITH-3-GLASS-BEAKERS-300x300.webp", desc:"Elegant cork frame planter featuring three glass beakers for propagation."},
  {id:12, name:"Cork Ice Bucket", price:2000, cat:"Gifts", img:"https://i.ibb.co/yFmvCxWj/CORK-ICE-BUCKET-WITH-REMOVABLE-STAINLESS-STEEL-TUB-300x300.webp", desc:"Premium cork exterior with removable stainless steel inner tub."},
];

/* ═══════════════════════════════════════════════════════
   STATE
═══════════════════════════════════════════════════════ */
let cart = JSON.parse(localStorage.getItem('sortuseco_cart') || '[]');
let activeFilter = 'All';

function saveCart(){ localStorage.setItem('sortuseco_cart', JSON.stringify(cart)); }

/* ═══════════════════════════════════════════════════════
   RENDER PRODUCTS
═══════════════════════════════════════════════════════ */
function renderProducts(){
  const grid = document.getElementById('productGrid');
  const filtered = activeFilter === 'All' ? PRODUCTS : PRODUCTS.filter(p => p.cat === activeFilter);
  grid.innerHTML = '';
  filtered.forEach((p, i) => {
    const inCart = cart.find(c => c.id === p.id);
    const card = document.createElement('div');
    card.className = 'card';
    card.style.animationDelay = (i * 0.06) + 's';
    card.innerHTML = `
      <div class="card-img-wrap">
        <img src="${p.img}" alt="${p.name}" loading="lazy"/>
        <span class="card-badge">${p.cat}</span>
      </div>
      <div class="card-body">
        <div class="card-cat">${p.cat}</div>
        <div class="card-name">${p.name}</div>
        <div class="card-desc">${p.desc}</div>
        <div class="card-footer">
          <div class="card-price">₹${p.price.toLocaleString('en-IN')}</div>
          <button class="add-btn${inCart?' added':''}" data-id="${p.id}">
            ${inCart ? '✓ Added' : '+ Add'}
          </button>
        </div>
      </div>`;
    grid.appendChild(card);
  });
  // Attach add to cart listeners
  grid.querySelectorAll('.add-btn').forEach(btn => {
    btn.addEventListener('click', () => addToCart(+btn.dataset.id));
  });
}

/* ═══════════════════════════════════════════════════════
   CART LOGIC
═══════════════════════════════════════════════════════ */
function addToCart(id){
  const product = PRODUCTS.find(p => p.id === id);
  const existing = cart.find(c => c.id === id);
  if(existing){
    existing.qty++;
    showToast(`+1 ${product.name.split(' ').slice(0,3).join(' ')}…`);
  } else {
    cart.push({...product, qty:1});
    showToast(`Added: ${product.name.split(' ').slice(0,4).join(' ')}…`);
  }
  saveCart();
  renderProducts();
  updateCounts();
  renderCartItems();
}

function removeFromCart(id){
  cart = cart.filter(c => c.id !== id);
  saveCart();
  renderProducts();
  updateCounts();
  renderCartItems();
}

function changeQty(id, delta){
  const item = cart.find(c => c.id === id);
  if(!item) return;
  item.qty += delta;
  if(item.qty <= 0) { removeFromCart(id); return; }
  saveCart();
  updateCounts();
  renderCartItems();
  renderProducts();
}

function getTotal(){
  return cart.reduce((s, c) => s + c.price * c.qty, 0);
}

function updateCounts(){
  const count = cart.reduce((s,c)=>s+c.qty,0);
  document.getElementById('cartCount').textContent = count;
  document.getElementById('floatCount').textContent = count;
}

/* ═══════════════════════════════════════════════════════
   RENDER CART ITEMS
═══════════════════════════════════════════════════════ */
function renderCartItems(){
  const wrap = document.getElementById('cartItemsWrap');
  const empty = document.getElementById('emptyCart');
  const footer = document.getElementById('cartFooter');
  const total = document.getElementById('grandTotal');
  wrap.innerHTML = '';
  if(cart.length === 0){
    empty.style.display = 'block';
    footer.style.display = 'none';
    return;
  }
  empty.style.display = 'none';
  footer.style.display = 'block';
  cart.forEach(item => {
    const div = document.createElement('div');
    div.className = 'cart-item';
    div.innerHTML = `
      <img class="cart-item-img" src="${item.img}" alt="${item.name}" loading="lazy"/>
      <div class="cart-item-info">
        <div class="cart-item-name">${item.name}</div>
        <div class="cart-item-price">₹${item.price.toLocaleString('en-IN')} each</div>
        <div class="cart-item-controls">
          <div class="qty-controls">
            <button class="qty-btn" data-id="${item.id}" data-delta="-1">−</button>
            <span class="qty-val">${item.qty}</span>
            <button class="qty-btn" data-id="${item.id}" data-delta="1">+</button>
          </div>
          <span class="cart-item-subtotal">₹${(item.price*item.qty).toLocaleString('en-IN')}</span>
        </div>
        <button class="remove-btn" data-id="${item.id}">Remove</button>
      </div>`;
    wrap.appendChild(div);
  });
  total.textContent = '₹' + getTotal().toLocaleString('en-IN');
  wrap.querySelectorAll('.qty-btn').forEach(b => {
    b.addEventListener('click', () => changeQty(+b.dataset.id, +b.dataset.delta));
  });
  wrap.querySelectorAll('.remove-btn').forEach(b => {
    b.addEventListener('click', () => removeFromCart(+b.dataset.id));
  });
}

/* ═══════════════════════════════════════════════════════
   DRAWER OPEN/CLOSE
═══════════════════════════════════════════════════════ */
function openCart(){
  renderCartItems();
  document.getElementById('cartDrawer').classList.add('open');
  document.getElementById('backdrop').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeCart(){
  document.getElementById('cartDrawer').classList.remove('open');
  document.getElementById('backdrop').classList.remove('open');
  document.body.style.overflow = '';
}

document.getElementById('cartToggle').addEventListener('click', openCart);
document.getElementById('closeCart').addEventListener('click', closeCart);
document.getElementById('backdrop').addEventListener('click', closeCart);
document.getElementById('floatCartBtn').addEventListener('click', openCart);

/* ═══════════════════════════════════════════════════════
   CHECKOUT MODAL
═══════════════════════════════════════════════════════ */
function buildModalSummary(){
  const box = document.getElementById('modalSummary');
  box.innerHTML = '<h4>📦 Order Summary</h4>';
  cart.forEach(item => {
    const row = document.createElement('div');
    row.className = 'summary-row';
    row.innerHTML = `<span>${item.name} × ${item.qty}</span><span>₹${(item.price*item.qty).toLocaleString('en-IN')}</span>`;
    box.appendChild(row);
  });
  const total = document.createElement('div');
  total.className = 'summary-row total';
  total.innerHTML = `<span>Grand Total</span><strong>₹${getTotal().toLocaleString('en-IN')}</strong>`;
  box.appendChild(total);
}

function populateHiddenFields(){
  let summary = '';
  cart.forEach(item => {
    summary += `${item.name} x${item.qty} = ₹${(item.price*item.qty).toLocaleString('en-IN')}\n`;
  });
  summary += `\nGrand Total: ₹${getTotal().toLocaleString('en-IN')}`;
  document.getElementById('f_summary').value = summary;
  document.getElementById('f_total').value = '₹' + getTotal().toLocaleString('en-IN');
  document.getElementById('f_subject').value = `New Order from SortUs Eco – ₹${getTotal().toLocaleString('en-IN')}`;
}

document.getElementById('checkoutBtn').addEventListener('click', () => {
  if(cart.length === 0) return;
  closeCart();
  buildModalSummary();
  populateHiddenFields();
  document.getElementById('checkoutModal').classList.add('open');
  document.getElementById('orderForm').style.display = 'block';
  document.getElementById('successScreen').classList.remove('show');
});

document.getElementById('closeModal').addEventListener('click', () => {
  document.getElementById('checkoutModal').classList.remove('open');
});
document.getElementById('checkoutModal').addEventListener('click', e => {
  if(e.target === e.currentTarget) e.currentTarget.classList.remove('open');
});

/* ═══════════════════════════════════════════════════════
   FORM SUBMIT (Formspree)
═══════════════════════════════════════════════════════ */
document.getElementById('orderForm').addEventListener('submit', async function(e){
  e.preventDefault();
  const btn = document.getElementById('placeOrderBtn');
  btn.textContent = 'Sending…';
  btn.disabled = true;
  populateHiddenFields();
  try{
    const resp = await fetch(this.action, {
      method:'POST',
      headers:{'Accept':'application/json'},
      body: new FormData(this)
    });
    if(resp.ok){
      this.style.display = 'none';
      document.getElementById('modalSummary').style.display = 'none';
      document.getElementById('successScreen').classList.add('show');
      cart = [];
      saveCart();
      updateCounts();
    } else {
      btn.textContent = 'Try Again';
      btn.disabled = false;
      showToast('⚠ Could not send. Please try again.');
    }
  } catch(err){
    btn.textContent = 'Try Again';
    btn.disabled = false;
    showToast('⚠ Network error. Please retry.');
  }
});

/* ═══════════════════════════════════════════════════════
   CATEGORY FILTER
═══════════════════════════════════════════════════════ */
document.getElementById('filters').addEventListener('click', e => {
  if(!e.target.matches('.filter-btn')) return;
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  e.target.classList.add('active');
  activeFilter = e.target.dataset.cat;
  renderProducts();
});

/* ═══════════════════════════════════════════════════════
   TOAST
═══════════════════════════════════════════════════════ */
let toastTimer;
function showToast(msg){
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => t.classList.remove('show'), 2000);
}

/* ═══════════════════════════════════════════════════════
   INIT
═══════════════════════════════════════════════════════ */
renderProducts();
updateCounts();
</script>
</body>
</html>
