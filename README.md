<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <title>NSHUTI Emmanuel - Home</title>
    <link rel="icon" href="target.gif">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="style.css">
    <style>
        .hero {
            padding-top: 120px;
            background: linear-gradient(135deg, var(--light-color) 0%, var(--background-color) 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
        }
        
        .hero-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 50px;
            align-items: center;
        }
        
        @media (min-width: 992px) {
            .hero-content {
                grid-template-columns: 1fr 1fr;
            }
        }
        
        .hero-text h1 {
            margin-bottom: 10px;
        }
        
        .hero-text h3 {
            color: var(--primary-color);
            font-weight: 500;
            margin-bottom: 20px;
            min-height: 60px;
            display: flex;
            align-items: center;
        }
        
        .typing-container {
            display: inline;
        }
        
        .typing-text {
            color: var(--secondary-color);
            font-weight: 600;
            border-right: 3px solid var(--primary-color);
            padding-right: 5px;
            animation: blink 0.7s infinite;
        }
        
        @keyframes blink {
            0%, 100% { border-color: var(--primary-color); }
            50% { border-color: transparent; }
        }
        
        .hero-btns {
            display: flex;
            gap: 15px;
            margin-top: 30px;
        }
        
        .hero-image {
            text-align: center;
        }
        
        .profile-image-container {
            width: 100%;
            max-width: 400px;
            margin: 0 auto;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: var(--shadow);
        }
        
        .profile-image {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .image-fallback {
            height: 400px;
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 5rem;
        }
        
        .quick-links {
            padding: 80px 0;
            background-color: var(--card-bg);
        }
        
        .links-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .link-card {
            background-color: var(--light-color);
            padding: 40px 30px;
            border-radius: 15px;
            text-align: center;
            transition: var(--transition);
            box-shadow: var(--shadow);
        }
        
        .link-card:hover {
            transform: translateY(-10px);
            background-color: var(--primary-color);
        }
        
        .link-card:hover * {
            color: white;
        }
        
        .link-icon {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 20px;
            transition: var(--transition);
        }
        
        .link-card h3 {
            margin-bottom: 15px;
        }
        
        .link-card p {
            margin-bottom: 0;
        }
    </style>
</head>
<body>
    <div class="theme-toggle" id="themeToggle">
        <i class="fas fa-moon"></i>
        <i class="fas fa-sun"></i>
    </div>

    <header>
        <div class="navbar">
            <a href="index.html" class="logo">NSHUTI<span>.</span></a>
            
            <div class="nav-center">
                <ul class="nav-links" id="navLinks">
                    <li><a href="index.html" class="active">Home</a></li>
                    <li><a href="about.html">About</a></li>
                    <li><a href="education.html">Education</a></li>
                    <li><a href="projects.html">Projects</a></li>
                    <li><a href="contact.html">Contact</a></li>
                </ul>
            </div>
            
            <div class="nav-right">
            </div>
            
            <div class="hamburger" id="hamburger">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <div class="hero-text">
                    <h1>NSHUTI Emmanuel</h1>
                    <h3>IT Student & Aspiring <span class="typing-container"><span id="typing-text"></span></span></h3>
                    <p>I am a passionate IT student at King David Academy with expertise in programming languages like C++ and C, web development with HTML, CSS, JavaScript, and cybersecurity. Based in Rubavu, Rwanda, I'm dedicated to becoming a skilled software developer and ethical hacker.</p>
                    <p>My journey in technology started with curiosity about how software works, and now I'm pursuing it seriously to solve real-world problems through secure and efficient software solutions.</p>
                    <div class="hero-btns">
                        <a href="projects.html" class="btn">View My Work</a>
                        <a href="contact.html" class="btn btn-secondary">Contact Me</a>
                    </div>
                </div>
                <div class="hero-image">
                    <div class="profile-image-container">
                        <img src="Nshuti8.png.jpg" alt="NSHUTI Emmanuel" class="profile-image" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
                        <div class="image-fallback" style="display: none;">
                            <i class="fas fa-user"></i>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="quick-links">
        <div class="container">
            <h2>Explore My Portfolio</h2>
            <div class="links-grid">
                <a href="about.html" class="link-card">
                    <div class="link-icon">
                        <i class="fas fa-user"></i>
                    </div>
                    <h3>About Me</h3>
                    <p>Learn about my skills, background, and what drives me in technology</p>
                </a>
                
                <a href="education.html" class="link-card">
                    <div class="link-icon">
                        <i class="fas fa-graduation-cap"></i>
                    </div>
                    <h3>Education</h3>
                    <p>See my academic journey and career goals at King David Academy</p>
                </a>
                
                <a href="projects.html" class="link-card">
                    <div class="link-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <h3>Projects</h3>
                    <p>View my programming projects and web development work</p>
                </a>
                
                <a href="contact.html" class="link-card">
                    <div class="link-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3>Contact</h3>
                    <p>Get in touch with me for opportunities or collaboration</p>
                </a>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <div class="footer-logo">NSHUTI<span>.</span></div>
                    <p class="footer-text">IT Student at King David Academy passionate about software development and cybersecurity</p>
                </div>
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="index.html" class="footer-link">Home</a></li>
                        <li><a href="about.html" class="footer-link">About</a></li>
                        <li><a href="education.html" class="footer-link">Education</a></li>
                        <li><a href="projects.html" class="footer-link">Projects</a></li>
                        <li><a href="contact.html" class="footer-link">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-social">
                    <h3>Connect</h3>
                    <div class="social-icons">
                        <a href="https://github.com/nshutiemmanuel860-coder/" target="_blank" class="social-icon"><i class="fab fa-github"></i></a>
                        <a href="https://www.linkedin.com/feed/" target="_blank" class="social-icon"><i class="fab fa-linkedin"></i></a>
                        <a href="https://www.instagram.com/nshuti__wagakira/" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
                        <a href="mailto:nshutiemmanuel860@gmail.com" class="social-icon"><i class="fas fa-envelope"></i></a>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; <span id="currentYear"></span> NSHUTI Emmanuel. All Rights Reserved.</p>
                <p class="footer-contact">Phone: +250 783805137 | Location: Rubavu, Rwanda</p>
            </div>
        </div>
    </footer>

    <div class="back-to-top" id="backToTop">
        <i class="fas fa-arrow-up"></i>
    </div>

    <script src="script.js"></script>
</body>
</html>
