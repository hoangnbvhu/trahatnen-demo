/* ======== GLOBAL STYLES & VARIABLES ======== */
:root {
    --charcoal-gray: #36454F;
    --off-white: #F8F6F2; /* Slightly warmer than F5F5DC */
    --matcha-green: #3D550C;
    --muted-gold: #B08D57;
    --light-gray: #EAEAEA;
    --font-serif: 'Playfair Display', serif;
    --font-sans: 'Montserrat', sans-serif;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    font-size: 16px;
}

body {
    font-family: var(--font-sans);
    background-color: var(--off-white);
    color: var(--charcoal-gray);
    line-height: 1.7;
}

.container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 2rem;
}

.section-padding {
    padding: 6rem 0;
}

.section-title {
    font-family: var(--font-serif);
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 2rem;
    color: var(--charcoal-gray);
}

.text-center {
    text-align: center;
}

.bg-light {
    background-color: #fff;
}

/* ======== HEADER ======== */
.main-header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 100;
    padding: 1rem 0;
    transition: background-color 0.4s ease, padding 0.4s ease;
}

.main-header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-family: var(--font-serif);
    font-size: 1.8rem;
    font-weight: 700;
    color: #fff;
    text-decoration: none;
}

.main-nav ul {
    list-style: none;
    display: flex;
}

.main-nav ul li {
    margin-left: 2rem;
}

.main-nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: 400;
    padding-bottom: 5px;
    border-bottom: 2px solid transparent;
    transition: border-color 0.3s ease;
}

.main-nav ul li a:hover {
    border-color: var(--muted-gold);
}

/* Scrolled header style */
body.scrolled .main-header {
    background-color: rgba(54, 69, 79, 0.95);
    padding: 0.5rem 0;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

/* ======== HERO SECTION ======== */
#hero {
    height: 100vh;
    background: url('images/hero-bg.jpg') no-repeat center center/cover;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #fff;
    text-align: center;
}

.hero-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
}

.hero-content {
    position: relative;
    z-index: 1;
}

.hero-title {
    font-family: var(--font-serif);
    font-size: 4.5rem;
    font-weight: 700;
    margin-bottom: 1rem;
}

.hero-subtitle {
    font-size: 1.2rem;
    font-weight: 300;
    margin-bottom: 2rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
}

.cta-button {
    display: inline-block;
    background-color: var(--muted-gold);
    color: #fff;
    padding: 1rem 2.5rem;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 500;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.cta-button:hover {
    background-color: #c9a56b;
    transform: translateY(-3px);
}

/* ======== PHILOSOPHY SECTION ======== */
#philosophy .section-intro {
    max-width: 700px;
    margin: 0 auto;
    font-size: 1.1rem;
    font-style: italic;
    color: #555;
}

/* ======== PRODUCTS SECTION ======== */
.product-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
}

.product-card {
    background-color: #fff;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
}

.product-image img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    display: block;
}

.product-info {
    padding: 1.5rem;
    text-align: center;
}

.product-info h3 {
    font-family: var(--font-serif);
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
}

.product-info p {
    color: #777;
    margin-bottom: 1rem;
}

.btn-secondary {
    display: inline-block;
    color: var(--muted-gold);
    text-decoration: none;
    font-weight: 500;
    border: 1px solid var(--muted-gold);
    padding: 0.5rem 1.5rem;
    border-radius: 5px;
    transition: background-color 0.3s, color 0.3s;
}

.btn-secondary:hover {
    background-color: var(--muted-gold);
    color: #fff;
}

/* ======== PROCESS SECTION ======== */
.process-container {
    display: flex;
    justify-content: space-between;
    text-align: center;
    gap: 2rem;
}

.process-step {
    flex-basis: 23%;
}

.process-icon {
    font-size: 3rem;
    color: var(--matcha-green);
    margin-bottom: 1rem;
}

.process-step h3 {
    font-family: var(--font-serif);
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
}

/* ======== BLOG SECTION ======== */
.blog-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
}

.blog-post {
    background: #fff;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
}

.blog-post img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.blog-content {
    padding: 1.5rem;
}

.blog-content h4 {
    font-family: var(--font-serif);
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
}

.blog-content p {
    font-size: 0.9rem;
    color: #666;
    margin-bottom: 1rem;
}

.blog-content a {
    color: var(--matcha-green);
    text-decoration: none;
    font-weight: 500;
}

.blog-content a:hover {
    text-decoration: underline;
}


/* ======== FOOTER ======== */
.main-footer {
    background-color: var(--charcoal-gray);
    color: var(--off-white);
    padding-top: 4rem;
}

.footer-container {
    display: flex;
    justify-content: space-between;
    gap: 2rem;
    padding-bottom: 4rem;
}

.footer-column {
    flex: 1;
}

.footer-column h4 {
    font-family: var(--font-serif);
    font-size: 1.3rem;
    margin-bottom: 1rem;
    color: var(--muted-gold);
}

.footer-column ul {
    list-style: none;
}

.footer-column ul li a {
    color: var(--off-white);
    text-decoration: none;
    opacity: 0.8;
    transition: opacity 0.3s;
}

.footer-column ul li a:hover {
    opacity: 1;
}

.social-icons a {
    color: var(--off-white);
    font-size: 1.2rem;
    margin-right: 1rem;
    opacity: 0.8;
    transition: opacity 0.3s, color 0.3s;
}

.social-icons a:hover {
    opacity: 1;
    color: var(--muted-gold);
}

.footer-bottom {
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    text-align: center;
    padding: 1.5rem 0;
    font-size: 0.9rem;
    opacity: 0.7;
}

/* ======== RESPONSIVE DESIGN ======== */
@media(max-width: 768px) {
    html {
        font-size: 15px;
    }

    .main-nav { display: none; } /* Simplified for demo, needs hamburger */

    .hero-title { font-size: 3rem; }
    .hero-subtitle { font-size: 1rem; }

    .product-grid, .blog-grid {
        grid-template-columns: 1fr;
    }

    .process-container {
        flex-direction: column;
    }

    .footer-container {
        flex-direction: column;
        text-align: center;
    }

    .social-icons {
        margin-bottom: 1rem;
    }
}
