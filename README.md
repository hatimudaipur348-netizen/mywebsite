![My Image](image-name.png)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <img src="images/photo.jpg" alt="My Photo">
    <title>[BAKESATION] - Delicious Bakery</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #5a3f2e;
        }
        /* ALL COLORS - EASY TO CHANGE */
        :root {
            --primary: #ff6b6b;
            --secondary: #ffb347;
            --dark: #8b4513;
            --light: #f9dbbd;
        }
        .hero {
            background: linear-gradient(135deg, var(--light) 0%, #e8b4a0 100%);
            padding: 100px 20px;
            text-align: center;
            position: relative;
        }
        .logo {
            font-size: 4em;
            font-weight: bold;
            color: var(--dark);
            margin-bottom: 20px;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        .btn {
            display: inline-block;
            background: linear-gradient(45deg, var(--primary), #ff6b6b);
            color: white;
            padding: 18px 40px;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2em;
            font-weight: bold;
            margin: 0 10px;
            transition: all 0.3s;
            box-shadow: 0 8px 25px rgba(255,107,107,0.4);
        }
        .btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(255,107,107,0.6);
        }
        .container { max-width: 1200px; margin: 0 auto; padding: 0 20px; }
        .section { padding: 80px 0; }
        .section-title {
            text-align: center;
            font-size: 2.5em;
            color: var(--dark);
            margin-bottom: 60px;
            position: relative;
        }
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
        }
        .grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
            gap: 30px; 
            margin-top: 50px; 
        }
        .card {
            background: white;
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 15px 40px rgba(0,0,0,0.1);
            transition: all 0.4s;
        }
        .card:hover {
            transform: translateY(-15px);
            box-shadow: 0 25px 60px rgba(0,0,0,0.2);
        }
        .price { font-size: 1.5em; color: var(--primary); font-weight: bold; margin: 15px 0; }
        .contact { background: linear-gradient(135deg, #f8d7a8 0%, #e8b4a0 100%); }
        footer { background: var(--dark); color: white; text-align: center; padding: 40px 20px; }
        @media (max-width: 768px) { .logo { font-size: 2.5em; } }
    </style>
</head>
<body>
    <!-- 🖌️ HERO SECTION - EDIT HERE -->
    <section class="hero">
        <div class="hero-content" style="max-width: 800px; margin: 0 auto; position: relative; z-index: 2;">
            <h1 class="logo">[🍰 BAKESATION] </h1>
            <h2 style="font-size: 1.8em; color: var(--dark); margin-bottom: 30px;">
                [Where every bite is a sensation] ← YOUR TAGLINE
            </h2>
            <p style="font-size: 1.3em; margin-bottom: 30px; color: #654321;">
                [Freshly baked cakes, pastries & desserts made with love ❤️] 
            </p>
            <a href="#menu" class="btn">[🍪 View Menu]</a>
            <a href="#contact" class="btn">[📞 Contact Us]</a>
        </div>
    </section>

    <div class="container">
        <!-- 🖌️ MENU SECTION - ADD/EDIT ITEMS -->
        <section class="section" id="menu">
            <h2 class="section-title">[🍰 Our Delicious Menu]</h2>
            <div class="grid">
                <!-- MENU ITEM 1 -->
                <div class="card">
                    <div style="font-size: 4em; margin-bottom: 20px;">[🎂]</div>
                    <h3>[
Jeera ajwain cookies- 49RS


Tooty frooty cookies- 49RS


Chocolate chip cookies-49RS 
Oats and seeds cookies
Coconut crunch
Kesar pista cookies
Misri cookies
Rose cookies
Paan cookies
Nankhatai
Butter button cookies
Mini masala biscuits
Muffins Cupcakes
BENTO CAKES
Chocolate Truffle
Rich Chocolate
Classic Vanilla Butterscotch
Blueberry 
Raspberry
Pineapple
Strawberry
Mango
Black Forest
Red Velvet 
Mix fruit
Orange                        ]</h3>
                    <p>[Birthday, wedding, or celebration cakes made to perfection]</p>
                    <div class="price">[STARTING FROM 49 RS]</div>
                </div>
                
                <!-- MENU ITEM 2 - COPY THIS BLOCK TO ADD MORE -->
                <div class="card">
                    <div style="font-size: 4em; margin-bottom: 20px;">[🍪]</div>
                    <h3>[Fresh Cookies]</h3>
                    <p>[Chocolate chip, oatmeal raisin, and more!]</p>
                    <div class="price">[starting from 49rs]</div>
                </div>
                
                <!-- ADD MORE ITEMS BY COPYING ABOVE BLOCK -->
            </div>
        </section>

        <!-- 🖌️ ABOUT SECTION - OPTIONAL -->
        <section class="section">
            <h2 class="section-title">[👩‍🍳 About Bakesation]</h2>
            <div class="grid">
                <div class="card" style="grid-column: span 2;">
                    <p style="font-size: 1.2em;">
                        [[YOUR STORY HERE] - e.g. "Family-owned bakery since 2010. We use only the finest ingredients..."]<br><br>
                        [DELETE THIS WHOLE SECTION IF YOU DON'T WANT IT]
                    </p>
                </div>
            </div>
        </section>

        <!-- 🖌️ CONTACT SECTION -->
        <section class="section contact" id="contact">
            <h2 class="section-title">[📞 Get in Touch]</h2>
            <div class="grid">
                <div class="card">
                    <div style="font-size: 3em; margin-bottom: 20px;">📍</div>
                    <h3>[udaipur]</h3>
                    <p>[305,saifee burhani park ,mahaveer park colony near K9 supermarket navratan bhuwana udaipur 313001]</p>
                </div>
                <div class="card">
                    <div style="font-size: 3em; margin-bottom: 20px;">📱</div>
                    <h3>[+919351863700]</h3>
                    <p>[]</p>
                </div>
                <div class="card">
                    <div style="font-size: 3em; margin-bottom: 20px;">✉️</div>
                    <h3>[hatimudaipur348@gmail.com]</h3>
                    <p>[]</p>
                </div>
                <div class="card">
                    <div style="font-size: 3em; margin-bottom: 20px;">🕒</div>
                    <h3>[Hours]</h3>
                    <p>[24/7<br><br></p>
                </div>
            </div>
        </section>
    </div>

    <!-- 🖌️ FOOTER -->
    <footer>
        <p>&copy; 2024 [BAKESATION]. All rights reserved. [🍪 Made with love & butter!]</p>
    </footer>

    <script>
        // Smooth scrolling - NO NEED TO EDIT
        document.querySelectorAll('a[href^="#"]').forEach(a => {
            a.addEventListener('click', e => {
                e.preventDefault();
                document.querySelector(a.getAttribute('href')).scrollIntoView({behavior: 'smooth'});
            });
        });
    </script>
</body>
</html>
