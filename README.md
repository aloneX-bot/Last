<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CONSCIOUS CHEMIST — Your Beauty Is In Your Hands</title>
<meta name="description" content="Conscious Chemist — modern skincare for your everyday ritual.">

<style>
:root{
  --cream:#f8f6ef;
  --white:#ffffff;
  --green:#173c2b;
  --green2:#245b42;
  --sage:#dfe9df;
  --text:#18221d;
  --muted:#6d756f;
  --line:#e3e5df;
  --accent:#c6d8bf;
  --danger:#a33c3c;
  --shadow:0 12px 35px rgba(23,60,43,.09);
  --radius:22px;
}

*{box-sizing:border-box;margin:0;padding:0}

html{scroll-behavior:smooth}

body{
  font-family:Arial,Helvetica,sans-serif;
  background:var(--cream);
  color:var(--text);
  line-height:1.5;
}

button,input,textarea,select{font:inherit}

button{cursor:pointer}

a{text-decoration:none;color:inherit}

img{
  display:block;
  width:100%;
}

.container{
  width:min(1180px,92%);
  margin:auto;
}

/* HEADER */

header{
  position:sticky;
  top:0;
  z-index:1000;
  background:rgba(248,246,239,.95);
  backdrop-filter:blur(15px);
  border-bottom:1px solid var(--line);
}

.nav{
  min-height:76px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:25px;
}

.logo{
  font-weight:900;
  letter-spacing:2px;
  font-size:19px;
  color:var(--green);
}

.logo span{
  display:block;
  font-size:9px;
  letter-spacing:3px;
  font-weight:600;
  color:var(--muted);
  margin-top:-2px;
}

.navlinks{
  display:flex;
  gap:28px;
  font-size:14px;
  font-weight:600;
}

.navlinks a:hover{color:var(--green2)}

.nav-actions{
  display:flex;
  align-items:center;
  gap:10px;
}

.icon-btn{
  width:43px;
  height:43px;
  border:1px solid var(--line);
  background:white;
  border-radius:50%;
  display:grid;
  place-items:center;
  font-size:18px;
  position:relative;
}

.cart-count{
  position:absolute;
  right:-3px;
  top:-3px;
  width:19px;
  height:19px;
  border-radius:50%;
  background:var(--green);
  color:white;
  font-size:10px;
  display:grid;
  place-items:center;
  font-weight:bold;
}

.menu-btn{display:none}

/* HERO */

.hero{
  padding:55px 0 70px;
}

.hero-box{
  min-height:530px;
  border-radius:32px;
  overflow:hidden;
  background:
    linear-gradient(90deg,rgba(12,38,27,.86),rgba(12,38,27,.25)),
    url("https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=1800&q=85")
    center/cover;
  display:flex;
  align-items:center;
  padding:70px;
  color:white;
}

.hero-content{
  max-width:600px;
}

.eyebrow{
  text-transform:uppercase;
  letter-spacing:3px;
  font-size:11px;
  font-weight:800;
  margin-bottom:14px;
}

.hero h1{
  font-family:Georgia,serif;
  font-size:clamp(42px,6vw,76px);
  line-height:1.02;
  margin-bottom:22px;
}

.hero p{
  font-size:17px;
  max-width:520px;
  color:rgba(255,255,255,.86);
  margin-bottom:30px;
}

.primary{
  border:0;
  background:var(--green);
  color:white;
  padding:14px 23px;
  border-radius:100px;
  font-weight:700;
  transition:.2s;
}

.primary:hover{
  background:var(--green2);
  transform:translateY(-2px);
}

.hero .primary{
  background:white;
  color:var(--green);
}

/* FEATURES */

.features{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
  margin-bottom:80px;
}

.feature{
  background:white;
  padding:22px;
  border-radius:18px;
  border:1px solid var(--line);
}

.feature-icon{
  font-size:23px;
  margin-bottom:8px;
}

.feature strong{
  display:block;
  font-size:14px;
}

.feature span{
  font-size:12px;
  color:var(--muted);
}

/* SECTION */

.section{
  padding:20px 0 85px;
}

.section-head{
  display:flex;
  justify-content:space-between;
  align-items:end;
  gap:20px;
  margin-bottom:28px;
}

.section-head h2{
  font-family:Georgia,serif;
  font-size:40px;
}

.section-head p{
  color:var(--muted);
  font-size:14px;
}

.view-all{
  color:var(--green);
  font-weight:700;
  font-size:14px;
}

/* PRODUCTS */

.products{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:22px;
}

.product{
  background:white;
  border:1px solid var(--line);
  border-radius:var(--radius);
  overflow:hidden;
  transition:.25s;
}

.product:hover{
  transform:translateY(-5px);
  box-shadow:var(--shadow);
}

.product-img{
  position:relative;
  aspect-ratio:1/1.08;
  background:#edf0e9;
  overflow:hidden;
  cursor:pointer;
}

.product-img img{
  height:100%;
  object-fit:cover;
  transition:.4s;
}

.product:hover .product-img img{
  transform:scale(1.04);
}

.badge{
  position:absolute;
  top:13px;
  left:13px;
  background:white;
  color:var(--green);
  border-radius:50px;
  padding:6px 10px;
  font-size:10px;
  font-weight:800;
}

.product-info{
  padding:17px;
}

.category{
  color:var(--muted);
  text-transform:uppercase;
  letter-spacing:1.5px;
  font-size:9px;
  font-weight:700;
}

.product-name{
  font-family:Georgia,serif;
  font-size:19px;
  margin:5px 0 8px;
}

.product-desc{
  font-size:12px;
  color:var(--muted);
  min-height:38px;
}

.price-row{
  display:flex;
  align-items:center;
  justify-content:space-between;
  margin-top:15px;
}

.price{
  font-weight:800;
  color:var(--green);
}

.add{
  width:37px;
  height:37px;
  border-radius:50%;
  background:var(--green);
  color:white;
  border:0;
  font-size:21px;
}

/* ABOUT */

.about{
  background:var(--green);
  color:white;
  padding:80px 0;
  margin:20px 0 80px;
}

.about-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:70px;
  align-items:center;
}

.about h2{
  font-family:Georgia,serif;
  font-size:48px;
  line-height:1.1;
  margin-bottom:20px;
}

.about p{
  color:rgba(255,255,255,.72);
  margin-bottom:15px;
}

.about-img{
  border-radius:28px;
  overflow:hidden;
  height:430px;
}

.about-img img{
  height:100%;
  object-fit:cover;
}

/* FOOTER */

footer{
  background:#10291e;
  color:white;
  padding:55px 0 25px;
}

.footer-grid{
  display:grid;
  grid-template-columns:2fr 1fr 1fr;
  gap:50px;
}

.footer-title{
  font-family:Georgia,serif;
  font-size:22px;
  margin-bottom:15px;
}

footer p,footer a{
  color:rgba(255,255,255,.62);
  font-size:13px;
}

footer a{
  display:block;
  margin:8px 0;
}

.copyright{
  border-top:1px solid rgba(255,255,255,.1);
  margin-top:45px;
  padding-top:20px;
  font-size:11px;
  color:rgba(255,255,255,.45);
}

/* DRAWER */

.overlay{
  position:fixed;
  inset:0;
  background:rgba(0,0,0,.45);
  z-index:1500;
  display:none;
}

.overlay.active{display:block}

.drawer{
  position:fixed;
  z-index:1600;
  top:0;
  right:-450px;
  width:min(440px,94%);
  height:100%;
  background:white;
  transition:.3s;
  padding:25px;
  display:flex;
  flex-direction:column;
}

.drawer.active{right:0}

.drawer-head{
  display:flex;
  align-items:center;
  justify-content:space-between;
  padding-bottom:20px;
  border-bottom:1px solid var(--line);
}

.drawer h2{
  font-family:Georgia,serif;
}

.close{
  border:0;
  background:#f1f2ed;
  width:37px;
  height:37px;
  border-radius:50%;
  font-size:20px;
}

.cart-items{
  flex:1;
  overflow:auto;
  padding:18px 0;
}

.cart-item{
  display:grid;
  grid-template-columns:65px 1fr auto;
  gap:12px;
  align-items:center;
  padding:12px 0;
  border-bottom:1px solid var(--line);
}

.cart-item img{
  width:65px;
  height:75px;
  object-fit:cover;
  border-radius:12px;
}

.cart-item h4{
  font-family:Georgia,serif;
  font-size:15px;
}

.cart-item p{
  font-size:12px;
  color:var(--muted);
}

.qty{
  display:flex;
  align-items:center;
  gap:8px;
  margin-top:7px;
}

.qty button{
  width:25px;
  height:25px;
  border:1px solid var(--line);
  background:white;
  border-radius:50%;
}

.remove{
  color:var(--danger);
  border:0;
  background:none;
  font-size:11px;
}

.cart-bottom{
  border-top:1px solid var(--line);
  padding-top:18px;
}

.total-row{
  display:flex;
  justify-content:space-between;
  font-weight:800;
  margin-bottom:15px;
}

.full{
  width:100%;
}

/* MODAL */

.modal-wrap{
  position:fixed;
  inset:0;
  z-index:2000;
  display:none;
  place-items:center;
  background:rgba(0,0,0,.52);
  padding:20px;
}

.modal-wrap.active{display:grid}

.modal{
  width:min(980px,100%);
  max-height:92vh;
  overflow:auto;
  background:white;
  border-radius:28px;
  position:relative;
}

.modal-close{
  position:absolute;
  right:17px;
  top:17px;
  z-index:5;
  width:40px;
  height:40px;
  border:0;
  background:white;
  border-radius:50%;
  font-size:20px;
  box-shadow:0 5px 20px rgba(0,0,0,.1);
}

.product-detail{
  display:grid;
  grid-template-columns:1fr 1fr;
}

.gallery-main{
  aspect-ratio:1/1;
  overflow:hidden;
  background:#eef0ea;
}

.gallery-main img{
  height:100%;
  object-fit:cover;
}

.thumbs{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:8px;
  padding:10px;
}

.thumb{
  aspect-ratio:1;
  border:2px solid transparent;
  border-radius:10px;
  overflow:hidden;
  cursor:pointer;
}

.thumb.active{border-color:var(--green)}

.detail-info{
  padding:55px 40px 40px;
}

.detail-info .category{
  margin-bottom:8px;
}

.detail-info h2{
  font-family:Georgia,serif;
  font-size:40px;
  line-height:1.05;
  margin-bottom:15px;
}

.detail-price{
  font-size:25px;
  color:var(--green);
  font-weight:800;
  margin-bottom:22px;
}

.detail-description{
  color:var(--muted);
  font-size:14px;
  margin-bottom:22px;
}

.details-list{
  border-top:1px solid var(--line);
  border-bottom:1px solid var(--line);
  padding:15px 0;
  margin-bottom:22px;
}

.details-list div{
  display:flex;
  gap:8px;
  font-size:12px;
  margin:7px 0;
}

.details-list strong{min-width:95px}

.detail-actions{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:10px;
}

.secondary{
  border:1px solid var(--green);
  background:white;
  color:var(--green);
  padding:14px 20px;
  border-radius:100px;
  font-weight:700;
}

/* CHECKOUT */

.checkout-modal{
  width:min(760px,100%);
  max-height:94vh;
  overflow:auto;
  background:white;
  border-radius:28px;
  padding:35px;
  position:relative;
}

.checkout-modal h2{
  font-family:Georgia,serif;
  font-size:38px;
  margin-bottom:7px;
}

.checkout-note{
  color:var(--muted);
  font-size:13px;
  margin-bottom:25px;
}

.checkout-summary{
  background:var(--cream);
  border-radius:17px;
  padding:15px;
  margin-bottom:22px;
}

.summary-line{
  display:flex;
  justify-content:space-between;
  gap:15px;
  font-size:13px;
  margin:6px 0;
}

.summary-total{
  border-top:1px solid var(--line);
  margin-top:10px;
  padding-top:10px;
  font-weight:800;
}

.form-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:15px;
}

.field{
  display:flex;
  flex-direction:column;
  gap:6px;
  margin-bottom:14px;
}

.field.full-field{grid-column:1/-1}

.field label{
  font-size:12px;
  font-weight:700;
}

.field input,.field textarea,.field select{
  border:1px solid #dfe2db;
  background:#fafbf8;
  padding:13px;
  border-radius:12px;
  outline:none;
}

.field input:focus,.field textarea:focus{
  border-color:var(--green);
}

.field textarea{
  resize:vertical;
  min-height:90px;
}

/* SUCCESS */

.success{
  text-align:center;
  padding:55px 30px;
}

.success-icon{
  width:70px;
  height:70px;
  border-radius:50%;
  background:var(--sage);
  color:var(--green);
  display:grid;
  place-items:center;
  font-size:32px;
  margin:0 auto 20px;
}

.success h2{
  font-family:Georgia,serif;
  font-size:40px;
  margin-bottom:10px;
}

.success p{
  color:var(--muted);
  max-width:450px;
  margin:0 auto 25px;
}

.order-id{
  background:var(--cream);
  display:inline-block;
  padding:10px 15px;
  border-radius:10px;
  font-weight:800;
  color:var(--green);
}

/* TOAST */

.toast{
  position:fixed;
  z-index:5000;
  left:50%;
  bottom:25px;
  transform:translate(-50%,30px);
  background:var(--green);
  color:white;
  padding:13px 20px;
  border-radius:100px;
  font-size:13px;
  opacity:0;
  pointer-events:none;
  transition:.3s;
}

.toast.show{
  opacity:1;
  transform:translate(-50%,0);
}

/* EMPTY */

.empty{
  text-align:center;
  color:var(--muted);
  padding:50px 10px;
}

/* RESPONSIVE */

@media(max-width:950px){
  .products{grid-template-columns:repeat(3,1fr)}
  .features{grid-template-columns:repeat(2,1fr)}
  .hero-box{padding:50px}
}

@media(max-width:700px){
  .navlinks{display:none}
  .menu-btn{display:grid}

  .hero{
    padding:20px 0 50px;
  }

  .hero-box{
    min-height:540px;
    padding:35px 25px;
    border-radius:24px;
    align-items:end;
  }

  .hero h1{font-size:45px}

  .products{
    grid-template-columns:repeat(2,1fr);
    gap:12px;
  }

  .product-info{padding:13px}

  .product-name{font-size:16px}

  .product-desc{font-size:11px}

  .about{
    padding:55px 0;
  }

  .about-grid{
    grid-template-columns:1fr;
    gap:30px;
  }

  .about h2{font-size:39px}

  .about-img{height:300px}

  .footer-grid{
    grid-template-columns:1fr;
    gap:25px;
  }

  .product-detail{
    grid-template-columns:1fr;
  }

  .detail-info{
    padding:25px;
  }

  .detail-info h2{
    font-size:32px;
  }

  .form-grid{
    grid-template-columns:1fr;
  }

  .field.full-field{
    grid-column:auto;
  }

  .checkout-modal{
    padding:25px 18px;
  }
}

@media(max-width:430px){
  .features{
    grid-template-columns:1fr;
  }

  .section-head h2{
    font-size:31px;
  }

  .products{
    grid-template-columns:1fr 1fr;
  }

  .badge{
    font-size:8px;
  }

  .detail-actions{
    grid-template-columns:1fr;
  }
}
</style>
</head>

<body>

<header>
  <div class="container nav">
    <a href="#" class="logo">
      CONSCIOUS CHEMIST
      <span>YOUR BEAUTY IS IN YOUR HANDS</span>
    </a>

    <nav class="navlinks">
      <a href="#shop">Shop</a>
      <a href="#about">About</a>
      <a href="#why">Why Us</a>
    </nav>

    <div class="nav-actions">
      <button class="icon-btn menu-btn" onclick="document.getElementById('shop').scrollIntoView()">☰</button>

      <button class="icon-btn" onclick="openCart()" aria-label="Open cart">
        🛒
        <span class="cart-count" id="cartCount">0</span>
      </button>
    </div>
  </div>
</header>

<main>

<section class="hero">
  <div class="container">
    <div class="hero-box">
      <div class="hero-content">
        <div class="eyebrow">Conscious skincare</div>
        <h1>Your skin.<br>Your ritual.</h1>
        <p>
          Thoughtfully designed skincare made for everyday routines.
          Simple formulas, beautiful textures and products you will
          actually want to use.
        </p>
        <button class="primary" onclick="document.getElementById('shop').scrollIntoView()">
          Explore Collection →
        </button>
      </div>
    </div>
  </div>
</section>

<section class="container features" id="why">
  <div class="feature">
    <div class="feature-icon">🌿</div>
    <strong>Thoughtful Formulas</strong>
    <span>Designed around modern skincare routines.</span>
  </div>

  <div class="feature">
    <div class="feature-icon">✨</div>
    <strong>Everyday Essentials</strong>
    <span>Simple products for consistent care.</span>
  </div>

  <div class="feature">
    <div class="feature-icon">💧</div>
    <strong>Skin First</strong>
    <span>Comfortable textures made for daily use.</span>
  </div>

  <div class="feature">
    <div class="feature-icon">📦</div>
    <strong>Easy Ordering</strong>
    <span>Order online without complicated checkout.</span>
  </div>
</section>

<section class="container section" id="shop">
  <div class="section-head">
    <div>
      <div class="eyebrow">The collection</div>
      <h2>Shop skincare</h2>
      <p>Discover your new everyday essentials.</p>
    </div>
    <span class="view-all">12 products</span>
  </div>

  <div class="products" id="productsGrid"></div>
</section>

<section class="about" id="about">
  <div class="container about-grid">
    <div>
      <div class="eyebrow">Our philosophy</div>
      <h2>Beautiful skincare shouldn't be complicated.</h2>
      <p>
        CONSCIOUS CHEMIST is built around a simple idea:
        skincare should fit naturally into your everyday life.
      </p>
      <p>
        From cleansing to hydration and sun protection,
        every product is designed to make your routine feel
        simple, intentional and enjoyable.
      </p>
    </div>

    <div class="about-img">
      <img
        src="https://images.unsplash.com/photo-1556229010-6c3f2c9ca5f8?auto=format&fit=crop&w=1000&q=85"
        alt="Skincare products"
      >
    </div>
  </div>
</section>

</main>

<footer>
  <div class="container footer-grid">
    <div>
      <div class="footer-title">CONSCIOUS CHEMIST</div>
      <p>Your beauty is in your hands.</p>
      <p style="margin-top:10px">
        Thoughtful skincare for your everyday ritual.
      </p>
    </div>

    <div>
      <div class="footer-title">Shop</div>
      <a href="#shop">All Products</a>
      <a href="#shop">Cleansers</a>
      <a href="#shop">Serums</a>
      <a href="#shop">Moisturizers</a>
    </div>

    <div>
      <div class="footer-title">Help</div>
      <a href="#">Shipping</a>
      <a href="#">Returns</a>
      <a href="#">Contact</a>
      <a href="#">Privacy</a>
    </div>
  </div>

  <div class="container copyright">
    © 2026 CONSCIOUS CHEMIST. All rights reserved.
  </div>
</footer>


<!-- CART -->

<div class="overlay" id="overlay" onclick="closeCart()"></div>

<aside class="drawer" id="cartDrawer">
  <div class="drawer-head">
    <h2>Your Cart</h2>
    <button class="close" onclick="closeCart()">×</button>
  </div>

  <div class="cart-items" id="cartItems"></div>

  <div class="cart-bottom">
    <div class="total-row">
      <span>Total</span>
      <span id="cartTotal">₹0</span>
    </div>

    <button class="primary full" onclick="openCheckout()">
      Proceed to Checkout →
    </button>
  </div>
</aside>


<!-- PRODUCT MODAL -->

<div class="modal-wrap" id="productModal">
  <div class="modal">
    <button class="modal-close" onclick="closeProduct()">×</button>

    <div class="product-detail">

      <div>
        <div class="gallery-main">
          <img id="detailMainImage" src="" alt="">
        </div>
        <div class="thumbs" id="detailThumbs"></div>
      </div>

      <div class="detail-info">
        <div class="category" id="detailCategory"></div>
        <h2 id="detailName"></h2>
        <div class="detail-price" id="detailPrice"></div>
        <p class="detail-description" id="detailDescription"></p>

        <div class="details-list">
          <div>
            <strong>Skin type</strong>
            <span id="detailSkin"></span>
          </div>
          <div>
            <strong>Texture</strong>
            <span id="detailTexture"></span>
          </div>
          <div>
            <strong>Size</strong>
            <span id="detailSize"></span>
          </div>
        </div>

        <div class="detail-actions">
          <button class="secondary" id="detailCartButton">
            Add to Cart
          </button>

          <button class="primary" id="detailBuyButton">
            Buy Now
          </button>
        </div>
      </div>

    </div>
  </div>
</div>


<!-- CHECKOUT -->

<div class="modal-wrap" id="checkoutModal">
  <div class="checkout-modal">

    <button class="modal-close" onclick="closeCheckout()">×</button>

    <div id="checkoutContent">

      <div class="eyebrow">Secure order</div>
      <h2>Complete your order</h2>
      <p class="checkout-note">
        No online payment is required. Submit your details and
        we will receive your order.
      </p>

      <div class="checkout-summary" id="checkoutSummary"></div>

      <form id="orderForm">

        <div class="form-grid">

          <div class="field">
            <label>Full Name *</label>
            <input
              type="text"
              name="customer_name"
              placeholder="Your full name"
              required
            >
          </div>

          <div class="field">
            <label>Mobile Number *</label>
            <input
              type="tel"
              name="phone"
              placeholder="10-digit mobile number"
              pattern="[0-9]{10}"
              required
            >
          </div>

          <div class="field">
            <label>Email *</label>
            <input
              type="email"
              name="email"
              placeholder="you@example.com"
              required
            >
          </div>

          <div class="field">
            <label>Pincode *</label>
            <input
              type="text"
              name="pincode"
              placeholder="6-digit pincode"
              pattern="[0-9]{6}"
              required
            >
          </div>

          <div class="field full-field">
            <label>Delivery Address *</label>
            <textarea
              name="address"
              placeholder="House/Flat number, street, area..."
              required
            ></textarea>
          </div>

          <div class="field">
            <label>City *</label>
            <input
              type="text"
              name="city"
              placeholder="City"
              required
            >
          </div>

          <div class="field">
            <label>State *</label>
            <input
              type="text"
              name="state"
              placeholder="State"
              required
            >
          </div>

          <div class="field full-field">
            <label>Order Notes</label>
            <textarea
              name="order_notes"
              placeholder="Any special instructions? (optional)"
            ></textarea>
          </div>

        </div>

        <button
          type="submit"
          class="primary full"
          id="placeOrderButton"
        >
          Place Order →
        </button>

        <p
          id="checkoutError"
          style="color:#a33c3c;font-size:13px;margin-top:12px;text-align:center"
        ></p>

      </form>

    </div>

  </div>
</div>


<!-- SUCCESS -->

<div class="modal-wrap" id="successModal">
  <div class="checkout-modal">
    <div class="success">

      <div class="success-icon">✓</div>

      <div class="eyebrow">Order received</div>

      <h2>Order Confirmed!</h2>

      <p>
        Thank you for shopping with CONSCIOUS CHEMIST.
        Your order has been submitted successfully.
      </p>

      <div class="order-id" id="successOrderId"></div>

      <p style="margin-top:20px">
        We have received your order details and will contact
        you regarding the next steps.
      </p>

      <button class="primary" onclick="closeSuccess()">
        Continue Shopping
      </button>

    </div>
  </div>
</div>


<div class="toast" id="toast"></div>


<script>

/* ============================================================
   CONSCIOUS CHEMIST
   PRODUCT DATABASE
   ============================================================ */

const products = [

  {
    id:1,
    name:"HydraGlow Face Wash",
    category:"Cleanser",
    price:499,
    badge:"Bestseller",
    description:"A gentle daily cleanser that removes dirt and excess oil while leaving skin feeling fresh and comfortable.",
    skin:"All skin types",
    texture:"Light gel",
    size:"100 ml",
    images:[
      "https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1571781926291-c477ebfd024b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228720-195a672e8a03?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:2,
    name:"Glow Reset Serum",
    category:"Serum",
    price:799,
    badge:"New",
    description:"A lightweight daily serum designed to support a brighter-looking, smoother and more hydrated complexion.",
    skin:"Normal to combination",
    texture:"Water-light serum",
    size:"30 ml",
    images:[
      "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1612817288484-6f916006741a?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1611930022073-b7a4ba5fcccd?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1598440947619-2c35fc9aa908?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:3,
    name:"Barrier Repair Cream",
    category:"Moisturizer",
    price:699,
    badge:"Editor's Pick",
    description:"A rich yet comfortable moisturizer created for dry-feeling skin and everyday barrier support.",
    skin:"Dry to normal",
    texture:"Cream",
    size:"50 g",
    images:[
      "https://images.unsplash.com/photo-1611930022073-b7a4ba5fcccd?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556229010-6c3f2c9ca5f8?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:4,
    name:"Daily Shield SPF 50",
    category:"Sunscreen",
    price:749,
    badge:"Daily Essential",
    description:"A lightweight sunscreen designed for comfortable everyday wear with a smooth finish.",
    skin:"All skin types",
    texture:"Light lotion",
    size:"50 g",
    images:[
      "https://images.unsplash.com/photo-1556228841-7f0a4a5d9f4b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1598440947619-2c35fc9aa908?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1612817288484-6f916006741a?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:5,
    name:"Cloud Milk Cleanser",
    category:"Cleanser",
    price:599,
    badge:"",
    description:"A soft milky cleanser for a comfortable cleanse without leaving the skin feeling stripped.",
    skin:"Dry to sensitive",
    texture:"Milky lotion",
    size:"120 ml",
    images:[
      "https://images.unsplash.com/photo-1598440947619-2c35fc9aa908?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1571781926291-c477ebfd024b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:6,
    name:"Dew Drop Hyaluronic Serum",
    category:"Serum",
    price:849,
    badge:"Hydration",
    description:"A hydration-focused serum with a fresh texture for skin that feels soft, comfortable and replenished.",
    skin:"All skin types",
    texture:"Gel serum",
    size:"30 ml",
    images:[
      "https://images.unsplash.com/photo-1611930022073-b7a4ba5fcccd?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1612817288484-6f916006741a?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:7,
    name:"Calm Cloud Moisturizer",
    category:"Moisturizer",
    price:649,
    badge:"",
    description:"A soft everyday moisturizer made to provide comfortable hydration without a heavy finish.",
    skin:"Normal to dry",
    texture:"Soft cream",
    size:"50 g",
    images:[
      "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556229010-6c3f2c9ca5f8?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1611930022073-b7a4ba5fcccd?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:8,
    name:"Soft Touch Lip Balm",
    category:"Lip Care",
    price:299,
    badge:"Everyday",
    description:"A nourishing everyday lip balm that leaves lips feeling smooth and comfortable.",
    skin:"All skin types",
    texture:"Balm",
    size:"10 g",
    images:[
      "https://images.unsplash.com/photo-1586495777744-4413f21062fa?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1596462502278-27bfdc403348?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1612817288484-6f916006741a?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1598440947619-2c35fc9aa908?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:9,
    name:"Overnight Glow Mask",
    category:"Treatment",
    price:899,
    badge:"Night Ritual",
    description:"A comfortable overnight mask designed to leave skin feeling hydrated and refreshed by morning.",
    skin:"Normal to dry",
    texture:"Cream mask",
    size:"60 g",
    images:[
      "https://images.unsplash.com/photo-1571781926291-c477ebfd024b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228720-195a672e8a03?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:10,
    name:"Purify Clay Mask",
    category:"Mask",
    price:599,
    badge:"",
    description:"A weekly clay mask designed for a refreshed, clean-feeling complexion.",
    skin:"Combination to oily",
    texture:"Clay",
    size:"75 g",
    images:[
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1571781926291-c477ebfd024b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556229010-6c3f2c9ca5f8?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:11,
    name:"Bright Eyes Gel",
    category:"Eye Care",
    price:699,
    badge:"New",
    description:"A lightweight eye gel designed for a fresh and hydrated-looking eye area.",
    skin:"All skin types",
    texture:"Cooling gel",
    size:"15 ml",
    images:[
      "https://images.unsplash.com/photo-1598440947619-2c35fc9aa908?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1612817288484-6f916006741a?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1620916297397-a4a5402a3c6c?auto=format&fit=crop&w=900&q=85"
    ]
  },

  {
    id:12,
    name:"Gentle Micellar Water",
    category:"Cleanser",
    price:449,
    badge:"",
    description:"A refreshing micellar cleanser for removing everyday impurities and makeup.",
    skin:"All skin types",
    texture:"Water",
    size:"200 ml",
    images:[
      "https://images.unsplash.com/photo-1556228720-195a672e8a03?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1571781926291-c477ebfd024b?auto=format&fit=crop&w=900&q=85",
      "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?auto=format&fit=crop&w=900&q=85"
    ]
  }

];


/* ============================================================
   CART
   ============================================================ */

let cart = JSON.parse(localStorage.getItem("cc_cart") || "[]");

function saveCart(){
  localStorage.setItem("cc_cart",JSON.stringify(cart));
  updateCart();
}

function addToCart(id, quantity=1){
  const existing = cart.find(item=>item.id===id);

  if(existing){
    existing.quantity += quantity;
  }else{
    cart.push({id,quantity});
  }

  saveCart();
  showToast("Added to your cart");
}

function removeFromCart(id){
  cart = cart.filter(item=>item.id!==id);
  saveCart();
}

function changeQuantity(id,amount){
  const item = cart.find(item=>item.id===id);

  if(!item) return;

  item.quantity += amount;

  if(item.quantity<=0){
    removeFromCart(id);
  }else{
    saveCart();
  }
}

function cartCount(){
  return cart.reduce((total,item)=>total+item.quantity,0);
}

function cartTotal(){
  return cart.reduce((total,item)=>{
    const p = products.find(x=>x.id===item.id);
    return total+(p ? p.price*item.quantity : 0);
  },0);
}

function updateCart(){
  document.getElementById("cartCount").textContent=cartCount();
  document.getElementById("cartTotal").textContent=formatMoney(cartTotal());

  const box=document.getElementById("cartItems");

  if(cart.length===0){
    box.innerHTML=`
      <div class="empty">
        <div style="font-size:40px;margin-bottom:10px">🛍️</div>
        <strong>Your cart is empty</strong>
        <p style="margin-top:5px">Add something beautiful to your routine.</p>
      </div>
    `;
    return;
  }

  box.innerHTML=cart.map(item=>{
    const p=products.find(x=>x.id===item.id);

    return `
      <div class="cart-item">
        <img src="${p.images[0]}" alt="${p.name}">

        <div>
          <h4>${p.name}</h4>
          <p>${formatMoney(p.price)}</p>

          <div class="qty">
            <button onclick="changeQuantity(${p.id},-1)">−</button>
            <span>${item.quantity}</span>
            <button onclick="changeQuantity(${p.id},1)">+</button>
          </div>
        </div>

        <button class="remove" onclick="removeFromCart(${p.id})">
          Remove
        </button>
      </div>
    `;
  }).join("");
}


/* ============================================================
   PRODUCT GRID
   ============================================================ */

function renderProducts(){

  const grid=document.getElementById("productsGrid");

  grid.innerHTML=products.map(p=>`

    <article class="product">

      <div class="product-img" onclick="openProduct(${p.id})">

        ${p.badge ? `<div class="badge">${p.badge}</div>` : ""}

        <img src="${p.images[0]}" alt="${p.name}" loading="lazy">

      </div>

      <div class="product-info">

        <div class="category">${p.category}</div>

        <div class="product-name">${p.name}</div>

        <div class="product-desc">${p.description}</div>

        <div class="price-row">

          <span class="price">${formatMoney(p.price)}</span>

          <button
            class="add"
            onclick="addToCart(${p.id})"
            aria-label="Add ${p.name} to cart"
          >
            +
          </button>

        </div>

      </div>

    </article>

  `).join("");
}


/* ============================================================
   PRODUCT DETAILS
   ============================================================ */

let selectedProduct=null;

function openProduct(id){

  const p=products.find(x=>x.id===id);

  if(!p) return;

  selectedProduct=p;

  document.getElementById("detailCategory").textContent=p.category;
  document.getElementById("detailName").textContent=p.name;
  document.getElementById("detailPrice").textContent=formatMoney(p.price);
  document.getElementById("detailDescription").textContent=p.description;
  document.getElementById("detailSkin").textContent=p.skin;
  document.getElementById("detailTexture").textContent=p.texture;
  document.getElementById("detailSize").textContent=p.size;

  document.getElementById("detailMainImage").src=p.images[0];
  document.getElementById("detailMainImage").alt=p.name;

  document.getElementById("detailThumbs").innerHTML=p.images.map((image,index)=>`
    <div
      class="thumb ${index===0 ? "active":""}"
      onclick="changeMainImage('${image}',this)"
    >
      <img src="${image}" alt="${p.name} view ${index+1}">
    </div>
  `).join("");

  document.getElementById("detailCartButton").onclick=()=>{
    addToCart(p.id);
  };

  document.getElementById("detailBuyButton").onclick=()=>{
    addToCart(p.id);
    closeProduct();
    openCheckout();
  };

  document.getElementById("productModal").classList.add("active");
  document.body.style.overflow="hidden";
}

function changeMainImage(src,element){

  document.getElementById("detailMainImage").src=src;

  document.querySelectorAll(".thumb").forEach(t=>{
    t.classList.remove("active");
  });

  element.classList.add("active");
}

function closeProduct(){
  document.getElementById("productModal").classList.remove("active");

  if(
    !document.getElementById("checkoutModal").classList.contains("active") &&
    !document.getElementById("successModal").classList.contains("active")
  ){
    document.body.style.overflow="";
  }
}


/* ============================================================
   CART DRAWER
   ============================================================ */

function openCart(){
  updateCart();

  document.getElementById("overlay").classList.add("active");
  document.getElementById("cartDrawer").classList.add("active");

  document.body.style.overflow="hidden";
}

function closeCart(){
  document.getElementById("overlay").classList.remove("active");
  document.getElementById("cartDrawer").classList.remove("active");

  if(
    !document.getElementById("checkoutModal").classList.contains("active") &&
    !document.getElementById("productModal").classList.contains("active")
  ){
    document.body.style.overflow="";
  }
}


/* ============================================================
   CHECKOUT
   ============================================================ */

function openCheckout(){

  if(cart.length===0){
    showToast("Your cart is empty");
    return;
  }

  closeCart();

  renderCheckoutSummary();

  document.getElementById("checkoutError").textContent="";

  document.getElementById("checkoutModal").classList.add("active");

  document.body.style.overflow="hidden";
}

function closeCheckout(){

  document.getElementById("checkoutModal").classList.remove("active");

  if(
    !document.getElementById("productModal").classList.contains("active") &&
    !document.getElementById("successModal").classList.contains("active")
  ){
    document.body.style.overflow="";
  }
}

function renderCheckoutSummary(){

  const box=document.getElementById("checkoutSummary");

  box.innerHTML=`

    ${cart.map(item=>{

      const p=products.find(x=>x.id===item.id);

      return `
        <div class="summary-line">
          <span>${p.name} × ${item.quantity}</span>
          <span>${formatMoney(p.price*item.quantity)}</span>
        </div>
      `;

    }).join("")}

    <div class="summary-line summary-total">
      <span>Total</span>
      <span>${formatMoney(cartTotal())}</span>
    </div>

  `;
}


/* ============================================================
   FORMSPREE ORDER SUBMISSION
   ============================================================ */

const FORMSPREE_ENDPOINT =
  "https://formspree.io/f/xrpgkrpd";

document.getElementById("orderForm").addEventListener("submit",async function(e){

  e.preventDefault();

  if(cart.length===0){
    document.getElementById("checkoutError").textContent=
      "Your cart is empty.";
    return;
  }

  const button=document.getElementById("placeOrderButton");
  const error=document.getElementById("checkoutError");

  button.disabled=true;
  button.textContent="Submitting Order...";
  error.textContent="";

  const orderId=
    "CC-" +
    Date.now().toString().slice(-8);

  const orderDate=
    new Date().toLocaleString("en-IN");

  const productDetails=cart.map(item=>{

    const p=products.find(x=>x.id===item.id);

    return (
      `${p.name} × ${item.quantity} = ` +
      `₹${(p.price*item.quantity).toLocaleString("en-IN")}`
    );

  }).join("\n");

  const formData=new FormData(this);

  /*
    These fields are added to the customer's order submission.
  */

  formData.append("order_id",orderId);
  formData.append("order_date",orderDate);
  formData.append("order_status","NEW ORDER");
  formData.append("products_ordered",productDetails);
  formData.append(
    "order_total",
    `₹${cartTotal().toLocaleString("en-IN")}`
  );
  formData.append(
    "items_count",
    String(cartCount())
  );

  try{

    const response=await fetch(
      FORMSPREE_ENDPOINT,
      {
        method:"POST",
        body:formData,
        headers:{
          "Accept":"application/json"
        }
      }
    );

    if(response.ok){

      /*
        Save the order ID for the confirmation screen.
      */

      document.getElementById("successOrderId").textContent=
        `Order ID: ${orderId}`;

      /*
        Clear cart ONLY after Formspree successfully accepts
        the order.
      */

      cart=[];
      saveCart();

      this.reset();

      closeCheckout();

      document.getElementById("successModal").classList.add("active");

      document.body.style.overflow="hidden";

    }else{

      let message="Unable to submit your order.";

      try{

        const data=await response.json();

        if(data && data.errors && data.errors.length){
          message=data.errors.map(x=>x.message).join(", ");
        }

      }catch(_){}

      error.textContent=
        message + " Please try again.";

    }

  }catch(err){

    error.textContent=
      "Network error. Please check your internet connection and try again.";

  }finally{

    button.disabled=false;
    button.textContent="Place Order →";

  }

});


/* ============================================================
   SUCCESS
   ============================================================ */

function closeSuccess(){

  document.getElementById("successModal").classList.remove("active");

  document.body.style.overflow="";

  window.scrollTo({
    top:document.getElementById("shop").offsetTop-80,
    behavior:"smooth"
  });
}


/* ============================================================
   HELPERS
   ============================================================ */

function formatMoney(amount){

  return "₹" +
    Number(amount).toLocaleString("en-IN");

}

function showToast(message){

  const toast=document.getElementById("toast");

  toast.textContent=message;

  toast.classList.add("show");

  setTimeout(()=>{
    toast.classList.remove("show");
  },2200);
}


/* ============================================================
   INITIALIZE
   ============================================================ */

renderProducts();
updateCart();


/* Close modals when clicking outside */

document.getElementById("productModal").addEventListener("click",function(e){

  if(e.target===this){
    closeProduct();
  }

});

document.getElementById("checkoutModal").addEventListener("click",function(e){

  if(e.target===this){
    closeCheckout();
  }

});

document.getElementById("successModal").addEventListener("click",function(e){

  if(e.target===this){
    closeSuccess();
  }

});

</script>

</body>
</html>
