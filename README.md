<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="description" content="Sadguru Shop - Jewellery, Earrings, Bracelets, Bangles, Facewash and Beauty Products">

<title>Sadguru Shop | Jewellery & Beauty Collection</title>

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
    font-family:Arial,Helvetica,sans-serif;
    background:#fffaf3;
    color:#251b16;
    line-height:1.6;
}

a{
    text-decoration:none;
    color:inherit;
}

/* HEADER */
header{
    position:sticky;
    top:0;
    z-index:1000;
    background:#19110d;
    box-shadow:0 4px 20px rgba(0,0,0,.25);
}

.navbar{
    max-width:1200px;
    margin:auto;
    padding:15px 20px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-family:Georgia,serif;
    font-size:29px;
    font-weight:bold;
    color:#e9b94e;
}

.nav-links{
    display:flex;
    gap:25px;
    color:white;
}

.nav-links a{
    font-size:15px;
    transition:.3s;
}

.nav-links a:hover{
    color:#e9b94e;
}

.menu{
    display:none;
    color:white;
    font-size:28px;
    cursor:pointer;
}

/* HERO */
.hero{
    min-height:620px;
    display:flex;
    align-items:center;
    background:
    linear-gradient(rgba(25,17,13,.72),rgba(25,17,13,.72)),
    url("images/product-1.jpg") center/cover no-repeat;
}

.hero-content{
    max-width:1200px;
    width:100%;
    margin:auto;
    padding:70px 20px;
    color:white;
}

.badge{
    display:inline-block;
    padding:8px 15px;
    border:1px solid #e9b94e;
    border-radius:30px;
    color:#e9b94e;
    font-size:13px;
    letter-spacing:2px;
}

.hero h1{
    font-family:Georgia,serif;
    font-size:clamp(48px,8vw,82px);
    line-height:1;
    margin:20px 0;
}

.hero p{
    max-width:600px;
    font-size:18px;
    color:#f6eee7;
}

.buttons{
    margin-top:30px;
    display:flex;
    gap:12px;
    flex-wrap:wrap;
}

.btn{
    display:inline-block;
    padding:13px 22px;
    border-radius:30px;
    font-weight:bold;
}

.gold-btn{
    background:#d29b2f;
    color:#18110d;
}

.dark-btn{
    border:1px solid #d29b2f;
    color:white;
}

/* COMMON SECTION */
.section{
    max-width:1200px;
    margin:auto;
    padding:75px 20px;
}

.title{
    text-align:center;
    margin-bottom:40px;
}

.title span{
    color:#c58d25;
    font-size:13px;
    font-weight:bold;
    letter-spacing:2px;
}

.title h2{
    font-family:Georgia,serif;
    font-size:42px;
    margin:5px 0;
}

.title p{
    color:#766b63;
    max-width:700px;
    margin:auto;
}

/* CATEGORIES */
.categories{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:15px;
}

.category{
    background:white;
    border:1px solid #eadccf;
    border-radius:18px;
    padding:25px 15px;
    text-align:center;
    cursor:pointer;
    transition:.3s;
}

.category:hover{
    transform:translateY(-5px);
    box-shadow:0 12px 30px rgba(0,0,0,.1);
}

.category-icon{
    font-size:40px;
}

.category h3{
    margin-top:8px;
    font-size:17px;
}

/* PRODUCTS */
.products{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:22px;
}

.product{
    background:white;
    border:1px solid #eadccf;
    border-radius:18px;
    overflow:hidden;
    box-shadow:0 5px 20px rgba(0,0,0,.07);
    transition:.3s;
}

.product:hover{
    transform:translateY(-5px);
}

.product img{
    width:100%;
    height:270px;
    object-fit:cover;
    display:block;
}

.product-info{
    padding:17px;
}

.product-info h3{
    font-family:Georgia,serif;
    font-size:20px;
}

.product-info p{
    color:#776b63;
    font-size:14px;
    margin:5px 0 14px;
}

.product-buttons{
    display:flex;
    gap:8px;
}

.product-btn{
    flex:1;
    text-align:center;
    padding:9px;
    border-radius:25px;
    background:#fff4df;
    border:1px solid #e8cf9d;
    font-size:13px;
    font-weight:bold;
}

.whatsapp{
    background:#e8f8ed;
    border-color:#b7dfc0;
}

/* ABOUT */
.about{
    background:#201510;
    color:white;
}

.about-inner{
    max-width:1200px;
    margin:auto;
    padding:70px 20px;
}

.about-grid{
    display:grid;
    grid-template-columns:1.1fr .9fr;
    gap:40px;
    align-items:center;
}

.about h2{
    font-family:Georgia,serif;
    color:#e9b94e;
    font-size:45px;
    margin:15px 0;
}

.about p{
    color:#eadfd8;
    font-size:17px;
}

.info-box{
    background:white;
    color:#251b16;
    border-radius:20px;
    padding:25px;
}

.info-row{
    padding:13px 0;
    border-bottom:1px solid #eee;
}

.info-row:last-child{
    border-bottom:0;
}

/* CONTACT */
.contact{
    background:white;
}

.contact-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.contact-card{
    text-align:center;
    padding:28px 20px;
    border:1px solid #eadccf;
    border-radius:18px;
}

.contact-icon{
    font-size:38px;
}

.contact-card h3{
    margin:8px 0;
}

.contact-card p{
    color:#766b63;
}

/* FOOTER */
footer{
    background:#120c09;
    color:#ddd;
    text-align:center;
    padding:25px 15px;
}

/* FLOATING BUTTONS */
.floating{
    position:fixed;
    right:18px;
    bottom:18px;
    display:flex;
    flex-direction:column;
    gap:10px;
    z-index:999;
}

.float-btn{
    width:52px;
    height:52px;
    border-radius:50%;
    display:grid;
    place-items:center;
    color:white;
    font-size:23px;
    box-shadow:0 5px 15px rgba(0,0,0,.25);
}

.float-wa{
    background:#25d366;
}

.float-call{
    background:#c9952e;
}

/* MOBILE */
@media(max-width:950px){

    .products{
        grid-template-columns:repeat(3,1fr);
    }

    .categories{
        grid-template-columns:repeat(3,1fr);
    }
}

@media(max-width:650px){

    .navbar{
        padding:13px 15px;
    }

    .logo{
        font-size:24px;
    }

    .menu{
        display:block;
    }

    .nav-links{
        display:none;
        position:absolute;
        top:60px;
        left:0;
        right:0;
        background:#19110d;
        flex-direction:column;
        padding:20px;
        gap:18px;
    }

    .nav-links.show{
        display:flex;
    }

    .hero{
        min-height:540px;
    }

    .hero-content{
        padding:50px 20px;
    }

    .hero h1{
        font-size:52px;
    }

    .hero p{
        font-size:16px;
    }

    .section{
        padding:55px 15px;
    }

    .title h2{
        font-size:34px;
    }

    .categories{
        grid-template-columns:repeat(2,1fr);
    }

    .products{
        grid-template-columns:repeat(2,1fr);
        gap:12px;
    }

    .product img{
        height:210px;
    }

    .product-info{
        padding:12px;
    }

    .product-info h3{
        font-size:17px;
    }

    .product-info p{
        font-size:12px;
    }

    .product-buttons{
        flex-direction:column;
    }

    .about-grid{
        grid-template-columns:1fr;
    }

    .about h2{
        font-size:36px;
    }

    .contact-grid{
        grid-template-columns:1fr;
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
<nav class="navbar">

<a href="#home" class="logo">Sadguru Shop</a>

<div class="menu" onclick="openMenu()">☰</div>

<div class="nav-links" id="navLinks">
<a href="#home">Home</a>
<a href="#categories">Categories</a>
<a href="#products">Products</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>
</div>

</nav>
</header>


<!-- HERO -->
<section class="hero" id="home">

<div class="hero-content">

<span class="badge">
STYLE • BEAUTY • COLLECTION
</span>

<h1>Sadguru Shop</h1>

<p>
Discover beautiful jewellery, earrings, bracelets, bangles,
facewash and beauty products — all in one place.
</p>

<div class="buttons">

<a href="#products" class="btn gold-btn">
View Collection
</a>

<a href="https://wa.me/919667486365"
target="_blank"
class="btn dark-btn">
WhatsApp Us
</a>

</div>

</div>

</section>


<!-- CATEGORIES -->
<section class="section" id="categories">

<div class="title">

<span>OUR COLLECTION</span>

<h2>Shop by Category</h2>

<p>
Explore our jewellery, fashion accessories and beauty collection.
</p>

</div>


<div class="categories">

<div class="category" onclick="filterProducts('Jewellery')">
<div class="category-icon">💎</div>
<h3>Jewellery</h3>
</div>

<div class="category" onclick="filterProducts('Earrings')">
<div class="category-icon">✨</div>
<h3>Earrings</h3>
</div>

<div class="category" onclick="filterProducts('Bracelets')">
<div class="category-icon">📿</div>
<h3>Bracelets</h3>
</div>

<div class="category" onclick="filterProducts('Bangles')">
<div class="category-icon">⭕</div>
<h3>Bangles</h3>
</div>

<div class="category" onclick="filterProducts('Beauty')">
<div class="category-icon">🧴</div>
<h3>Facewash & Beauty</h3>
</div>

</div>

</section>


<!-- PRODUCTS -->
<section class="section" id="products">

<div class="title">

<span>FEATURED PRODUCTS</span>

<h2>Our Collection</h2>

<p>
For price, colour, size and availability, contact Sadguru Shop.
</p>

</div>


<div class="products" id="productGrid">


<!-- PRODUCT 1 -->

<div class="product" data-category="Jewellery">

<img src="images/product-1.jpg"
alt="Traditional Jewellery Set">

<div class="product-info">

<h3>Traditional Jewellery Set</h3>

<p>
Beautiful necklace set with matching earrings.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365?text=Hello%20Sadguru%20Shop%2C%20I%20want%20to%20know%20about%20the%20Traditional%20Jewellery%20Set."
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 2 -->

<div class="product" data-category="Bangles">

<img src="images/product-2.jpg"
alt="Gold Bangles">

<div class="product-info">

<h3>Classic Gold Bangles</h3>

<p>
Elegant bangles for everyday styling.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 3 -->

<div class="product" data-category="Bangles">

<img src="images/product-3.jpg"
alt="Gold Bangle Set">

<div class="product-info">

<h3>Gold Bangle Set</h3>

<p>
Stylish bangle collection with polished finish.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 4 -->

<div class="product" data-category="Bracelets">

<img src="images/product-4.jpg"
alt="Designer Bracelets">

<div class="product-info">

<h3>Designer Bracelets</h3>

<p>
Fancy stone-studded bracelet designs.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 5 -->

<div class="product" data-category="Jewellery">

<img src="images/product-5.jpg"
alt="Butterfly Necklace">

<div class="product-info">

<h3>Butterfly Necklace</h3>

<p>
Delicate necklace with butterfly charms.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 6 -->

<div class="product" data-category="Bangles">

<img src="images/product-6.jpg"
alt="Stone Bangles">

<div class="product-info">

<h3>Stone Bangles</h3>

<p>
Colourful stone-work bangle designs.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 7 -->

<div class="product" data-category="Bangles">

<img src="images/product-7.jpg"
alt="Traditional Bangles">

<div class="product-info">

<h3>Traditional Bangles</h3>

<p>
Traditional designs with colourful stones.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 8 -->

<div class="product" data-category="Jewellery">

<img src="images/product-8.jpg"
alt="Fashion Jewellery">

<div class="product-info">

<h3>Fashion Jewellery</h3>

<p>
Fancy jewellery for parties and functions.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 9 -->

<div class="product" data-category="Bracelets">

<img src="images/product-9.jpg"
alt="Fashion Collection">

<div class="product-info">

<h3>Fashion Collection</h3>

<p>
Trendy designs for a modern look.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


<!-- PRODUCT 10 -->

<div class="product" data-category="Bangles">

<img src="images/product-10.jpg"
alt="Premium Bangle Collection">

<div class="product-info">

<h3>Premium Bangle Collection</h3>

<p>
Statement designs for festive occasions.
</p>

<div class="product-buttons">

<a class="product-btn whatsapp"
href="https://wa.me/919667486365"
target="_blank">
WhatsApp
</a>

<a class="product-btn"
href="tel:9767486365">
Call
</a>

</div>

</div>
</div>


</div>

</section>


<!-- ABOUT -->
<section class="about" id="about">

<div class="about-inner">

<div class="about-grid">

<div>

<span class="badge">
ABOUT SADGURU SHOP
</span>

<h2>
Style for every occasion.
</h2>

<p>
Sadguru Shop offers jewellery, earrings, bracelets,
bangles, facewash and other fashion and beauty products.
Explore our collection and contact us for product
availability and current prices.
</p>

</div>


<div class="info-box">

<div class="info-row">

<strong>📍 Shop Location</strong>

<br>

Ashoknagar Bhaji Market,
Nagre Chowk,
Behind Kadam Jewellers

</div>


<div class="info-row">

<strong>📞 Call</strong>

<br>

<a href="tel:9767486365">
9767486365
</a>

<br>

<a href="tel:9665029894">
9665029894
</a>

</div>


<div class="info-row">

<strong>💬 WhatsApp</strong>

<br>

<a href="https://wa.me/919667486365"
target="_blank">
9767486365
</a>

<br>

<a href="https://wa.me/919665029894"
target="_blank">
9665029894
</a>

</div>

</div>

</div>

</div>

</section>


<!-- CONTACT -->
<section class="section contact" id="contact">

<div class="title">

<span>GET IN TOUCH</span>

<h2>Visit or Contact Us</h2>

<p>
For product photos, prices and availability,
message us on WhatsApp or call.
</p>

</div>


<div class="contact-grid">


<div class="contact-card">

<div class="contact-icon">
📍
</div>

<h3>Shop Location</h3>

<p>
Ashoknagar Bhaji Market<br>
Nagre Chowk<br>
Behind Kadam Jewellers
</p>

</div>


<div class="contact-card">

<div class="contact-icon">
💬
</div>

<h3>WhatsApp</h3>

<p>

<a href="https://wa.me/919667486365"
target="_blank">
9767486365
</a>

<br>

<a href="https://wa.me/919665029894"
target="_blank">
9665029894
</a>

</p>

</div>


<div class="contact-card">

<div class="contact-icon">
📞
</div>

<h3>Call Us</h3>

<p>

<a href="tel:9767486365">
9767486365
</a>

<br>

<a href="tel:9665029894">
9665029894
</a>

</p>

</div>


</div>

</section>


<!-- FOOTER -->
<footer>

<p>
© <span id="year"></span> Sadguru Shop. All Rights Reserved.
</p>

<p style="font-size:13px;margin-top:5px;">
Jewellery • Earrings • Bracelets • Bangles • Facewash & Beauty
</p>

</footer>


<!-- FLOATING BUTTONS -->

<div class="floating">

<a class="float-btn float-wa"
href="https://wa.me/919667486365"
target="_blank">
💬
</a>

<a class="float-btn float-call"
href="tel:9767486365">
☎
</a>

</div>


<script>

function openMenu(){

    document
    .getElementById("navLinks")
    .classList.toggle("show");

}


function filterProducts(category){

    const products =
    document.querySelectorAll(".product");

    products.forEach(function(product){

        if(product.dataset.category === category){

            product.style.display = "block";

        }else{

            product.style.display = "none";

        }

    });

    document
    .getElementById("products")
    .scrollIntoView({
        behavior:"smooth"
    });

}


document.getElementById("year").textContent =
new Date().getFullYear();

</script>

</body>
</html>
