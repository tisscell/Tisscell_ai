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
