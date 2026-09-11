# sadguru-shop-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sadguru Shop | Jewellery, Beauty & Home Accessories</title>

<meta name="description"
content="Sadguru Shop - Jewellery, Earrings, Bracelets, Bangles, Cutlery Sets, Face Wash and more.">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:#fffaf7;
    color:#29201d;
}

/* HEADER */
header{
    background:linear-gradient(135deg,#5a1830,#8d3151);
    color:white;
    padding:15px 6%;
    position:sticky;
    top:0;
    z-index:1000;
    box-shadow:0 3px 15px rgba(0,0,0,.15);
}

.navbar{
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:20px;
}

.logo{
    font-size:27px;
    font-weight:bold;
}

.logo span{
    color:#ffd88a;
}

nav{
    display:flex;
    gap:20px;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
}

nav a:hover{
    color:#ffd88a;
}

/* HERO */
.hero{
    min-height:500px;
    padding:70px 7%;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    background:
    linear-gradient(rgba(60,10,30,.72),rgba(60,10,30,.72)),
    url("https://images.unsplash.com/photo-1617038220319-276d3cfab638?auto=format&fit=crop&w=1600&q=80")
    center/cover;
    color:white;
}

.hero-content{
    max-width:750px;
}

.hero h1{
    font-size:55px;
    margin-bottom:15px;
}

.hero h1 span{
    color:#ffd88a;
}

.hero p{
    font-size:20px;
    line-height:1.6;
    margin-bottom:30px;
}

.btn{
    display:inline-block;
    padding:13px 25px;
    background:#ffd88a;
    color:#4d1729;
    text-decoration:none;
    border-radius:30px;
    font-weight:bold;
    margin:5px;
    border:none;
    cursor:pointer;
}

.btn:hover{
    transform:translateY(-2px);
    box-shadow:0 5px 15px rgba(0,0,0,.2);
}

/* SECTION */
section{
    padding:60px 6%;
}

.section-title{
    text-align:center;
    margin-bottom:35px;
}

.section-title h2{
    color:#671c38;
    font-size:34px;
    margin-bottom:8px;
}

.section-title p{
    color:#777;
}

/* CATEGORIES */
.categories{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
    gap:18px;
}

.category{
    background:white;
    padding:25px 12px;
    text-align:center;
    border-radius:15px;
    box-shadow:0 4px 15px rgba(0,0,0,.08);
    cursor:pointer;
    transition:.3s;
}

.category:hover{
    transform:translateY(-6px);
    background:#fff2e6;
}

.category .icon{
    font-size:40px;
    margin-bottom:10px;
}

.category h3{
    font-size:16px;
}

/* SEARCH */
.search-box{
    max-width:600px;
    margin:0 auto 30px;
    display:flex;
}

.search-box input{
    width:100%;
    padding:15px 20px;
    border:1px solid #ddd;
    border-radius:30px;
    outline:none;
    font-size:16px;
}

/* PRODUCTS */
.products{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(210px,1fr));
    gap:25px;
}

.product{
    background:white;
    border-radius:16px;
    overflow:hidden;
    box-shadow:0 4px 18px rgba(0,0,0,.09);
    transition:.3s;
}

.product:hover{
    transform:translateY(-5px);
}

.product img{
    width:100%;
    height:210px;
    object-fit:cover;
}

.product-info{
    padding:18px;
}

.product-info h3{
    color:#53172e;
    margin-bottom:8px;
}

.category-name{
    font-size:13px;
    color:#888;
    margin-bottom:8px;
}

.price{
    font-size:20px;
    font-weight:bold;
    color:#9a3c4f;
    margin:10px 0;
}

.order-btn{
    display:block;
    text-align:center;
    background:#25D366;
    color:white;
    padding:11px;
    border-radius:25px;
    text-decoration:none;
    font-weight:bold;
}

/* ABOUT */
.about{
    background:#f8eee8;
}

.about-box{
    max-width:900px;
    margin:auto;
    text-align:center;
    line-height:1.8;
    font-size:17px;
}

/* FEATURES */
.features{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
    gap:20px;
}

.feature{
    background:white;
    padding:25px;
    text-align:center;
    border-radius:15px;
    box-shadow:0 3px 12px rgba(0,0,0,.07);
}

.feature-icon{
    font-size:35px;
    margin-bottom:10px;
}

/* CONTACT */
.contact{
    background:#fff;
}

.contact-box{
    max-width:700px;
    margin:auto;
    text-align:center;
}

.contact-item{
    margin:15px;
    font-size:18px;
}

.contact-item a{
    color:#7c2342;
    text-decoration:none;
    font-weight:bold;
}

/* FOOTER */
footer{
    background:#3e1325;
    color:white;
    text-align:center;
    padding:30px 15px;
}

footer h2{
    color:#ffd88a;
    margin-bottom:10px;
}

.social{
    margin:15px 0;
}

.social a{
    color:white;
    text-decoration:none;
    margin:0 8px;
}

/* WHATSAPP FLOAT */
.whatsapp{
    position:fixed;
    right:20px;
    bottom:20px;
    width:58px;
    height:58px;
    background:#25D366;
    color:white;
    border-radius:50%;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:30px;
    text-decoration:none;
    box-shadow:0 4px 15px rgba(0,0,0,.25);
    z-index:2000;
}

/* MOBILE */
@media(max-width:700px){

    header{
        padding:13px 4%;
    }

    .navbar{
        flex-direction:column;
    }

    nav{
        gap:12px;
        flex-wrap:wrap;
        justify-content:center;
    }

    nav a{
        font-size:14px;
    }

    .hero{
        min-height:450px;
        padding:50px 5%;
    }

    .hero h1{
        font-size:40px;
    }

    .hero p{
        font-size:17px;
    }

    section{
        padding:45px 5%;
    }

    .section-title h2{
        font-size:28px;
    }

    .products{
        grid-template-columns:repeat(2,1fr);
        gap:13px;
    }

    .product img{
        height:160px;
    }

    .product-info{
        padding:12px;
    }

    .product-info h3{
        font-size:15px;
    }

    .price{
        font-size:17px;
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
<div class="navbar">

<div class="logo">
Sadguru <span>Shop</span>
</div>

<nav>
<a href="#home">Home</a>
<a href="#categories">Categories</a>
<a href="#products">Products</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>
</nav>

</div>
</header>


<!-- HERO -->
<section class="hero" id="home">

<div class="hero-content">

<h1>Welcome to <span>Sadguru Shop</span></h1>

<p>
Discover beautiful jewellery, trendy accessories,
useful cutlery sets, beauty products and much more —
all at great prices.
</p>

<a href="#products" class="btn">Shop Now</a>

<a href="#contact" class="btn">Contact Us</a>

</div>

</section>


<!-- CATEGORIES -->
<section id="categories">

<div class="section-title">
<h2>Shop By Category</h2>
<p>Choose your favourite category</p>
</div>

<div class="categories">

<div class="category" onclick="filterProducts('Cutlery')">
<div class="icon">🍽️</div>
<h3>Cutlery Sets</h3>
</div>

<div class="category" onclick="filterProducts('Jewellery')">
<div class="icon">💎</div>
<h3>Jewellery</h3>
</div>

<div class="category" onclick="filterProducts('Earrings')">
<div class="icon">👂</div>
<h3>Earrings</h3>
</div>

<div class="category" onclick="filterProducts('Bracelet')">
<div class="icon">✨</div>
<h3>Bracelets</h3>
</div>

<div class="category" onclick="filterProducts('Bangles')">
<div class="icon">💫</div>
<h3>Bangles</h3>
</div>

<div class="category" onclick="filterProducts('Beauty')">
<div class="icon">🧴</div>
<h3>Beauty</h3>
</div>

</div>

</section>


<!-- PRODUCTS -->
<section id="products">

<div class="section-title">
<h2>Our Products</h2>
<p>Explore our latest collection</p>
</div>

<div class="search-box">
<input
type="text"
id="searchInput"
placeholder="🔍 Search products..."
onkeyup="searchProducts()">
</div>


<div class="products" id="productList">


<!-- PRODUCT 1 -->
<div class="product" data-name="cutlery set" data-category="Cutlery">

<img src="https://images.unsplash.com/photo-1584302179602-e4c3d3fd629d?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Cutlery</div>

<h3>Premium Cutlery Set</h3>

<p>Beautiful and useful kitchen cutlery set.</p>

<div class="price">₹499</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Premium%20Cutlery%20Set."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 2 -->
<div class="product" data-name="jewellery set" data-category="Jewellery">

<img src="https://images.unsplash.com/photo-1611652022419-a9419f74343d?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Jewellery</div>

<h3>Elegant Jewellery Set</h3>

<p>Stylish jewellery for special occasions.</p>

<div class="price">₹699</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Elegant%20Jewellery%20Set."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 3 -->
<div class="product" data-name="earrings" data-category="Earrings">

<img src="https://images.unsplash.com/photo-1535632066927-ab7c9ab60908?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Earrings</div>

<h3>Fashion Earrings</h3>

<p>Trendy earrings for everyday style.</p>

<div class="price">₹199</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Fashion%20Earrings."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 4 -->
<div class="product" data-name="bracelet" data-category="Bracelet">

<img src="https://images.unsplash.com/photo-1573408301185-9146fe634ad0?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Bracelet</div>

<h3>Designer Bracelet</h3>

<p>Beautiful bracelet with premium look.</p>

<div class="price">₹249</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Designer%20Bracelet."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 5 -->
<div class="product" data-name="bangles" data-category="Bangles">

<img src="https://images.unsplash.com/photo-1617038260897-41a1f14a8ca0?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Bangles</div>

<h3>Traditional Bangles</h3>

<p>Beautiful bangles for every occasion.</p>

<div class="price">₹299</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Traditional%20Bangles."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 6 -->
<div class="product" data-name="face wash" data-category="Beauty">

<img src="https://images.unsplash.com/photo-1556228578-8c89e6adf883?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Beauty</div>

<h3>Face Wash</h3>

<p>Daily skincare face wash.</p>

<div class="price">₹149</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Face%20Wash."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 7 -->
<div class="product" data-name="beauty accessories" data-category="Beauty">

<img src="https://images.unsplash.com/photo-1596462502278-27bfdc403348?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Beauty</div>

<h3>Beauty Accessories</h3>

<p>Useful beauty accessories collection.</p>

<div class="price">₹199</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Beauty%20Accessories."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


<!-- PRODUCT 8 -->
<div class="product" data-name="gift set" data-category="Jewellery">

<img src="https://images.unsplash.com/photo-1515562141207-7a88fb7ce338?auto=format&fit=crop&w=700&q=80">

<div class="product-info">

<div class="category-name">Jewellery</div>

<h3>Special Gift Set</h3>

<p>A beautiful gifting option.</p>

<div class="price">₹599</div>

<a class="order-btn"
href="https://wa.me/919999999999?text=Hello%20Sadguru%20Shop,%20I%20want%20to%20order%20Special%20Gift%20Set."
target="_blank">
Order on WhatsApp
</a>

</div>
</div>


</div>
</section>


<!-- FEATURES -->
<section>

<div class="section-title">
<h2>Why Choose Sadguru Shop?</h2>
</div>

<div class="features">

<div class="feature">
<div class="feature-icon">⭐</div>
<h3>Quality Products</h3>
<p>Selected products with good quality.</p>
</div>

<div class="feature">
<div class="feature-icon">💰</div>
<h3>Best Prices</h3>
<p>Affordable prices for everyone.</p>
</div>

<div class="feature">
<div class="feature-icon">📱</div>
<h3>Easy Ordering</h3>
<p>Order easily through WhatsApp.</p>
</div>

<div class="feature">
<div class="feature-icon">❤️</div>
<h3>Customer Service</h3>
<p>We value every customer.</p>
</div>

</div>

</section>


<!-- ABOUT -->
<section class="about" id="about">

<div class="section-title">
<h2>About Sadguru Shop</h2>
</div>

<div class="about-box">

<p>
Welcome to <b>Sadguru Shop</b>.

We offer a variety of products including
fashion jewellery, earrings, bracelets, bangles,
cutlery sets, face wash, beauty accessories and more.

Our goal is to provide useful and stylish products
at reasonable prices with friendly customer service.

</p>

</div>

</section>


<!-- CONTACT -->
<section class="contact" id="contact">

<div class="section-title">
<h2>Contact Us</h2>
<p>We would love to hear from you</p>
</div>

<div class="contact-box">

<div class="contact-item">
📞 Phone:
<a href="tel:+919999999999">+91 99999 99999</a>
</div>

<div class="contact-item">
💬 WhatsApp:
<a href="https://wa.me/919999999999" target="_blank">
Chat With Us
</a>
</div>

<div class="contact-item">
📸 Instagram:
<a href="https://instagram.com/" target="_blank">
@SadguruShop
</a>
</div>

<div class="contact-item">
📍 Address:
Your Shop Address, Maharashtra
</div>

</div>

</section>


<!-- FOOTER -->
<footer>

<h2>Sadguru Shop</h2>

<p>
Jewellery • Accessories • Beauty • Cutlery
</p>

<div class="social">

<a href="#home">Home</a> |
<a href="#products">Products</a> |
<a href="#contact">Contact</a>

</div>

<p>
© 2026 Sadguru Shop. All Rights Reserved.
</p>

</footer>


<!-- FLOATING WHATSAPP -->
<a class="whatsapp"
href="https://wa.me/919999999999"
target="_blank"
title="WhatsApp">
💬
</a>


<script>

/* SEARCH PRODUCTS */

function searchProducts(){

    let input =
    document.getElementById("searchInput")
    .value.toLowerCase();

    let products =
    document.querySelectorAll(".product");

    products.forEach(function(product){

        let name =
        product.getAttribute("data-name")
        .toLowerCase();

        let category =
        product.getAttribute("data-category")
        .toLowerCase();

        if(name.includes(input) || category.includes(input)){
            product.style.display = "block";
        }
        else{
            product.style.display = "none";
        }

    });

}


/* CATEGORY FILTER */

function filterProducts(category){

    let products =
    document.querySelectorAll(".product");

    products.forEach(function(product){

        if(product.getAttribute("data-category") === category){
            product.style.display = "block";
        }
        else{
            product.style.display = "none";
        }

    });

    document
    .getElementById("products")
    .scrollIntoView({
        behavior:"smooth"
    });

}

</script>

</body>
</html>
