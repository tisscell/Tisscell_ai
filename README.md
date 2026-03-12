/* ROOT VARIABLES - Easy to change colors here */
:root {
    --navy: #0A1F44;
    --gold: #D4AF37;
    --white: #FFFFFF;
    --light-gray: #f4f4f4;
    --transition: all 0.3s ease;
}

* { box-sizing: border-box; margin: 0; padding: 0; }

body {
    font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    line-height: 1.6;
    color: var(--navy);
    background-color: var(--white);
}

/* NAVIGATION */
nav {
    background: var(--navy);
    padding: 1rem 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 1000;
}

nav a { color: white; text-decoration: none; margin-left: 20px; font-weight: 500; }
.logo { color: var(--gold); font-size: 1.5rem; font-weight: bold; }

/* HERO SECTION */
.hero {
    background: linear-gradient(rgba(10,31,68,0.8), rgba(10,31,68,0.8)), url('https://images.unsplash.com/photo-1554224155-169641357599?auto=format&fit=crop&w=1200&q=80');
    background-size: cover;
    color: white;
    padding: 100px 10%;
    text-align: center;
}

.hero h1 { font-size: 3rem; margin-bottom: 1rem; }
.hero span { color: var(--gold); }

/* PINTEREST STYLE GRID */
.container { padding: 50px 10%; }
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 30px;
}

/* CARDS */
.card {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 10px 20px rgba(0,0,0,0.05);
    transition: var(--transition);
    border-bottom: 3px solid transparent;
}

.card:hover {
    transform: translateY(-10px);
    border-color: var(--gold);
}

.card img { width: 100%; height: 200px; object-fit: cover; }
.card-content { padding: 20px; }
.card-tag { color: var(--gold); font-size: 0.8rem; text-transform: uppercase; font-weight: bold; }

/* BUTTONS */
.btn-gold {
    background: var(--gold);
    color: var(--navy);
    padding: 12px 25px;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
    display: inline-block;
    transition: var(--transition);
    border: none;
    cursor: pointer;
}

.btn-gold:hover {
    background: #b8962d;
    transform: scale(1.05);
}

/* FOOTER */
footer { background: var(--navy); color: white; text-align: center; padding: 40px; margin-top: 50px; }

/* RESPONSIVE */
@media (max-width: 768px) {
    .hero h1 { font-size: 2rem; }
    nav { flex-direction: column; }
    nav a { margin: 10px 5px; }
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wealth & Tools | Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <nav>
        <div class="logo">GOLDEN VENTURE</div>
        <div class="links">
            <a href="index.html">Home</a>
            <a href="blog.html">Blog</a>
            <a href="tools.html">Tools</a>
            <a href="about.html">About</a>
        </div>
    </nav>

    <header class="hero">
        <h1>Master Your <span>Digital Revenue</span></h1>
        <p>Expert reviews on tools and strategies to grow your online business.</p>
        <br>
        <a href="blog.html" class="btn-gold">Explore the Blog</a>
    </header>

    <section class="container">
        <h2 style="margin-bottom: 30px;">Latest Insights</h2>
        <div class="grid">
            <div class="card">
                <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=500&q=60" alt="Work from home">
                <div class="card-content">
                    <span class="card-tag">Passive Income</span>
                    <h3>5 Tools to Automate Your Business</h3>
                    <p>Stop doing manual work. These 5 tools saved me 20 hours a week...</p>
                    <br>
                    <a href="post.html" class="btn-gold">Read More</a>
                </div>
            </div>
            </div>
    </section>

    <footer>
        <p>&copy; 2024 Golden Venture Blog. All Rights Reserved.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Post Title - Golden Venture</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <div class="logo">GOLDEN VENTURE</div>
        <div class="links"><a href="index.html">Home</a><a href="blog.html">Blog</a><a href="tools.html">Tools</a></div>
    </nav>

    <article class="container" style="max-width: 800px; margin: auto;">
        <p class="card-tag">Tools & Software</p>
        <h1>How to Start an Affiliate Blog in 2024</h1>
        <img src="https://images.unsplash.com/photo-1499750310107-5fef28a66643?auto=format&fit=crop&w=800&q=80" style="width: 100%; border-radius: 15px; margin: 20px 0;">
        
        <div class="post-text">
            <p>Paste your first paragraph here. Make it engaging to keep readers on the page.</p>
            
            <h2 style="margin: 20px 0;">Why this tool is a game changer</h2>
            <p>Paste more text here about the product or strategy you are promoting.</p>

            <div style="background: var(--light-gray); padding: 30px; border-radius: 10px; text-align: center; margin: 40px 0; border-left: 5px solid var(--gold);">
                <h3>Ready to scale your income?</h3>
                <p>I highly recommend using this software to track your links.</p>
                <br>
                <a href="YOUR_AFFILIATE_LINK_HERE" class="btn-gold">Get the Deal Now</a>
            </div>
        </div>
    </article>

    <footer>
        <p>&copy; 2024 Golden Venture Blog</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recommended Tools</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav>
        <div class="logo">GOLDEN VENTURE</div>
        <div class="links"><a href="index.html">Home</a><a href="blog.html">Blog</a></div>
    </nav>

    <div class="container">
        <h1 style="text-align: center; margin-bottom: 50px;">Top Recommended <span>Tools</span></h1>
        
        <div class="grid">
            <div class="card" style="text-align: center; padding: 20px;">
                <h3>Email Marketing Tool</h3>
                <p>The best way to build your list.</p>
                <br>
                <a href="YOUR_LINK" class="btn-gold">Start for Free</a>
            </div>
            
            <div class="card" style="text-align: center; padding: 20px;">
                <h3>Hosting Provider</h3>
                <p>Fast, reliable, and affordable.</p>
                <br>
                <a href="YOUR_LINK" class="btn-gold">Try This Tool</a>
            </div>
        </div>
    </div>
</body>
</html>
