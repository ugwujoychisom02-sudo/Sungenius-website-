# Sungenius-website-
Marketing website 
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sungenius Electronics</title>
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

header{
    background:#0a3d62;
    color:white;
    padding:20px;
}

.logo{
    font-size:30px;
    font-weight:bold;
}

nav{
    margin-top:15px;
}

nav a{
    color:white;
    text-decoration:none;
    margin-right:20px;
    font-weight:bold;
}

.hero{
    background:linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.6)), url("banner.jpg");
    background-size:cover;
    background-position:center;
    color:white;
    text-align:center;
    padding:100px 20px;
}

.hero h1{
    font-size:50px;
}

.hero p{
    margin:20px 0;
    font-size:20px;
}

.btn{
    display:inline-block;
    background:#ff9800;
    color:white;
    text-decoration:none;
    padding:15px 30px;
    border-radius:5px;
}

.section-title{
    text-align:center;
    margin:40px 0 20px;
}

.products{
    display:flex;
    justify-content:center;
    gap:20px;
    flex-wrap:wrap;
    padding:20px;
}

.card{
    background:white;
    width:250px;
    border-radius:10px;
    box-shadow:0 0 10px rgba(0,0,0,.2);
    overflow:hidden;
    text-align:center;
}

.card img{
    width:100%;
    height:200px;
    object-fit:cover;
}

.card h3{
    margin:10px;
}

.price{
    color:#0a3d62;
    font-size:22px;
    font-weight:bold;
}

button{
    margin:15px;
    background:#0a3d62;
    color:white;
    border:none;
    padding:12px 20px;
    border-radius:5px;
    cursor:pointer;
}

footer{
    background:#0a3d62;
    color:white;
    text-align:center;
    padding:20px;
    margin-top:40px;
}
</style>

</head>
<body>

<header>
    <section class="slider">

<img id="slide" src="banner1.jpg" alt="Banner">

</section>
    <div class="top-bar">
    <input type="text" placeholder="Search products..." id="search">
    <button class="search-btn">Search</button>
    <button id="darkBtn">🌙 Dark Mode</button>

    <div class="cart">
        🛒 Cart (<span id="cart-count">0</span>)
    </div>
</div>

<div class="logo">Sungenius Electronics</div>

<nav>
    <a href="index.html">Home</a>
    <a href="products.html">Products</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
    <a href="cart.html">🛒 Cart</a>
    <a href="login.html">Login</a>
</nav>

</header>

<section class="hero">

<h1>Welcome to Sungenius Electronics</h1>

<p>Your Trusted Online Electronics Store</p>

<a href="#" class="btn">Shop Now</a>

</section>
<section class="categories">

<h2 class="section-title">Shop by Category</h>
<div class="products">

<div class="card">
    <a href="phones.html">
        <h3>📱 Smartphones</h3>
    </a>
</div>

<div class="card">
    <a href="laptop.html">
        <h3>💻 Laptops</h3>
    </a>
</div>

<div class="card">
    <a href="accessories.html">
        <h3>🎧 Accessories</h3>
    </a>
</div>

<div class="card">
    <a href="televisions.html">
        <h3>📺 Televisions</h3>
    </a>
</div>

</div>

</section>

<h2 class="section-title">Featured Products</h2>

<div class="products">
<section id="cart-section">

<h2 class="section-title">Shopping Cart</h2>

<div id="cart-items">
<p>Your cart is empty.</p>
</div>

<h3>Total: ₦<span id="total">0</span></h3>

</section>

<section id="checkout">

<h2 class="section-title">Checkout</h2>

<form id="checkoutForm">

<input type="text" placeholder="Full Name" required>

<input type="email" placeholder="Email Address" required>

<input type="text" placeholder="Delivery Address" required>

<input type="tel" placeholder="Phone Number" required>

<button type="submit">Place Order</button>

</form>

</section>
<div class="card">
<img src="sam.jpg" alt="Phone">
<div
<h3>
<a href="product.html">Samsung S26 ultra</a>
</h3>
</div>
<button>Buy Now</button>
</div>

<div class="card">
<img src="hp.jpg" alt="Laptop">
<h3>HP Laptop</h3>
<p class="price">₦450,000</p>
<button>Buy Now</button>
</div>

<div class="card">
<img src="s.jpg" alt="smartwatch">
<h3>smart watch</h3>
<p class="price">₦35,000</p>
<button>Buy Now</button>
</div>

</div>
<section id="login">

<h2 class="section-title">Login</h2>

<form>

<input type="email" placeholder="Email" required>

<input type="password" placeholder="Password" required>

<button type="submit">Login</button>

</form>

</section>

<section id="reviews">

<h2 class="section-title">Customer Reviews</h2>

<div class="card">
⭐⭐⭐⭐⭐
<p>"Excellent service and fast delivery!"</p>
<b>- Emmanuel</b>
</div>

<div class="card">
⭐⭐⭐⭐☆
<p>"The laptop I bought works perfectly."</p>
<b>- Joy</b>
</div>

</section>

<section id="newsletter">

<h2 class="section-title">Subscribe</h2>

<p>Receive updates about new products and discounts.</p>

<input type="email" id="newsEmail" placeholder="Enter your email">

<button oncltoick="subscribe()">Subscribe</button>

</section>
<footer>

<h3>Sungenius Electronics</h3>

<p>Quality Electronics at Affordable Prices.</p>

<p>📞 +234 XXX XXX XXXX</p>

<p>📧 info@sungenius.com</p>

</footer>
<script>
function subscribe(){

let email=document.getElementById("newsEmail").value;

if(email==""){

alert("Please enter your email.");

}else{

alert("Thank you for subscribing!");

}

}
let cart = 0;

const buttons = document.querySelectorAll("button");

buttons.forEach(button => {
    if(button.innerText === "Buy Now"){
        button.addEventListener("click", () => {
            cart++;
            document.getElementById("cart-count").innerText = cart;
       
<a href="https://wa.me/2348000000000" class="whatsapp" target="_blank">
💬
</a></body>
</html>
