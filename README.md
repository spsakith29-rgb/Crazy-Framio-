<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Crazy Framio | Luxury Photo Frame Studio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
scroll-behavior:smooth;
font-family:'Poppins', sans-serif;
}

body{
background:#0d0d0d;
color:white;
}

/* Header */
header{
background:black;
padding:20px;
text-align:center;
border-bottom:2px solid gold;
}

header h1{
color:gold;
font-size:32px;
}

/* Navigation */
nav{
display:flex;
justify-content:center;
background:#111;
flex-wrap:wrap;
}

nav a{
color:white;
padding:15px 20px;
text-decoration:none;
transition:0.3s;
}

nav a:hover{
color:gold;
}

/* Hero */
.hero{
height:90vh;
background:linear-gradient(rgba(0,0,0,0.7),rgba(0,0,0,0.7)),
url('https://images.unsplash.com/photo-1516035069371-29a1b244cc32');
background-size:cover;
background-position:center;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero h2{
font-size:42px;
color:gold;
margin-bottom:15px;
animation:fadeIn 2s ease-in;
}

.hero button{
padding:12px 25px;
background:gold;
border:none;
font-weight:bold;
cursor:pointer;
border-radius:5px;
transition:0.3s;
}

.hero button:hover{
background:white;
}

/* Sections */
.section{
padding:60px 20px;
text-align:center;
}

.section h2{
color:gold;
margin-bottom:20px;
}

/* Gallery */
.gallery{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:20px;
}

.gallery img{
width:280px;
height:200px;
object-fit:cover;
border-radius:10px;
transition:0.4s;
}

.gallery img:hover{
transform:scale(1.1);
}

/* Pricing */
.pricing{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
}

.card{
background:#1a1a1a;
padding:30px;
width:250px;
border:1px solid gold;
border-radius:10px;
transition:0.3s;
}

.card:hover{
transform:translateY(-10px);
}

/* Form */
form{
max-width:400px;
margin:auto;
display:flex;
flex-direction:column;
gap:15px;
}

input, textarea{
padding:10px;
border:none;
border-radius:5px;
}

button.submit{
background:gold;
color:black;
border:none;
padding:12px;
font-weight:bold;
cursor:pointer;
}

/* Footer */
footer{
background:black;
padding:15px;
text-align:center;
border-top:2px solid gold;
}

/* WhatsApp floating */
.whatsapp{
position:fixed;
bottom:20px;
right:20px;
background:#25D366;
color:white;
padding:15px;
border-radius:50%;
font-size:20px;
text-decoration:none;
}

@keyframes fadeIn{
from{opacity:0;}
to{opacity:1;}
}

@media(max-width:768px){
.hero h2{
font-size:28px;
}
}
</style>
</head>

<body>

<header>
<h1>Crazy Framio</h1>
<p>Luxury Photo Frame Studio</p>
</header>

<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#gallery">Gallery</a>
<a href="#pricing">Pricing</a>
<a href="#order">Order</a>
</nav>

<section id="home" class="hero">
<h2>Capture Memories. Frame Emotions.</h2>
<p>Premium custom photo frames for your special moments.</p>
<br>
<button onclick="window.location.href='tel:0764974719'">Call Now</button>
</section>

<section id="about" class="section">
<h2>About Us</h2>
<p>Crazy Framio creates high-quality custom frames, wall art, and memory displays. We turn your photos into luxury masterpieces.</p>
</section>

<section id="gallery" class="section">
<h2>Our Work</h2>
<div class="gallery">
 <form action="/upload" method="post" enctype="multipart/form-data">
    <input type="file" name="photo" accept="image/*">
    <button type="submit">Upload</button>
  </form>
<section id="pricing" class="section">
<h2>Pricing</h2>
<div class="pricing">
<div class="card">
<h3>Basic size and price </h3>
  <p>12×18</p>
<p>From LKR 2600</p>
</div>
<div class="card">
<h3>medium size and price</h3>
  <p>18×24</p>
<p>From LKR 5000</p>
</div>
<div class="card">
<h3>maximum size and price</h3>
<p>36×48</p>
  <p>From LKR 15000</p>
</div>
</div>
</section>

<section id="order" class="section">
<h2>Place an Order</h2>
<form>
<input type="text" placeholder="Your Name" required>
<input type="tel" placeholder="Phone Number" required>
<textarea placeholder="Frame Details" rows="4"></textarea>
<button class="submit">Submit Order</button>
</form>
</section>

<footer>
<p>© 2026 Crazy Framio. All Rights Reserved.</p>
</footer>

<a class="whatsapp" href="https://wa.me/94764974719" target="_blank">💬</a>

</body>
</html>
