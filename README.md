<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI/ML Expert - Professional Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #10b981;
            --dark: #1f2937;
            --light: #f9fafb;
            --gray: #6b7280;
            --accent: #8b5cf6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            gap: 30px;
        }
        
        .nav-links a {
            color: var(--dark);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        /* Hero Section */
        .hero {
            padding: 150px 0 100px;
            background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 100%);
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .hero p {
            font-size: 1.2rem;
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .hero-buttons {
            display: flex;
            gap: 15px;
            justify-content: center;
        }
        
        .btn {
            padding: 12px 28px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
        }
        
        .btn-primary {
            background-color: var(--primary);
            color: white;
        }
        
        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }
        
        .btn-outline {
            border: 2px solid var(--primary);
            color: var(--primary);
        }
        
        .btn-outline:hover {
            background-color: var(--primary);
            color: white;
            transform: translateY(-2px);
        }
        
        /* About Section */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        .section-title p {
            color: var(--gray);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .about-content {
            display: flex;
            gap: 50px;
            align-items: center;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--dark);
        }
        
        .about-text p {
            margin-bottom: 20px;
            color: var(--gray);
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 30px;
        }
        
        .skill {
            background-color: var(--primary);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }
        
        .about-image {
            flex: 1;
            text-align: center;
        }
        
        .profile-img {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid var(--primary);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Projects Section */
        .projects {
            background-color: #f8fafc;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }
        
        .project-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .project-img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .project-content {
            padding: 25px;
        }
        
        .project-content h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        .project-content p {
            color: var(--gray);
            margin-bottom: 20px;
        }
        
        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 20px;
        }
        
        .project-tag {
            background-color: #eef2ff;
            color: var(--primary);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }
        
        .project-link {
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
            display: inline-flex;
            align-items: center;
            gap: 5px;
        }
        
        .project-link:hover {
            text-decoration: underline;
        }
        
        /* Contact Section */
        .contact {
            text-align: center;
        }
        
        .contact-content {
            max-width: 600px;
            margin: 0 auto;
        }
        
        .contact-content p {
            color: var(--gray);
            margin-bottom: 30px;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
        }
        
        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background-color: var(--primary);
            color: white;
            border-radius: 50%;
            font-size: 1.2rem;
            transition: all 0.3s;
        }
        
        .social-link:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
        }
        
        .contact-form {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }
        
        .form-group {
            text-align: left;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--dark);
        }
        
        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        
        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--primary);
        }
        
        .form-group textarea {
            min-height: 150px;
            resize: vertical;
        }
        
        .submit-btn {
            background-color: var(--primary);
            color: white;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            padding: 14px 0;
            border-radius: 6px;
            font-weight: 600;
            transition: background-color 0.3s;
        }
        
        .submit-btn:hover {
            background-color: var(--primary-dark);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 50px 0 20px;
            text-align: center;
        }
        
        .footer-content {
            margin-bottom: 30px;
        }
        
        .footer-content h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        .footer-content p {
            color: #d1d5db;
            max-width: 500px;
            margin: 0 auto;
        }
        
        .copyright {
            padding-top: 20px;
            border-top: 1px solid #374151;
            color: #9ca3af;
            font-size: 0.9rem;
        }
        
        /* Responsive Design */
        @media (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .about-image {
                order: -1;
            }
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 576px) {
            .nav-links {
                display: none;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">AIExpert</a>
                <div class="nav-links">
                    <a href="#about">About</a>
                    <a href="#projects">Projects</a>
                    <a href="#contact">Contact</a>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>AI & Machine Learning Specialist</h1>
            <p>I transform complex data into intelligent solutions. With expertise in Python, TensorFlow, and NLP, I build AI systems that drive real impact for businesses.</p>
            <div class="hero-buttons">
                <a href="#projects" class="btn btn-primary">View My Work</a>
                <a href="#contact" class="btn btn-outline">Get In Touch</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <div class="container">
            <div class="section-title">
                <h2>About Me</h2>
                <p>Learn about my expertise and skills in the AI/ML field</p>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Transforming Ideas into Intelligent Solutions</h3>
                    <p>I am an AI/ML expert with hands-on experience in building smart, scalable solutions. I specialize in developing machine learning models, natural language processing systems, and computer vision applications that solve real-world problems.</p>
                    <p>My approach combines technical expertise with a deep understanding of business needs, ensuring that the AI solutions I deliver are not only technologically advanced but also aligned with strategic goals.</p>
                    
                    <div class="skills">
                        <span class="skill">Python</span>
                        <span class="skill">TensorFlow</span>
                        <span class="skill">PyTorch</span>
                        <span class="skill">NLP</span>
                        <span class="skill">Computer Vision</span>
                        <span class="skill">Deep Learning</span>
                        <span class="skill">Data Analysis</span>
                        <span class="skill">Machine Learning</span>
                    </div>
                </div>
                <div class="about-image">
                    <img src="https://placeholder-image-service.onrender.com/image/300x300?prompt=A professional headshot of an AI engineer with a friendly expression&id=ff5c3e6a-7d70-4ae7-b68c-3c33b2de1e50" alt="Professional AI/ML expert headshot" class="profile-img">
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
        <div class="container">
            <div class="section-title">
                <h2>Featured Projects</h2>
                <p>Check out some of my recent AI/ML projects</p>
            </div>
            <div class="projects-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <img src="https://placeholder-image-service.onrender.com/image/400x200?prompt=AI chatbot interface with conversation bubbles and a friendly robot avatar&id=7b16b10c-a6c2-48fa-a6da-fa7dc9d73a8c" alt="AI chatbot interface design" class="project-img">
                    <div class="project-content">
                        <h3>Intelligent Customer Support Chatbot</h3>
                        <p>Developed a conversational AI chatbot using NLP techniques and Python libraries like NLTK and spaCy.</p>
                        <div class="project-tags">
                            <span class="project-tag">NLP</span>
                            <span class="project-tag">Python</span>
                            <span class="project-tag">Chatbot</span>
                        </div>
                        <a href="https://chat.openai.com/" class="project-link" target="_blank">
                            View Demo <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="project-card">
                    <img src="https://placeholder-image-service.onrender.com/image/400x200?prompt=Image classification interface showing different categories of objects with accuracy metrics&id=10d7c2b8-12c4-4b8e-a80a-9c9b2d5c5f70" alt="Image classification model interface" class="project-img">
                    <div class="project-content">
                        <h3>Advanced Image Classification Model</h3>
                        <p>Built a deep learning image classifier using TensorFlow and Keras to accurately identify and categorize images.</p>
                        <div class="project-tags">
                            <span class="project-tag">TensorFlow</span>
                            <span class="project-tag">Computer Vision</span>
                            <span class="project-tag">Deep Learning</span>
                        </div>
                        <a href="https://teachablemachine.withgoogle.com/" class="project-link" target="_blank">
                            View Demo <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="project-card">
                    <img src="https://placeholder-image-service.onrender.com/image/400x200?prompt=Sales forecasting dashboard with charts and prediction graphs&id=5a4b29d8-5d9c-421c-9f9b-2caf4e8bb5d9" alt="Sales forecasting dashboard" class="project-img">
                    <div class="project-content">
                        <h3>Sales Forecasting with LSTM</h3>
                        <p>Implemented a predictive model using LSTM networks to forecast sales trends based on historical data.</p>
                        <div class="project-tags">
                            <span class="project-tag">LSTM</span>
                            <span class="project-tag">Time Series</span>
                            <span class="project-tag">Predictive Analytics</span>
                        </div>
                        <a href="https://www.kaggle.com/code/ryanholbrook/forecasting-with-machine-learning" class="project-link" target="_blank">
                            View Demo <i class="fas fa-arrow-right"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <div class="container">
            <div class="section-title">
                <h2>Get In Touch</h2>
                <p>Ready to bring your AI ideas to life? Let's connect!</p>
            </div>
            <div class="contact-content">
                <p>I'm available for freelance projects and consulting engagements. Whether you need a custom AI solution or technical guidance, I'm here to help.</p>
                
                <div class="social-links">
                    <a href="#" class="social-link"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-github"></i></a>
                    <a href="#" class="social-link"><i class="fab fa-twitter"></i></a>
                    <a href="#" class="social-link"><i class="fas fa-envelope"></i></a>
                </div>
                
                <form class="contact-form">
                    <div class="form-group">
                        <label for="name">Your Name</label>
                        <input type="text" id="name" placeholder="Enter your name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Your Email</label>
                        <input type="email" id="email" placeholder="Enter your email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Your Message</label>
                        <textarea id="message" placeholder="Tell me about your project" required></textarea>
                    </div>
                    <button type="submit" class="submit-btn">Send Message</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <h3>AI & Machine Learning Expert</h3>
                <p>Transforming complex data into intelligent solutions that drive real business impact.</p>
            </div>
            <div class="copyright">
                <p>© 2023 AIExpert. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Form submission handler
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thanks for your message! I\'ll get back to you soon.');
            this.reset();
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
