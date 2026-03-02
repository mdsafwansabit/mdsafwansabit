<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Safwan Sabit - Full Stack Engineer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .hero {
            text-align: center;
            padding: 60px 20px;
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            animation: fadeInUp 1s ease-out;
        }
        
        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #f9ca24);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
            animation: rainbow 3s linear infinite;
        }
        
        .hero-subtitle {
            font-size: clamp(1.2rem, 3vw, 1.8rem);
            color: #fff;
            margin-bottom: 20px;
            font-weight: 300;
        }
        
        .profile-views {
            background: rgba(255,255,255,0.2);
            padding: 15px 30px;
            border-radius: 50px;
            display: inline-block;
            margin: 20px 0;
            backdrop-filter: blur(10px);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 30px 0;
        }
        
        .social-btn {
            display: flex;
            align-items: center;
            gap: 10px;
            padding: 12px 24px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        
        .social-btn:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }
        
        .section {
            background: rgba(255,255,255,0.95);
            backdrop-filter: blur(20px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
            animation: fadeInUp 1s ease-out;
            animation-fill-mode: both;
        }
        
        .section h2 {
            font-size: 2.2rem;
            margin-bottom: 25px;
            background: linear-gradient(45deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-align: center;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .stat-card {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-10px);
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .tech-item {
            text-align: center;
            padding: 20px;
            background: linear-gradient(135deg, #f093fb, #f5576c);
            border-radius: 15px;
            transition: all 0.3s ease;
            color: white;
        }
        
        .tech-item:hover {
            transform: translateY(-10px) rotate(5deg);
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }
        
        .tech-item img {
            width: 50px;
            height: 50px;
            margin-bottom: 10px;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .section:nth-child(odd) { animation-delay: 0.2s; }
        .section:nth-child(even) { animation-delay: 0.4s; }
        
        @keyframes rainbow {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .hero h1 {
            background-size: 300% 300%;
            animation: rainbow 3s ease infinite;
        }
        
        @media (max-width: 768px) {
            .container { padding: 10px; }
            .hero { padding: 40px 20px; }
            .section { padding: 25px; }
            .social-links { flex-direction: column; align-items: center; }
        }
        
        .gradient-text {
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <h1>🚀 Safwan Sabit</h1>
            <p class="hero-subtitle gradient-text">Full Stack Engineer | React | Node.js | Laravel | Bangladesh 🇧🇩</p>
            <div class="profile-views">
                <img src="https://komarev.com/ghpvc/?username=mdsafwansabit&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" />
            </div>
            
            <!-- Social Links -->
            <div class="social-links">
                <a href="https://linkedin.com/in/safwan-sabit" class="social-btn" target="_blank">
                    💼 LinkedIn
                </a>
                <a href="https://facebook.com/safwansabit99" class="social-btn" target="_blank">
                    📘 Facebook
                </a>
                <a href="https://instagram.com/safwansabit10" class="social-btn" target="_blank">
                    📷 Instagram
                </a>
                <a href="https://youtube.com/@safwan_sabit" class="social-btn" target="_blank">
                    🎥 YouTube
                </a>
            </div>
        </section>

        <!-- Stats Section -->
        <section class="section">
            <h2>📊 GitHub Analytics</h2>
            <div class="stats-grid">
                <div class="stat-card">
                    <h3>⭐ Stars</h3>
                    <p>50+</p>
                </div>
                <div class="stat-card">
                    <h3>🍴 Forks</h3>
                    <p>25+</p>
                </div>
                <div class="stat-card">
                    <h3>👥 Followers</h3>
                    <p>100+</p>
                </div>
                <div class="stat-card">
                    <h3>📁 Repos</h3>
                    <p>30+</p>
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section class="section">
            <h2>🛠️ Tech Stack Mastery</h2>
            <p style="text-align: center; color: #666; margin-bottom: 30px; font-size: 1.1rem;">
                Mastered 75+ technologies across the full stack
            </p>
            <div class="tech-grid">
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React">
                    <div>React</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg" alt="Node.js">
                    <div>Node.js</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original.svg" alt="Vue.js">
                    <div>Vue.js</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain.svg" alt="Laravel">
                    <div>Laravel</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" alt="MongoDB">
                    <div>MongoDB</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg" alt="MySQL">
                    <div>MySQL</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original.svg" alt="AWS">
                    <div>AWS</div>
                </div>
                <div class="tech-item">
                    <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/tailwindcss/tailwindcss-original.svg" alt="Tailwind">
                    <div>Tailwind</div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer style="text-align: center; padding: 30px; color: white; background: rgba(0,0,0,0.3); border-radius: 20px; margin-top: 40px;">
            <p>💫 Built with ❤️ for the developer community</p>
            <p><strong>Safwan Sabit</strong> | Full Stack Engineer | Bangladesh 🇧🇩</p>
        </footer>
    </div>

    <script>
        // Smooth scroll animations
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                const rect = section.getBoundingClientRect();
                if (rect.top < window.innerHeight && rect.bottom > 0) {
                    section.style.opacity = '1';
                    section.style.transform = 'translateY(0)';
                }
            });
        });
    </script>
</body>
</html>
