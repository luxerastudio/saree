<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luxera Studio | Official Store</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <style>
        /* মোবাইলের জন্য হেডার ও টাইটেল ফিক্স */
@media (max-width: 768px) {
    header { display: flex !important; flex-direction: column !important; align-items: center !important; text-align: center !important; }
    .logo { font-size: 20px !important; margin-bottom: 10px !important; } 
    .header-icons { display: flex !important; gap: 20px !important; justify-content: center !important; }
    .header-icons span { display: none !important; } /* শুধু লোগো থাকবে, লেখা মুছে যাবে */
    
    /* টাইটেল ছোট ও এক লাইনে করা */
    .section-title h2 { font-size: 18px !important; white-space: nowrap !important; overflow: hidden !important; text-overflow: ellipsis !important; }
}        * { margin: 0; padding: 0; box-sizing: border-box; outline: none; border: none; text-decoration: none; scroll-behavior: smooth; }
        body { font-family: 'Poppins', sans-serif; background-color: #fffdfa; color: #1a1a1a; overflow-x: hidden; }

        /* --- Header: Premium & Responsive --- */
        header { background: #fff; position: sticky; top: 0; z-index: 1000; box-shadow: 0 2px 15px rgba(0,0,0,0.05); padding: 10px 5%; }
        
        /* Mobile One Line Header */
        .header-top { display: flex; align-items: center; justify-content: space-between; height: 60px; gap: 10px; }
        
        .nav-trigger { width: 40px; }
        .mobile-hamburger { font-size: 22px; color: #8e6d10; cursor: pointer; }

        .logo { 
            font-size: 24px; color: #8e6d10; letter-spacing: 3px; font-weight: 900; 
            font-family: 'Playfair Display', serif; text-transform: uppercase; 
            text-align: center; flex: 1; white-space: nowrap;
        }
        
        .header-right-icons { display: flex; gap: 10px; width: 90px; justify-content: flex-end; }
        .glass-icon { background: rgba(142, 109, 16, 0.05); width: 38px; height: 38px; border-radius: 10px; display: flex; align-items: center; justify-content: center; color: #8e6d10; cursor: pointer; font-size: 16px; }

        /* Long Search Bar */
        .search-row { display: flex; justify-content: center; padding: 10px 0 15px; }
        .search-container { width: 100%; max-width: 850px; position: relative; }
        .search-bar { width: 100%; padding: 14px 25px 14px 55px; border: 1px solid #f0f0f0; border-radius: 30px; background: #fbfbfb; font-size: 14px; box-shadow: inset 0 2px 4px rgba(0,0,0,0.02); }
        .search-icon { position: absolute; left: 22px; top: 50%; transform: translateY(-50%); color: #8e6d10; font-size: 18px; }

        /* PC Navigation */
        .desktop-nav { display: flex; justify-content: space-around; padding: 15px 0; border-top: 1px solid #f5f5f5; }
        .cat-item { color: #444; font-size: 12px; font-weight: 600; text-transform: uppercase; letter-spacing: 1px; transition: 0.3s; }
        .cat-item:hover { color: #8e6d10; }

        /* --- Sliding Mobile Menu --- */
        .side-menu { position: fixed; top: 0; left: -300px; width: 300px; height: 100%; background: #fff; z-index: 2000; transition: 0.5s cubic-bezier(0.4, 0, 0.2, 1); padding: 50px 30px; box-shadow: 10px 0 30px rgba(0,0,0,0.1); }
        .side-menu.active { left: 0; }
        .side-menu h3 { font-family: 'Playfair Display'; color: #8e6d10; font-size: 24px; margin-bottom: 30px; border-bottom: 2px solid #f8f1e0; padding-bottom: 15px; }
        .side-menu a { display: block; padding: 18px 0; color: #333; font-weight: 500; border-bottom: 1px solid #f9f9f9; transition: 0.3s; }
        .side-menu a:hover { padding-left: 10px; color: #8e6d10; }
        .overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.6); z-index: 1500; display: none; backdrop-filter: blur(3px); }
        .overlay.active { display: block; }

        /* --- Hero Slideshow --- */
        .hero { width: 100%; height: 550px; position: relative; overflow: hidden; }
        .slide { position: absolute; width: 100%; height: 100%; opacity: 0; transition: opacity 1.5s ease-in-out; background-size: cover; background-position: center; display: flex; align-items: center; justify-content: center; transform: scale(1.1); }
        .slide.active { opacity: 1; transform: scale(1); transition: opacity 1.5s ease-in-out, transform 8s linear; }
        .slide h2 { color: #fff; font-size: 45px; font-family: 'Playfair Display'; text-align: center; text-shadow: 2px 2px 15px rgba(0,0,0,0.4); letter-spacing: 5px; }

        /* --- Product Grid --- */
        .container { padding: 80px 8%; }
        .section-title { font-size: 28px; text-align: center; margin-bottom: 50px; font-family: 'Playfair Display'; text-transform: uppercase; letter-spacing: 3px; position: relative; }
        .section-title::after { content: ''; width: 60px; height: 2px; background: #8e6d10; position: absolute; bottom: -15px; left: 50%; transform: translateX(-50%); }
        .grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 30px; margin-bottom: 80px; }
        .card { background: #fff; border: 1px solid #f1f1f1; padding: 20px; border-radius: 20px; text-align: center; cursor: pointer; transition: 0.4s; }
        .card:hover { border-color: #8e6d10; transform: translateY(-10px); box-shadow: 0 10px 25px rgba(0,0,0,0.05); }
        .img-box { width: 100%; height: 350px; background: #f9f9f9; border-radius: 15px; margin-bottom: 20px; background-size: cover; background-position: center; }

        /* --- Wide & Premium Footer --- */
        footer { background: #000; color: #fff; padding: 120px 8% 60px; border-top: 5px solid #8e6d10; position: relative; }
        .f-grid { display: grid; grid-template-columns: 1.5fr 1fr 1fr; gap: 80px; }
        .f-col h3 { color: #d4af37; font-size: 26px; margin-bottom: 35px; font-family: 'Playfair Display'; letter-spacing: 2px; }
        .f-col p { color: #999; line-height: 2; font-size: 15px; margin-bottom: 15px; }
        
        .footer-gmail-box { display: flex; margin-top: 30px; position: relative; max-width: 400px; }
        .footer-gmail-box input { width: 100%; padding: 16px 25px; border-radius: 35px; background: #111; border: 1px solid #333; color: #fff; font-size: 14px; outline: none; transition: 0.3s; }
        .footer-gmail-box input:focus { border-color: #d4af37; box-shadow: 0 0 10px rgba(212, 175, 55, 0.2); }
        .footer-gmail-box button { position: absolute; right: 6px; top: 6px; padding: 10px 25px; background: #8e6d10; border-radius: 30px; color: #fff; font-weight: 600; cursor: pointer; transition: 0.3s; }
        .footer-gmail-box button:hover { background: #d4af37; }

        .f-socials { display: flex; gap: 20px; margin-top: 40px; }
        .f-socials a { width: 55px; height: 55px; border-radius: 50%; border: 1px solid #333; display: flex; align-items: center; justify-content: center; color: #fff; font-size: 22px; transition: 0.4s; }
        .f-socials a:hover { background: #8e6d10; border-color: #8e6d10; transform: translateY(-8px); }

        .f-links p { margin-bottom: 12px; transition: 0.3s; cursor: pointer; }
        .f-links p:hover { color: #d4af37; padding-left: 5px; }

        /* --- Modals --- */
        .modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.92); z-index: 3000; align-items: center; justify-content: center; padding: 20px; backdrop-filter: blur(5px); }
        .modal-content { background: #fff; width: 100%; max-width: 900px; display: flex; border-radius: 25px; overflow: hidden; position: relative; max-height: 90vh; }
        .modal-img { width: 45%; background-size: cover; background-position: center; }
        .modal-info { width: 55%; padding: 50px; overflow-y: auto; }

        @media (max-width: 768px) {
            .logo { font-size: 20px; }
            .desktop-nav { display: none; }
            .grid { grid-template-columns: repeat(2, 1fr); gap: 15px; }
            .f-grid { grid-template-columns: 1fr; gap: 60px; }
            .modal-content { flex-direction: column; }
            .modal-img { width: 100%; height: 280px; }
            .modal-info { width: 100%; padding: 30px; }
            footer { padding: 80px 8% 40px; }
            .hero { height: 350px; }
            .slide h2 { font-size: 28px; }
            
           /* LUXERA MOBILE FINAL PREMIUM FIX (ONLY FOR MOBILE) */
    @media (max-width: 768px) {
        /* ১. ব্র্যান্ডের নাম মাঝখানে এবং আইকন ছোট করা */
        header, .header-container { 
            display: flex !important; 
            flex-direction: column !important; 
            align-items: center !important; 
            padding: 10px 0 !important;
        }
        .logo, .logo-text { 
            font-size: 22px !important; 
            margin-bottom: 10px !important; 
            text-align: center !important;
            width: 100% !important;
        }
        .header-icons { 
            display: flex !important; 
            gap: 25px !important; 
            justify-content: center !important;
            width: 100% !important;
        }
        .header-icons a span, .header-icons span { 
            display: none !important; /* লগইন ও কার্ট লেখা মুছে শুধু লোগো থাকবে */
        }
        .header-icons i {
            font-size: 20px !important;
        }

        /* ২. টাইটেল ছোট ও এক লাইনে করা (যেমন: গর্জিয়াস পার্টি ওয়্যার) */
        .section-title h2, h2.section-title { 
            font-size: 18px !important; 
            white-space: nowrap !important; 
            overflow: hidden !important; 
            text-overflow: ellipsis !important; 
            text-align: center !important;
            padding: 0 10px !important;
            margin-bottom: 20px !important;
        }

        /* ৩. প্রোডাক্ট বক্স প্রিমিয়াম ও সাইজ ছোট করা */
        .grid, .product-grid { 
            display: grid !important; 
            grid-template-columns: repeat(2, 1fr) !important; /* এক লাইনে ২টা বক্স */
            gap: 12px !important; 
            padding: 10px !important;
        }
        .card, .product-card { 
            background: #fff !important;
            border-radius: 12px !important; 
            box-shadow: 0 4px 12px rgba(0,0,0,0.06) !important; 
            border: 1px solid #f2f2f2 !important;
            padding: 8px !important;
            margin: 0 !important;
            overflow: hidden !important;
        }
        .card img, .product-image { 
            height: 160px !important; 
            border-radius: 8px !important;
            object-fit: cover !important;
        }
        .card h3, .product-name { 
            font-size: 13px !important; 
            margin: 8px 0 4px !important;
            height: 35px;
            overflow: hidden;
        }
        .price { font-size: 14px !important; font-weight: 700 !important; }
    }
  </style>
</head>
<body>

    <div class="overlay" id="overlay" onclick="toggleMenu()"></div>
    <div class="side-menu" id="sideMenu">
        <h3>Menu</h3>
        <a href="#party" onclick="toggleMenu()">Party Wear</a>
        <a href="#bridal" onclick="toggleMenu()">Bridal Layer</a>
        <a href="#silk" onclick="toggleMenu()">Luxury Silk</a>
        <a href="#" onclick="toggleMenu()">New Arrivals</a>
        <a href="#" onclick="toggleMenu()">Member Access</a>
        <a href="#" onclick="toggleMenu()">Contact Us</a>
    </div>

    <header>
        <div class="header-top">
            <div class="nav-trigger"><i class="fas fa-bars mobile-hamburger" onclick="toggleMenu()"></i></div>
            <div class="logo">LUXERA STUDIO</div>
            <div class="header-right-icons">
                <div class="glass-icon" onclick="openModal('authModal')"><i class="fas fa-user"></i></div>
                <div class="glass-icon"><i class="fas fa-shopping-bag"></i></div>
            </div>
        </div>
        <div class="search-row">
            <div class="search-container">
                <i class="fas fa-search search-icon"></i>
                <input type="text" id="searchInput" class="search-bar" placeholder="Search by product code or name..." onkeyup="filterItems()">
            </div>
        </div>
        <nav class="desktop-nav">
            <a href="#party" class="cat-item">Gorgeous Party Wear</a>
            <a href="#bridal" class="cat-item">Exclusive Bridal Layer</a>
            <a href="#silk" class="cat-item">Luxury Silk Saree</a>
            <a href="#" class="cat-item">Collection</a>
            <a href="#" class="cat-item">Contact</a>
        </nav>
    </header>

    <div class="hero">
        <div class="slide active" style="background-image: linear-gradient(rgba(0,0,0,0.3),rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1610030469983-98e550d6193c?w=1600')">
            <h2>The Art of Royalty</h2>
        </div>
        <div class="slide" style="background-image: linear-gradient(rgba(0,0,0,0.3),rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1583391733959-1c5861b369c6?w=1600')">
            <h2>Exquisite Elegance</h2>
        </div>
    </div>

    <div class="container">
        <h2 class="section-title" id="party">Gorgeous Party Wear</h2>
        <div class="grid" id="gridParty"></div>

        <h2 class="section-title" id="bridal">Exclusive Bridal Layer</h2>
        <div class="grid" id="gridBridal"></div>

        <h2 class="section-title" id="silk">Luxury Silk Saree</h2>
        <div class="grid" id="gridSilk"></div>
    </div>

    <div class="modal" id="pModal">
        <div class="modal-content">
            <span onclick="closeModal('pModal')" style="position:absolute; top:20px; right:30px; font-size:40px; cursor:pointer; z-index:100;">&times;</span>
            <div class="modal-img" id="modalImg"></div>
            <div class="modal-info">
                <h2 id="mTitle" style="font-family:'Playfair Display'; font-size:32px; margin-bottom:15px;">Product Name</h2>
                <p id="mPrice" style="font-size:32px; color:#8e6d10; font-weight:700;">৳ 0</p>
                <p id="mCode" style="color:red; font-weight:600; margin-bottom:25px; letter-spacing:1px;">CODE: 000</p>
                <div style="font-size:15px; border-top:1px solid #eee; padding-top:20px;">
                    <p style="margin-bottom:12px;"><b>Color:</b> <span id="mColor">Premium Shade</span></p>
                    <p style="margin-bottom:12px;"><b>Includes:</b> Saree only</p>
                    <p style="margin-bottom:12px;"><b>Fabric:</b> Handcrafted Luxury Silk</p>
                    <p style="margin-bottom:12px;"><b>Work:</b> Detailed Zari Embroidery</p>
                </div>
                <a href="#" id="waLink" style="background:#000; color:#fff; display:block; text-align:center; padding:18px; border-radius:12px; margin-top:35px; font-weight:600; letter-spacing:1px;" target="_blank">ORDER VIA WHATSAPP</a>
            </div>
        </div>
    </div>

    <div class="modal" id="authModal">
        <div style="background:#fff; padding:50px; border-radius:30px; width:400px; text-align:center; position:relative;">
            <span onclick="closeModal('authModal')" style="position:absolute; top:20px; right:25px; cursor:pointer; font-size:25px;">&times;</span>
            <h2 style="font-family:'Playfair Display'; color:#8e6d10; margin-bottom:25px;">Customer Login</h2>
            <input type="email" placeholder="Email Address" style="width:100%; padding:14px; margin-bottom:15px; border:1px solid #ddd; border-radius:10px;">
            <input type="password" placeholder="Password" style="width:100%; padding:14px; margin-bottom:25px; border:1px solid #ddd; border-radius:10px;">
            <button style="background:#000; color:#fff; width:100%; padding:14px; border-radius:10px; cursor:pointer; font-weight:600;">ACCESS ACCOUNT</button>
        </div>
    </div>

   <footer style="background-color: #ffffff; padding: 60px 0 30px 0; font-family: 'Poppins', sans-serif; border-top: 1px solid #eee; margin-top: 40px; width: 100%;">
    
    <div style="text-align: center; max-width: 800px; margin: 0 auto 40px auto; padding: 0 20px;">
        <h3 style="font-family: 'Playfair Display', serif; font-size: 28px; color: #111; margin-bottom: 10px; font-weight: 700;">Subscribe to Our Newsletter</h3>
        
        <div style="display: flex; justify-content: center; max-width: 450px; margin: 20px auto; border: 1px solid #000; padding: 3px; background: #fff;">
            <input type="email" placeholder="Your email address" style="flex: 1; border: none; padding: 10px; outline: none; font-size: 14px; width: 50%;">
            <button style="background: #000; color: #fff; border: none; padding: 0 20px; cursor: pointer; text-transform: uppercase; font-size: 12px; font-weight: 600;">Subscribe</button>
        </div>

        <div style="margin-top: 35px;">
            <a href="https://www.facebook.com/luxerasaree/" style="color: #1877F2; margin: 0 12px; font-size: 26px; text-decoration: none;" target="_blank"><i class="fab fa-facebook"></i></a>
            <a href="#" style="color: #E4405F; margin: 0 12px; font-size: 26px; text-decoration: none;" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="https://www.youtube.com/" style="color: #FF0000; margin: 0 12px; font-size: 26px; text-decoration: none;" target="_blank"><i class="fab fa-youtube"></i></a>
            <a href="https://wa.me/8801961454604" style="color: #25D366; margin: 0 12px; font-size: 26px; text-decoration: none;" target="_blank"><i class="fab fa-whatsapp"></i></a>
        </div>
    </div>

    <div class="footer-grid-container">
        
        <div class="footer-col">
            <h4>Luxera Studio</h4>
            <p>Dhaka, Bangladesh<br>contact@luxera.fashion<br>01961454604</p>
        </div>

        <div class="footer-col">
            <h4>Quick Links</h4>
            <ul>
                <li>Who We Are</li>
                <li>Refund Policy</li>
                <li>Shipping Policy</li>
            </ul>
        </div>

        <div class="footer-col">
            <h4>Policies</h4>
            <ul>
                <li>Privacy Policy</li>
                <li>Terms & Conditions</li>
            </ul>
        </div>

        <div class="footer-col">
            <h4>Get Our App</h4>
            <div class="app-badges">
                <img src="https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg" alt="Play Store">
                <img src="https://upload.wikimedia.org/wikipedia/commons/3/3c/Download_on_the_App_Store_Badge.svg" alt="App Store">
            </div>
        </div>
    </div>

    <div style="text-align: center; margin-top: 50px; font-size: 11px; color: #bbb; letter-spacing: 1px;">
        &copy; 2026 LUXERA STUDIO. ALL RIGHTS RESERVED.
    </div>
</footer>

<style>
    /* পিসি এবং মোবাইলের জন্য কমন স্টাইল */
    .footer-grid-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 20px;
        text-align: center; /* সব টেক্সট মাঝখানে */
    }
    .footer-col {
        flex: 1;
        min-width: 250px;
        margin-bottom: 30px;
        display: flex;
        flex-direction: column;
        align-items: center; /* মোবাইলে আইটেম মাঝখানে */
    }
    .footer-col h4 {
        font-size: 14px;
        margin-bottom: 20px;
        font-weight: 700;
        text-transform: uppercase;
        color: #111;
    }
    .footer-col p, .footer-col ul {
        font-size: 13px;
        color: #777;
        line-height: 2.5;
        list-style: none;
        padding: 0;
    }
    .app-badges img {
        width: 130px;
        margin: 5px 0;
        display: block;
    }

    /* মোবাইল ভার্সনের জন্য বিশেষ নির্দেশ */
    @media (max-width: 768px) {
        .footer-col {
            flex: 0 0 100%; /* মোবাইলে পুরো জায়গা নেবে */
            margin-bottom: 40px;
        }
        .footer-grid-container {
            flex-direction: column; /* লম্বা লম্বি সাজাবে */
        }
    }
</style>    
    <style>
    .floating-wa { position: fixed; bottom: 85px; right: 20px; background: #25D366; color: #fff; width: 55px; height: 55px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 30px; box-shadow: 0 4px 10px rgba(0,0,0,0.2); z-index: 9999; text-decoration: none; }
    .mobile-sticky-nav { position: fixed; bottom: 0; left: 0; width: 100%; background: #fff; display: flex; justify-content: space-around; padding: 12px 0; border-top: 1px solid #eee; z-index: 9998; box-shadow: 0 -2px 10px rgba(0,0,0,0.05); }
    .mobile-sticky-nav a { text-decoration: none; color: #111; text-align: center; font-size: 10px; flex: 1; }
    .mobile-sticky-nav i { display: block; font-size: 18px; color: #d4af37; margin-bottom: 4px; }
    @media (min-width: 769px) { .mobile-sticky-nav { display: none; } }
</style>

<a href="https://wa.me/8801961454604" class="floating-wa" target="_blank">
    <i class="fab fa-whatsapp"></i>
</a>

<div class="mobile-sticky-nav">
    <a href="#"><i class="fas fa-home"></i><span>Home</span></a>
    <a href="#"><i class="fas fa-search"></i><span>Search</span></a>
    <a href="https://wa.me/8801961454604"><i class="fab fa-whatsapp"></i><span>Chat</span></a>
    <a href="#"><i class="fas fa-user"></i><span>Account</span></a>
</div>
    <script>
        // Sidebar Navigation Logic
        function toggleMenu() {
            document.getElementById('sideMenu').classList.toggle('active');
            document.getElementById('overlay').classList.toggle('active');
        }

        // Automatic Hero Slideshow
        let sIdx = 0;
        const slides = document.querySelectorAll('.slide');
        setInterval(() => {
            slides[sIdx].classList.remove('active');
            sIdx = (sIdx + 1) % slides.length;
            slides[sIdx].classList.add('active');
        }, 5000);

        // Grid Generation with 24 Products
        const sections = [
            { id: 'gridParty', prefix: 'PT', title: 'Party Wear' },
            { id: 'gridBridal', prefix: 'BR', title: 'Bridal Layer' },
            { id: 'gridSilk', prefix: 'SL', title: 'Silk Saree' }
        ];

        sections.forEach(sec => {
            let grid = document.getElementById(sec.id);
            for(let i=1; i<=8; i++) {
                let code = sec.prefix + "-" + (100 + i);
                let price = (sec.prefix === 'BR' ? '28,500' : '12,500');
                let name = "Luxera Exclusive " + sec.title;
                grid.innerHTML += `
                    <div class="card" onclick="openDetails('${name}', '${price}', '${code}')">
                        <div class="img-box" style="background-image: url('https://via.placeholder.com/400x500/f9f9f9/8e6d10?text=${sec.prefix}+${i}')"></div>
                        <p style="color:red; font-size:11px; font-weight:600;">CODE: ${code}</p>
                        <h4 style="font-size:16px; margin:10px 0; font-family:'Playfair Display'">${name}</h4>
                        <p style="color:#8e6d10; font-weight:700; font-size:18px;">৳ ${price}</p>
                    </div>`;
            }
        });

        // Modal Functionalities
        function openDetails(name, price, code) {
            document.getElementById('mTitle').innerText = name;
            document.getElementById('mPrice').innerText = "৳ " + price;
            document.getElementById('mCode').innerText = "CODE: " + code;
            document.getElementById('mColor').innerText = "Premium Royal Shade";
            document.getElementById('modalImg').style.backgroundImage = `url('https://via.placeholder.com/400x500/f9f9f9/8e6d10?text=${code}')`;
            document.getElementById('waLink').href = "https://wa.me/8801961454604?text=Order: " + name + " (" + code + ")";
            document.getElementById('pModal').style.display = 'flex';
        }

        function openModal(id) { document.getElementById(id).style.display = 'flex'; }
        function closeModal(id) { document.getElementById(id).style.display = 'none'; }

        // Search Filter Logic
        function filterItems() {
            let val = document.getElementById('searchInput').value.toUpperCase();
            document.querySelectorAll('.card').forEach(card => {
                card.style.display = card.innerText.toUpperCase().includes(val) ? "block" : "none";
            });
        }
    </script>
</body>
</html>
