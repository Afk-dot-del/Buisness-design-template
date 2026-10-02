# Buisness-design-template
Buisness template
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Business Designer — Professional Websites</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html{
  scroll-behavior:smooth;
}

body{
  font-family:Inter,Arial,sans-serif;
  background:#fff;
  color:#171717;
}

/* NAVBAR */
nav{
  position:sticky;
  top:0;
  z-index:1000;
  display:flex;
  align-items:center;
  justify-content:space-between;
  padding:16px 7%;
  background:rgba(255,255,255,.95);
  backdrop-filter:blur(15px);
  border-bottom:1px solid #eee;
}

.logo{
  font-size:20px;
  font-weight:900;
}

.logo span{
  color:#ff6500;
}

.nav-links{
  display:flex;
  gap:28px;
  list-style:none;
}

.nav-links a{
  color:#333;
  text-decoration:none;
  font-weight:700;
}

.nav-links a:hover{
  color:#ff6500;
}

.nav-btn{
  background:#ff6500;
  color:#fff;
  text-decoration:none;
  padding:11px 18px;
  border-radius:11px;
  font-weight:800;
}

/* HERO */
.hero{
  min-height:680px;
  display:flex;
  align-items:center;
  padding:90px 7%;
  background:
    radial-gradient(circle at 85% 20%,#ffe1cf,transparent 30%),
    linear-gradient(135deg,#fff,#fff7f1);
}

.hero-content{
  max-width:780px;
}

.badge{
  display:inline-block;
  padding:7px 14px;
  background:#fff0e7;
  color:#e95500;
  border-radius:50px;
  font-size:12px;
  font-weight:900;
  letter-spacing:1px;
  margin-bottom:22px;
}

.hero h1{
  font-size:clamp(45px,7vw,80px);
  line-height:1.02;
  letter-spacing:-4px;
}

.hero h1 span{
  color:#ff6500;
}

.hero p{
  max-width:650px;
  margin:25px 0;
  color:#666;
  font-size:18px;
}

.buttons{
  display:flex;
  gap:12px;
  flex-wrap:wrap;
}

.btn{
  display:inline-block;
  padding:14px 22px;
  border-radius:12px;
  font-weight:850;
  text-decoration:none;
  cursor:pointer;
  border:0;
}

.orange{
  background:#ff6500;
  color:#fff;
  box-shadow:0 10px 28px rgba(255,101,0,.22);
}

.white{
  background:#fff;
  color:#ff6500;
  border:1px solid #ff6500;
}

/* SECTIONS */
section{
  padding:90px 7%;
}

.section-title{
  text-align:center;
  max-width:720px;
  margin:0 auto 50px;
}

.section-title h2{
  font-size:43px;
  line-height:1.1;
}

.section-title p{
  color:#777;
  margin-top:12px;
}

/* SERVICES */
.grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:22px;
}

.card{
  background:#fff;
  border:1px solid #eee;
  border-radius:22px;
  padding:30px;
  box-shadow:0 12px 35px rgba(0,0,0,.05);
  transition:.25s;
}

.card:hover{
  transform:translateY(-6px);
  box-shadow:0 20px 45px rgba(0,0,0,.09);
}

.icon{
  width:50px;
  height:50px;
  display:grid;
  place-items:center;
  background:#fff0e7;
  color:#ff6500;
  border-radius:15px;
  font-size:23px;
  margin-bottom:20px;
}

.card h3{
  font-size:22px;
  margin-bottom:9px;
}

.card p{
  color:#707070;
}

/* ABOUT */
.about{
  background:#fafafa;
}

.about-grid{
  max-width:950px;
  margin:auto;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:22px;
}

.about-card{
  background:#fff;
  border:1px solid #eee;
  border-radius:22px;
  padding:35px;
}

.about-card h3{
  font-size:25px;
  margin-bottom:10px;
}

.about-card p{
  color:#707070;
}

/* PRICING */
.pricing{
  background:#fafafa;
}

.price-card{
  position:relative;
}

.popular{
  position:absolute;
  top:18px;
  right:18px;
  background:#ff6500;
  color:white;
  padding:5px 10px;
  border-radius:50px;
  font-size:10px;
  font-weight:900;
}

.price{
  font-size:42px;
  font-weight:950;
  margin:15px 0;
}

.price small{
  font-size:13px;
  color:#777;
  font-weight:500;
}

.features{
  list-style:none;
  margin:22px 0;
}

.features li{
  padding:7px 0;
  color:#555;
}

.features li::before{
  content:"✓";
  color:#ff6500;
  font-weight:900;
  margin-right:9px;
}

.featured{
  border:2px solid #ff6500;
}

/* CONTACT */
.contact{
  background:#171717;
  color:#fff;
  text-align:center;
}

.contact h2{
  font-size:43px;
}

.contact p{
  max-width:600px;
  margin:15px auto 25px;
  color:#bbb;
}

/* INSTAGRAM */
.instagram-box{
  max-width:450px;
  margin:30px auto 0;
  padding:25px;
  background:#fff;
  color:#171717;
  border:2px solid #ff6500;
  border-radius:20px;
  box-shadow:0 12px 35px rgba(0,0,0,.25);
}

.instagram-label{
  color:#ff6500;
  font-size:12px;
  font-weight:950;
  letter-spacing:2px;
}

.instagram-id{
  margin:10px 0;
  padding:10px;
  font-size:20px;
  font-weight:950;
  cursor:pointer;
  user-select:all;
  word-break:break-word;
}

.copy-btn{
  border:0;
  background:#ff6500;
  color:white;
  padding:11px 18px;
  border-radius:10px;
  font-weight:850;
  cursor:pointer;
}

.copy-message{
  min-height:20px;
  margin-top:9px;
  color:#ff6500;
  font-size:13px;
  font-weight:800;
}

/* FOOTER */
footer{
  padding:28px 7%;
  background:#101010;
  color:#999;
  text-align:center;
  font-size:14px;
}

footer strong{
  color:white;
}

footer a{
  color:#ff6500;
  text-decoration:none;
}

/* MOBILE */
@media(max-width:850px){

  .nav-links{
    display:none;
  }

  .hero{
    padding:70px 6%;
  }

  section{
    padding:70px 6%;
  }

  .grid{
    grid-template-columns:1fr;
  }

  .about-grid{
    grid-template-columns:1fr;
  }

  .section-title h2,
  .contact h2{
    font-size:35px;
  }
}

@media(max-width:450px){

  .logo{
    font-size:17px;
  }

  .nav-btn{
    padding:9px 12px;
    font-size:12px;
  }

  .hero h1{
    font-size:45px;
    letter-spacing:-2px;
  }

  .buttons .btn{
    width:100%;
    text-align:center;
  }

  .instagram-id{
    font-size:18px;
  }
}
</style>
</head>

<body>

<!-- NAVBAR -->
<nav>

  <div class="logo">
    BUSINESS <span>DESIGNER</span>
  </div>

  <ul class="nav-links">
    <li><a href="#services">Services</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#pricing">Pricing</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>

  <a href="#contact" class="nav-btn">
    Get Started
  </a>

</nav>


<!-- HERO -->
<section class="hero">

  <div class="hero-content">

    <div class="badge">
      PREMIUM DIGITAL DESIGN STUDIO
    </div>

    <h1>
      Websites that make your
      <span>business stand out.</span>
    </h1>

    <p>
      Professional, modern and responsive websites
      designed for businesses, creators and brands.
    </p>

    <div class="buttons">

      <a href="#pricing" class="btn orange">
        View Packages
      </a>

      <a href="#contact" class="btn white">
        Contact Us
      </a>

    </div>

  </div>

</section>


<!-- SERVICES -->
<section id="services">

  <div class="section-title">

    <h2>What We Build</h2>

    <p>
      Everything you need for a professional
      online presence.
    </p>

  </div>

  <div class="grid">

    <div class="card">

      <div class="icon">✦</div>

      <h3>Business Websites</h3>

      <p>
        Modern websites designed specifically
        around your business and brand.
      </p>

    </div>


    <div class="card">

      <div class="icon">◈</div>

      <h3>Landing Pages</h3>

      <p>
        Clean and focused landing pages for
        products, services and campaigns.
      </p>

    </div>


    <div class="card">

      <div class="icon">◎</div>

      <h3>Digital Design</h3>

      <p>
        Professional digital designs that help
        your brand look polished online.
      </p>

    </div>

  </div>

</section>


<!-- ABOUT -->
<section id="about" class="about">

  <div class="section-title">

    <h2>Built for Modern Businesses</h2>

    <p>
      Clean design, responsive layouts and
      professional digital experiences.
    </p>

  </div>

  <div class="about-grid">

    <div class="about-card">

      <h3>Modern Design</h3>

      <p>
        Every website is designed with a clean,
        premium and modern visual style.
      </p>

    </div>

    <div class="about-card">

      <h3>Mobile Friendly</h3>

      <p>
        Your website works smoothly across
        phones, tablets and desktop screens.
      </p>

    </div>

  </div>

</section>


<!-- PRICING -->
<section id="pricing" class="pricing">

  <div class="section-title">

    <h2>Simple Pricing</h2>

    <p>
      Choose the package that fits your business.
    </p>

  </div>

  <div class="grid">

    <!-- STARTER -->
    <div class="card price-card">

      <h3>Starter</h3>

      <div class="price">
        ₹999 <small>/ project</small>
      </div>

      <ul class="features">
        <li>Professional website</li>
        <li>Responsive design</li>
        <li>Contact section</li>
        <li>Social links</li>
        <li>Basic customization</li>
      </ul>

      <a href="#contact" class="btn orange">
        Get Starter
      </a>

    </div>


    <!-- BUSINESS -->
    <div class="card price-card featured">

      <div class="popular">
        POPULAR
      </div>

      <h3>Business</h3>

      <div class="price">
        ₹1,999 <small>/ project</small>
      </div>

      <ul class="features">
        <li>Premium website</li>
        <li>Advanced responsive design</li>
        <li>10 social media designs</li>
        <li>10 promotional captions</li>
        <li>7-day content plan</li>
        <li>Google Maps + social integration</li>
      </ul>

      <a href="#contact" class="btn orange">
        Get Business
      </a>

    </div>


    <!-- PREMIUM -->
    <div class="card price-card">

      <h3>Premium</h3>

      <div class="price">
        ₹2,000 <small>/ project</small>
      </div>

      <ul class="features">
        <li>Everything in Business</li>
        <li>Premium custom design</li>
        <li>Advanced animations</li>
        <li>Custom sections</li>
        <li>Priority customization</li>
        <li>Premium support</li>
      </ul>

      <a href="#contact" class="btn orange">
        Get Premium
      </a>

    </div>

  </div>

</section>


<!-- CONTACT -->
<section id="contact" class="contact">

  <h2>
    Ready to build your website?
  </h2>

  <p>
    Contact us on Instagram and tell us what
    kind of website you want for your business.
  </p>


  <div class="instagram-box">

    <div class="instagram-label">
      INSTAGRAM
    </div>

    <div
      class="instagram-id"
      onclick="copyInstagram()">

      @buisness_template_deginer0x

    </div>

    <button
      class="copy-btn"
      onclick="copyInstagram()">

      📋 Copy Instagram ID

    </button>

    <div
      id="copyMessage"
      class="copy-message">
    </div>

  </div>

</section>


<!-- FOOTER -->
<footer>

  © 2026
  <strong>BUSINESS DESIGNER</strong>
  ·

  <a
    href="https://www.instagram.com/buisness_template_deginer0x/"
    target="_blank"
    rel="noopener noreferrer">

    Instagram

  </a>

</footer>


<script>

function copyInstagram(){

  const username =
    "buisness_template_deginer0x";

  if(navigator.clipboard){

    navigator.clipboard.writeText(username)
    .then(function(){

      document.getElementById("copyMessage")
      .textContent =
      "✓ Instagram ID copied!";

    })
    .catch(function(){

      fallbackCopy(username);

    });

  }else{

    fallbackCopy(username);

  }

}

function fallbackCopy(text){

  const input =
    document.createElement("textarea");

  input.value = text;

  document.body.appendChild(input);

  input.select();

  document.execCommand("copy");

  document.body.removeChild(input);

  document.getElementById("copyMessage")
  .textContent =
  "✓ Instagram ID copied!";

}

</script>

</body>
</html>
