<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Luxury Home Remodeling</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
<style>
/* Reset */
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{font-family:'Montserrat',sans-serif;color:#333;line-height:1.6;background:#fff;overflow-x:hidden;}
a{text-decoration:none;color:inherit;}
img{width:100%;display:block;border-radius:10px;transition: transform 0.5s;}
/* Colors */
:root{--accent:#1d3557;--gold:#cfa14b;--charcoal:#333;--light-gray:#f5f5f5;}

/* Sticky Nav */
nav{position:sticky;top:0;z-index:1000;background:rgba(255,255,255,0.95);display:flex;justify-content:space-between;align-items:center;padding:1rem 2rem;box-shadow:0 2px 10px rgba(0,0,0,0.1);}
nav .logo{font-weight:700;font-size:1.5rem;color:var(--accent);}
nav ul{list-style:none;display:flex;gap:1.5rem;align-items:center;}
nav ul li a{font-weight:600;transition:color 0.3s;}
nav ul li a:hover{color:var(--gold);}
nav .cta{padding:0.5rem 1rem;background:var(--gold);color:#fff;border-radius:5px;font-weight:600;transition:opacity 0.3s;}
nav .cta:hover{opacity:0.85;}

/* Hero with parallax */
.hero{height:100vh;background:url('https://source.unsplash.com/1600x900/?luxury-home,kitchen') center/cover no-repeat fixed;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;color:#fff;padding:0 1rem;position:relative;overflow:hidden;}
.hero h1{font-size:3rem;margin-bottom:1rem;opacity:0;transform:translateY(-50px);}
.hero p{font-size:1.25rem;margin-bottom:2rem;max-width:700px;opacity:0;transform:translateY(50px);}
.hero .buttons{display:flex;gap:1rem;flex-wrap:wrap;opacity:0;transform:translateY(50px);}
.hero .buttons a{padding:0.75rem 1.5rem;border-radius:5px;font-weight:600;transition:opacity 0.3s;}
.hero .buttons .primary{background:var(--gold);color:#fff;}
.hero .buttons .secondary{background:rgba(255,255,255,0.85);color:var(--charcoal);}
.hero .buttons a:hover{opacity:0.85;}

/* Sections */
section{padding:6rem 2rem;max-width:1200px;margin:auto;}
h2{text-align:center;font-size:2rem;margin-bottom:2rem;color:var(--accent);}

/* Services */
.services{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:2rem;}
.service-card{background:#fff;padding:2rem;border-radius:10px;box-shadow:0 10px 25px rgba(0,0,0,0.08);transition:transform 0.5s,box-shadow 0.5s; text-align:center;}
.service-card:hover{transform:translateY(-10px);box-shadow:0 15px 35px rgba(0,0,0,0.15);}
.service-card img{width:60px;margin-bottom:1rem;}

/* Gallery */
.gallery{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1rem;}
.gallery img{transition: transform 0.5s, box-shadow 0.5s;cursor:pointer;}
.gallery img:hover{transform:scale(1.05) rotate(0.5deg);box-shadow:0 15px 35px rgba(0,0,0,0.2);}

/* Features */
.features{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:2rem;text-align:center;}
.feature{background:var(--light-gray);padding:2rem;border-radius:10px;transition:transform 0.5s, box-shadow 0.5s;}
.feature:hover{transform:translateY(-10px);box-shadow:0 10px 25px rgba(0,0,0,0.15);}
.feature img{width:50px;margin-bottom:1rem;}

/* Testimonials */
.testimonials{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:2rem;}
.testimonial-card{background:#fff;padding:2rem;border-radius:10px;box-shadow:0 10px 25px rgba(0,0,0,0.1);}
.testimonial-card p{font-style:italic;margin-bottom:1rem;}
.stars{color:gold;margin-bottom:1rem;}

/* CTA Banner */
.cta-banner{background:linear-gradient(135deg,var(--accent),#3a5a80);color:#fff;padding:5rem 2rem;text-align:center;border-radius:15px;margin:3rem 0;box-shadow:0 15px 35px rgba(0,0,0,0.15);}
.cta-banner a{background:var(--gold);color:#fff;padding:1rem 2rem;border-radius:5px;font-weight:600;display:inline-block;margin-top:1rem;transition:transform 0.3s;}
.cta-banner a:hover{transform:scale(1.05);}

/* Contact */
.contact form{display:grid;gap:1rem;max-width:600px;margin:auto;}
.contact input,.contact textarea{padding:1rem;border:1px solid #ccc;border-radius:5px;width:100%;}
.contact button{padding:1rem;background:var(--accent);color:#fff;border:none;border-radius:5px;font-weight:600;cursor:pointer;transition:transform 0.3s;}
.contact button:hover{transform:scale(1.05);}

/* Footer */
footer{background:#222;color:#fff;padding:2rem;text-align:center;}
footer a{color:#fff;margin:0 0.5rem;transition:color 0.3s;}
footer a:hover{color:var(--gold);}

/* Responsive */
@media(max-width:768px){
.hero h1{font-size:2.5rem;}
.hero p{font-size:1rem;}
nav ul{flex-direction:column;gap:0.75rem;margin-top:0.5rem;}
}

/* Fade-in animation */
.fade-in{opacity:0;transform:translateY(30px);transition:opacity 1s ease, transform 1s ease;}
.fade-in.visible{opacity:1;transform:translateY(0);}
</style>
</head>
<body>

<!-- Navigation -->
<nav>
<div class="logo">LuxuryRemodel</div>
<ul>
<li><a href="#home">Home</a></li>
<li><a href="#services">Services</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#testimonials">Testimonials</a></li>
<li><a href="#contact">Contact</a></li>
<li><a href="#contact" class="cta">Get Free Estimate</a></li>
</ul>
</nav>

<!-- Hero -->
<section class="hero" id="home">
<h1>Luxury Home Remodeling & Renovations</h1>
<p>Transforming Kitchens, Bathrooms, and Entire Homes with Exceptional Craftsmanship.</p>
<div class="buttons">
<a href="#contact" class="primary">Get Free Estimate</a>
<a href="#projects" class="secondary">View Our Work</a>
</div>
</section>

<!-- Services -->
<section id="services">
<h2>Our Services</h2>
<div class="services">
<div class="service-card fade-in">
<img src="https://source.unsplash.com/60x60/?kitchen" alt="Kitchen Remodeling">
<h3>Kitchen Remodeling</h3>
<p>Modern, functional, and luxurious kitchen transformations tailored to your lifestyle.</p>
</div>
<div class="service-card fade-in">
<img src="https://source.unsplash.com/60x60/?bathroom" alt="Bathroom Remodeling">
<h3>Bathroom Remodeling</h3>
<p>Elegant bathrooms with premium fixtures and timeless designs.</p>
</div>
<div class="service-card fade-in">
<img src="https://source.unsplash.com/60x60/?home-renovation" alt="Full Home Renovations">
<h3>Full Home Renovations</h3>
<p>Complete home transformations with exceptional attention to detail.</p>
</div>
</div>
</section>

<!-- Projects -->
<section id="projects">
<h2>Featured Projects</h2>
<div class="gallery">
<img src="https://source.unsplash.com/400x300/?luxury-home1" class="fade-in" alt="">
<img src="https://source.unsplash.com/400x300/?luxury-home2" class="fade-in" alt="">
<img src="https://source.unsplash.com/400x300/?luxury-home3" class="fade-in" alt="">
<img src="https://source.unsplash.com/400x300/?luxury-home4" class="fade-in" alt="">
<img src="https://source.unsplash.com/400x300/?luxury-home5" class="fade-in" alt="">
<img src="https://source.unsplash.com/400x300/?luxury-home6" class="fade-in" alt="">
</div>
</section>

<!-- Why Choose Us -->
<section id="why">
<h2>Why Choose Us</h2>
<div class="features">
<div class="feature fade-in"><img src="https://source.unsplash.com/50x50/?badge" alt=""><p>Licensed & Insured</p></div>
<div class="feature fade-in"><img src="https://source.unsplash.com/50x50/?experience" alt=""><p>10+ Years Experience</p></div>
<div class="feature fade-in"><img src="https://source.unsplash.com/50x50/?pricing" alt=""><p>Transparent Pricing</p></div>
<div class="feature fade-in"><img src="https://source.unsplash.com/50x50/?materials" alt=""><p>Premium Materials</p></div>
<div class="feature fade-in"><img src="https://source.unsplash.com/50x50/?manager" alt=""><p>Dedicated Project Manager</p></div>
</div>
</section>

<!-- Testimonials -->
<section id="testimonials">
<h2>Testimonials</h2>
<div class="testimonials">
<div class="testimonial-card fade-in">
<div class="stars">★★★★★</div>
<p>"The team completely transformed our kitchen. Professional and precise work!"</p>
<strong>- Sarah W.</strong>
</div>
<div class="testimonial-card fade-in">
<div class="stars">★★★★★</div>
<p>"Our bathroom renovation exceeded all expectations. Highly recommended."</p>
<strong>- John D.</strong>
</div>
<div class="testimonial-card fade-in">
<div class="stars">★★★★★</div>
<p>"Full home renovation done seamlessly. Every detail is perfect."</p>
<strong>- Emily R.</strong>
</div>
</div>
</section>

<!-- CTA Banner -->
<section class="cta-banner fade-in">
<h2>Ready to Transform Your Home?</h2>
<a href="#contact">Request a Free Estimate</a>
</section>

<!-- Contact -->
<section id="contact">
<h2>Contact Us</h2>
<div class="contact">
<form>
<input type="text" placeholder="Name" required>
<input type="email" placeholder="Email" required>
<input type="tel" placeholder="Phone" required>
<textarea rows="5" placeholder="Project Details" required></textarea>
<button type="submit">Submit</button>
</form>
</div>
</section>

<!-- Footer -->
<footer>
<p>&copy; 2026 LuxuryRemodel. All Rights Reserved.</p>
<p>
<a href="#home">Home</a> | 
<a href="#services">Services</a> | 
<a href="#projects">Projects</a> | 
<a href="#contact">Contact</a>
</p>
</footer>

<script>
// Fade-in on scroll
const faders = document.querySelectorAll('.fade-in');
const appearOptions = { threshold:0.1, rootMargin:"0px 0px -50px 0px" };
const appearOnScroll = new IntersectionObserver((entries,observer)=>{
entries.forEach(entry=>{
if(entry.isIntersecting){entry.target.classList.add('visible');observer.unobserve(entry.target);}
});
},appearOptions);
faders.forEach(fader=>{appearOnScroll.observe(fader);});

// Hero text animation
window.addEventListener('load',()=>{ 
document.querySelector('.hero h1').classList.add('visible');
document.querySelector('.hero p').classList.add('visible');
document.querySelector('.hero .buttons').classList.add('visible');
});
</script>
</body>
</html>