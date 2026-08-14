<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ashfaq Creative Agency</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Arial,sans-serif;
}

body{
  background:#07111f;
  color:white;
  overflow-x:hidden;
}

header{
  position:sticky;
  top:0;
  z-index:100;
  padding:18px 7%;
  display:flex;
  justify-content:space-between;
  align-items:center;
  background:rgba(5,12,25,.9);
  backdrop-filter:blur(15px);
  border-bottom:1px solid #24395c;
}

.logo{
  font-size:25px;
  font-weight:bold;
  color:#55aaff;
}

nav a{
  color:white;
  text-decoration:none;
  margin-left:20px;
}

.hero{
  min-height:620px;
  padding:100px 7%;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:40px;
  background:
    radial-gradient(circle at 20% 20%,#164b9b,transparent 35%),
    radial-gradient(circle at 80% 70%,#6020a0,transparent 35%),
    #07111f;
}

.hero-text{
  max-width:650px;
}

.hero h1{
  font-size:clamp(45px,8vw,80px);
  line-height:1;
  margin-bottom:25px;
  text-shadow:0 0 30px #267cff;
}

.hero p{
  font-size:20px;
  color:#c8d6ed;
  line-height:1.6;
  margin-bottom:30px;
}

.btn{
  display:inline-block;
  padding:15px 28px;
  border-radius:14px;
  background:linear-gradient(135deg,#1677ff,#753cff);
  color:white;
  text-decoration:none;
  font-weight:bold;
  box-shadow:0 12px 30px rgba(30,110,255,.35);
  transition:.3s;
}

.btn:hover{
  transform:translateY(-5px);
  box-shadow:0 18px 40px rgba(70,130,255,.55);
}

.cube{
  width:220px;
  height:220px;
  border-radius:35px;
  background:linear-gradient(135deg,#1677ff,#8a35ff);
  transform:rotate(12deg);
  box-shadow:
    25px 25px 0 rgba(35,75,150,.35),
    0 0 70px rgba(65,120,255,.55);
  animation:float 4s ease-in-out infinite;
}

@keyframes float{
  0%,100%{transform:rotate(12deg) translateY(0)}
  50%{transform:rotate(17deg) translateY(-20px)}
}

section{
  padding:75px 7%;
}

.title{
  text-align:center;
  font-size:40px;
  margin-bottom:45px;
}

.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(230px,1fr));
  gap:25px;
}

.card{
  padding:30px;
  min-height:210px;
  border-radius:25px;
  background:linear-gradient(145deg,#101f38,#091425);
  border:1px solid #29456f;
  box-shadow:15px 15px 35px rgba(0,0,0,.35);
  transition:.3s;
}

.card:hover{
  transform:translateY(-10px) rotateX(3deg);
  border-color:#3d8cff;
  box-shadow:0 20px 45px rgba(30,110,255,.25);
}

.card h3{
  color:#65aaff;
  font-size:24px;
  margin:15px 0;
}

.card p{
  color:#b8c7df;
  line-height:1.6;
}

.price{
  font-size:35px;
  font-weight:bold;
  margin:20px 0;
  color:white;
}

.package{
  text-align:center;
}

.package ul{
  list-style:none;
  text-align:left;
  line-height:2;
  color:#c7d4e8;
  margin-bottom:20px;
}

.payment{
  background:linear-gradient(135deg,#0b1c35,#15103a);
}

.payment-box{
  max-width:700px;
  margin:auto;
  padding:35px;
  border-radius:28px;
  background:#0a1629;
  border:1px solid #31547f;
  box-shadow:0 20px 60px rgba(0,0,0,.4);
}

.payment-box h3{
  color:#65aaff;
  margin-bottom:18px;
}

.number{
  font-size:24px;
  font-weight:bold;
  background:#142743;
  padding:18px;
  border-radius:14px;
  margin:10px 0 25px;
  word-break:break-word;
}

.note{
  color:#b9c8df;
  line-height:1.6;
}

.contact{
  text-align:center;
}

footer{
  padding:30px;
  text-align:center;
  color:#9eb0ca;
  background:#040b15;
}

@media(max-width:700px){
  nav{display:none}
  .hero{
    text-align:center;
    flex-direction:column;
    padding-top:70px;
  }
  .cube{
    width:150px;
    height:150px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">Ashfaq Creative</div>
  <nav>
    <a href="#services">Services</a>
    <a href="#packages">Packages</a>
    <a href="#payment">Payment</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <div class="hero-text">
    <h1>Creative Agency</h1>
    <p>
      Professional digital services, creative designs and social media
      solutions for individuals and businesses.
    </p>
    <a class="btn" href="#packages">View Packages</a>
  </div>

  <div class="cube"></div>
</section>

<section id="services">
  <h2 class="title">Our Services</h2>

  <div class="grid">

    <div class="card">
      <h3>🎨 Graphic Design</h3>
      <p>Professional social media posts, banners, posters and creative designs.</p>
    </div>

    <div class="card">
      <h3>📱 Social Media</h3>
      <p>Creative content and profile/page improvement for social platforms.</p>
    </div>

    <div class="card">
      <h3>🌐 Website Design</h3>
      <p>Modern responsive websites for personal and business projects.</p>
    </div>

    <div class="card">
      <h3>🎬 Video Editing</h3>
      <p>Short-form video editing and promotional content for social media.</p>
    </div>

    <div class="card">
      <h3>✍️ Content Writing</h3>
      <p>Captions, descriptions, promotional text and creative content.</p>
    </div>

    <div class="card">
      <h3>💼 Business Branding</h3>
      <p>Creative branding ideas, promotional graphics and digital identity.</p>
    </div>

  </div>
</section>

<section id="packages">
  <h2 class="title">Service Packages</h2>

  <div class="grid">

    <div class="card package">
      <h3>Starter</h3>
      <div class="price">PKR 5,000</div>
      <ul>
        <li>✓ Basic Graphic Design</li>
        <li>✓ Social Media Content</li>
        <li>✓ 5 Creative Posts</li>
        <li>✓ Basic Support</li>
      </ul>
      <a class="btn" href="#payment">Order Now</a>
    </div>

    <div class="card package">
      <h3>Professional</h3>
      <div class="price">PKR 10,000</div>
      <ul>
        <li>✓ Premium Designs</li>
        <li>✓ 10 Creative Posts</li>
        <li>✓ Social Media Content</li>
        <li>✓ Priority Support</li>
      </ul>
      <a class="btn" href="#payment">Order Now</a>
    </div>

    <div class="card package">
      <h3>Business</h3>
      <div class="price">PKR 20,000</div>
      <ul>
        <li>✓ Business Branding</li>
        <li>✓ Website Design</li>
        <li>✓ Social Media Package</li>
        <li>✓ Premium Support</li>
      </ul>
      <a class="btn" href="#payment">Order Now</a>
    </div>

  </div>
</section>

<section id="payment" class="payment">
  <h2 class="title">Payment Method</h2>

  <div class="payment-box">

    <h3>JazzCash / Easypaisa</h3>

    <p class="note">
      Service package select karne ke baad payment neeche diye gaye
      account par send karein aur transaction screenshot/order details
      contact par bhejein.
    </p>

    <div class="number">
      Account Name: Ashfaq Sadiq<br>
      Mobile: 03081724110
    </div>

    <p class="note">
      ⚠️ Payment sirf ordered services ke liye karein.
      Service start hone se pehle package aur price confirm karna zaroori hai.
    </p>

    <br>

    <a class="btn" href="#contact">Send Order Details</a>

  </div>
</section>

<section id="contact" class="contact">
  <h2 class="title">Contact Us</h2>

  <p style="color:#bdcbe0;font-size:19px;line-height:1.8">
    Ashfaq Sadiq<br>
    Creative Agency<br>
    Mobile: 03081724110
  </p>

  <br>

  <a class="btn" href="tel:03081724110">Contact Now</a>
</section>

<footer>
  © 2026 Ashfaq Creative Agency — All Rights Reserved
</footer>

</body>
</html>
