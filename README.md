
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NattyBlog</title>
<style>
    * {
        margin: 0; padding: 0; box-sizing: border-box;
        font-family: 'Arial', sans-serif;
    }
    body {
        background: #f9f9f9; color: #333; line-height: 1.6; scroll-behavior: smooth;
    }
    a { text-decoration: none; color: inherit; }
    header {
        background: linear-gradient(135deg, #ff6a00, #ffcc00);
        color: #fff; text-align: center; padding: 40px 20px;
    }
    header h1 { font-size: 3rem; animation: fadeInDown 1s ease-in-out; }
    header p { animation: fadeInUp 1s ease-in-out; }
    nav {
        background: #fff; display: flex; justify-content: center; gap: 30px;
        padding: 15px; box-shadow: 0 3px 6px rgba(0,0,0,0.1); position: sticky; top: 0; z-index: 1000;
    }
    nav a {
        font-weight: bold; color: #ff6a00; transition: 0.3s;
    }
    nav a:hover { color: #333; }
    .container { width: 90%; max-width: 1200px; margin: 30px auto; }
    section { margin-bottom: 60px; }
    h2 { margin-bottom: 20px; color: #ff6a00; }
    .featured-posts {
        display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px;
    }
    .card {
        background: #fff; border-radius: 15px; overflow: hidden;
        box-shadow: 0 4px 10px rgba(0,0,0,0.1); transition: transform 0.3s;
    }
    .card:hover { transform: scale(1.03); }
    .card img { width: 100%; height: 200px; object-fit: cover; }
    .card-content { padding: 15px; }
    .card-content h3 { color: #ff6a00; margin-bottom: 10px; }
    .card-content p { font-size: 0.95rem; color: #555; }
    /* About Section */
    #about p { max-width: 700px; margin: auto; text-align: center; font-size: 1.1rem; }
    /* Contact Form */
    #contact form { max-width: 500px; margin: auto; display: flex; flex-direction: column; gap: 15px; }
    input, textarea {
        padding: 12px; border-radius: 8px; border: 1px solid #ccc; font-size: 1rem;
    }
    button {
        padding: 12px; border: none; background: #ff6a00; color: #fff; font-size: 1rem;
        border-radius: 8px; cursor: pointer; transition: background 0.3s;
    }
    button:hover { background: #e65c00; }
    /* Footer */
    footer {
        text-align: center; padding: 15px; background: #ff6a00; color: #fff;
    }
    .social-icons a {
        margin: 0 10px; color: #fff; font-size: 1.5rem; transition: 0.3s;
    }
    .social-icons a:hover { color: #333; }
    /* Animations */
    @keyframes fadeInDown { from { opacity: 0; transform: translateY(-20px);} to { opacity:1; transform: translateY(0);} }
    @keyframes fadeInUp { from { opacity: 0; transform: translateY(20px);} to { opacity:1; transform: translateY(0);} }
    @media(max-width:768px) { header h1 { font-size: 2rem; } }
</style>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

<!-- HEADER -->
<header>
    <h1>NattyBlog</h1>
    <p>Your space for ideas & inspiration</p>
</header>

<!-- NAV -->
<nav>
    <a href="#home">Home</a>
    <a href="#blog">Blog</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</nav>

<!-- HOME -->
<section id="home" class="container">
    <h2>Featured Posts</h2>
    <div class="featured-posts">
        <div class="card">
            <img src="https://source.unsplash.com/400x200/?nature,travel" alt="Post">
            <div class="card-content">
                <h3>Exploring Nature's Beauty</h3>
                <p>Discover breathtaking places that will leave you in awe...</p>
            </div>
        </div>
        <div class="card">
            <img src="https://source.unsplash.com/400x200/?technology" alt="Post">
            <div class="card-content">
                <h3>Top 5 Tech Trends of 2025</h3>
                <p>Stay ahead with the latest innovations shaping the future...</p>
            </div>
        </div>
        <div class="card">
            <img src="https://source.unsplash.com/400x200/?food" alt="Post">
            <div class="card-content">
                <h3>Delicious Recipes You Must Try</h3>
                <p>A collection of easy and tasty recipes to spice up your meals...</p>
            </div>
        </div>
    </div>
</section>

<!-- BLOG -->
<section id="blog" class="container">
    <h2>Blog Posts</h2>
    <p>Coming soon! More amazing content on travel, tech, and lifestyle.</p>
</section>

<!-- ABOUT -->
<section id="about" class="container">
    <h2>About Me</h2>
    <p>Hello! I'm Natty, a passionate writer and creator. NattyBlog is where I share my thoughts on travel, technology, food, and everything that inspires me. Join me on this journey of discovery and creativity!</p>
</section>

<!-- CONTACT -->
<section id="contact" class="container">
    <h2>Contact Me</h2>
    <form action="https://formspree.io/f/xayzgjbl" method="POST">
        <input type="text" name="name" placeholder="Your Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
    </form>
</section>

<!-- FOOTER -->
<footer>
    <div class="social-icons">
        <a href="#"><i class="fab fa-facebook"></i></a>
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
    </div>
    <p>© 2025 NattyBlog. All rights reserved.</p>
</footer>

</body>
</html>
