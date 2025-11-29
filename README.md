<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile README Preview</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600;700&family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            padding: 20px;
            line-height: 1.7;
            letter-spacing: -0.01em;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: #161b22;
            border-radius: 6px;
            padding: 30px;
            border: 1px solid #30363d;
        }
        
        .header {
            text-align: center;
            margin-bottom: 30px;
        }
        
        .header img {
            width: 100%;
            border-radius: 6px;
            margin-bottom: 20px;
        }
        
        .typing-effect {
            font-family: 'Poppins', sans-serif;
            font-size: 32px;
            font-weight: 700;
            color: #6366f1;
            margin: 20px 0;
            min-height: 40px;
            letter-spacing: -0.02em;
        }
        
        .social-badges {
            display: flex;
            gap: 10px;
            justify-content: center;
            flex-wrap: wrap;
            margin: 20px 0;
        }
        
        .badge {
            display: inline-block;
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-family: 'Inter', sans-serif;
            font-weight: 600;
            font-size: 14px;
            transition: transform 0.2s, box-shadow 0.2s;
            letter-spacing: 0.02em;
        }
        
        .badge:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(99, 102, 241, 0.3);
        }
        
        .badge-linkedin { background: #0077B5; color: white; }
        .badge-portfolio { background: #FF5722; color: white; }
        .badge-twitter { background: #1DA1F2; color: white; }
        .badge-email { background: #D14836; color: white; }
        
        .profile-views {
            display: inline-block;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 10px 20px;
            border-radius: 8px;
            font-family: 'Inter', sans-serif;
            font-weight: 700;
            margin: 20px 0;
            letter-spacing: 0.05em;
            box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
        }
        
        hr {
            border: none;
            border-top: 1px solid #30363d;
            margin: 30px 0;
        }
        
        h2 {
            color: #58a6ff;
            margin: 30px 0 20px 0;
            font-family: 'Poppins', sans-serif;
            font-size: 28px;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 10px;
            letter-spacing: -0.02em;
        }
        
        .code-block {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 24px;
            margin: 20px 0;
            font-family: 'JetBrains Mono', 'Courier New', monospace;
            overflow-x: auto;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
        }
        
        .code-block pre {
            color: #79c0ff;
            font-size: 15px;
            line-height: 1.8;
            font-weight: 500;
        }
        
        .about-points {
            margin: 20px 0;
        }
        
        .about-points p {
            margin: 10px 0;
            padding-left: 25px;
            position: relative;
            font-size: 16px;
            font-weight: 400;
        }
        
        .about-points p::before {
            content: '•';
            position: absolute;
            left: 0;
            color: #6366f1;
            font-size: 20px;
        }
        
        .tech-section {
            margin: 30px 0;
        }
        
        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            margin: 20px 0;
        }
        
        .tech-badge {
            padding: 10px 18px;
            border-radius: 8px;
            font-family: 'Inter', sans-serif;
            font-weight: 600;
            font-size: 14px;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            transition: transform 0.2s, box-shadow 0.2s;
            letter-spacing: 0.01em;
        }
        
        .tech-badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .stat-card {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            text-align: center;
        }
        
        .stat-card img {
            width: 100%;
            height: auto;
            border-radius: 6px;
        }
        
        .trophies {
            text-align: center;
            margin: 30px 0;
        }
        
        .project-card {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 28px;
            margin: 20px 0;
            transition: transform 0.3s, border-color 0.3s, box-shadow 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-8px);
            border-color: #58a6ff;
            box-shadow: 0 12px 40px rgba(88, 166, 255, 0.2);
        }
        
        .project-card h3 {
            color: #58a6ff;
            margin-bottom: 10px;
            font-family: 'Poppins', sans-serif;
            font-size: 22px;
            font-weight: 700;
            letter-spacing: -0.01em;
        }
        
        .project-card h4 {
            color: #8b949e;
            font-family: 'Inter', sans-serif;
            font-size: 16px;
            margin-bottom: 15px;
            font-weight: 600;
            letter-spacing: -0.01em;
        }
        
        .project-card p {
            margin: 15px 0;
            color: #c9d1d9;
            font-size: 15px;
            line-height: 1.7;
        }
        
        .project-tech {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin: 15px 0;
            font-family: 'JetBrains Mono', monospace;
            font-size: 13px;
            font-weight: 500;
        }
        
        .project-tech span {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 6px 14px;
            border-radius: 20px;
            letter-spacing: 0.02em;
        }
        
        .project-links {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }
        
        .project-links a {
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-family: 'Inter', sans-serif;
            font-weight: 600;
            font-size: 14px;
            transition: opacity 0.2s, transform 0.2s;
            letter-spacing: 0.02em;
        }
        
        .project-links a:hover {
            opacity: 0.9;
            transform: translateY(-2px);
        }
        
        .btn-demo { background: #00C7B7; color: white; }
        .btn-github { background: #238636; color: white; }
        
        .quote-box {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 12px;
            padding: 30px;
            margin: 20px 0;
            text-align: center;
            font-family: 'Poppins', sans-serif;
            font-style: italic;
            color: #8b949e;
            font-size: 18px;
            font-weight: 400;
            line-height: 1.8;
        }
        
        .footer {
            text-align: center;
            margin-top: 40px;
            padding: 30px 0;
            border-top: 1px solid #30363d;
        }
        
        .footer h3 {
            color: #c9d1d9;
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 24px;
            margin-bottom: 20px;
            letter-spacing: -0.01em;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate-in {
            animation: fadeIn 0.6s ease-out;
        }
    </style>
</head>
<body>
    <div class="container animate-in">
        <!-- Header Section -->
        <div class="header">
            <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Hi%20There!%20👋%20I'm%20[YOUR_NAME]&fontSize=42&fontAlignY=32&desc=Welcome%20to%20my%20digital%20playground&descAlignY=51&descAlign=50&animation=twinkling" alt="Header">
            
            <div class="typing-effect" id="typing"></div>
            
            <div class="social-badges">
                <a href="#" class="badge badge-linkedin">🔗 LinkedIn</a>
                <a href="#" class="badge badge-portfolio">🌐 Portfolio</a>
                <a href="#" class="badge badge-twitter">🐦 Twitter</a>
                <a href="#" class="badge badge-email">📧 Email</a>
            </div>
            
            <div class="profile-views">👁️ PROFILE VIEWS: 1,234</div>
        </div>
        
        <hr>
        
        <!-- About Me Section -->
        <h2>🙋‍♂️ About Me</h2>
        <div class="code-block">
            <pre>const developer = {
    name: "Your Name",
    role: "Full Stack Developer",
    location: "Surakarta, Indonesia 🇮🇩",
    code: ["JavaScript", "TypeScript", "Python", "Java"],
    currentFocus: "Building scalable web applications",
    challenge: "Mastering System Design & Cloud Architecture",
    funFact: "I debug with console.log() and I'm not ashamed 😄"
};</pre>
        </div>
        
        <div class="about-points">
            <p><strong>💡 I'm passionate about</strong> creating elegant solutions to complex problems and contributing to open-source projects that make a difference.</p>
            <p><strong>🌱 Currently Learning:</strong> Next.js 14, AWS, Docker & Kubernetes</p>
            <p><strong>🔭 Working On:</strong> [Your Current Project] - A revolutionary app that changes everything</p>
            <p><strong>⚡ Fun Fact:</strong> Coffee = Code. More Coffee = Better Code ☕</p>
        </div>
        
        <hr>
        
        <!-- Tech Stack Section -->
        <h2>🛠️ Tech Stack & Tools</h2>
        
        <div class="tech-section">
            <h3 style="color: #8b949e; text-align: center; margin: 20px 0; font-family: 'Poppins', sans-serif; font-weight: 600; font-size: 18px;">💻 Programming Languages</h3>
            <div class="tech-badges">
                <span class="tech-badge" style="background: #F7DF1E; color: black;">JavaScript</span>
                <span class="tech-badge" style="background: #007ACC; color: white;">TypeScript</span>
                <span class="tech-badge" style="background: #3776AB; color: white;">Python</span>
                <span class="tech-badge" style="background: #ED8B00; color: white;">Java</span>
                <span class="tech-badge" style="background: #E34F26; color: white;">HTML5</span>
                <span class="tech-badge" style="background: #1572B6; color: white;">CSS3</span>
            </div>
        </div>
        
        <div class="tech-section">
            <h3 style="color: #8b949e; text-align: center; margin: 20px 0; font-family: 'Poppins', sans-serif; font-weight: 600; font-size: 18px;">🚀 Frameworks & Libraries</h3>
            <div class="tech-badges">
                <span class="tech-badge" style="background: #61DAFB; color: black;">⚛️ React</span>
                <span class="tech-badge" style="background: #000000; color: white;">▲ Next.js</span>
                <span class="tech-badge" style="background: #43853D; color: white;">Node.js</span>
                <span class="tech-badge" style="background: #38B2AC; color: white;">Tailwind CSS</span>
                <span class="tech-badge" style="background: #563D7C; color: white;">Bootstrap</span>
            </div>
        </div>
        
        <div class="tech-section">
            <h3 style="color: #8b949e; text-align: center; margin: 20px 0; font-family: 'Poppins', sans-serif; font-weight: 600; font-size: 18px;">🗄️ Databases & Cloud</h3>
            <div class="tech-badges">
                <span class="tech-badge" style="background: #4EA94B; color: white;">🍃 MongoDB</span>
                <span class="tech-badge" style="background: #316192; color: white;">PostgreSQL</span>
                <span class="tech-badge" style="background: #00000F; color: white;">MySQL</span>
                <span class="tech-badge" style="background: #FFCA28; color: black;">🔥 Firebase</span>
                <span class="tech-badge" style="background: #232F3E; color: white;">☁️ AWS</span>
            </div>
        </div>
        
        <div class="tech-section">
            <h3 style="color: #8b949e; text-align: center; margin: 20px 0; font-family: 'Poppins', sans-serif; font-weight: 600; font-size: 18px;">🔧 Tools & Platforms</h3>
            <div class="tech-badges">
                <span class="tech-badge" style="background: #F05032; color: white;">Git</span>
                <span class="tech-badge" style="background: #2496ED; color: white;">🐳 Docker</span>
                <span class="tech-badge" style="background: #007ACC; color: white;">VS Code</span>
                <span class="tech-badge" style="background: #FF6C37; color: white;">Postman</span>
                <span class="tech-badge" style="background: #F24E1E; color: white;">Figma</span>
            </div>
        </div>
        
        <hr>
        
        <!-- GitHub Stats Section -->
        <h2>📊 GitHub Stats</h2>
        <div class="stats-grid">
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats">
            </div>
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages">
            </div>
        </div>
        
        <div style="text-align: center; margin: 20px 0;">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=anuraghazra&theme=tokyonight&hide_border=true" alt="GitHub Streak" style="max-width: 100%; border-radius: 6px;">
        </div>
        
        <hr>
        
        <!-- Trophies Section -->
        <h2>🏆 GitHub Trophies</h2>
        <div class="trophies">
            <img src="https://github-profile-trophy.vercel.app/?username=anuraghazra&theme=tokyonight&no-frame=true&no-bg=true&row=1&column=7" alt="Trophies" style="max-width: 100%;">
        </div>
        
        <hr>
        
        <!-- Featured Projects Section -->
        <h2>🚀 Featured Projects</h2>
        
        <div class="project-card">
            <h3>💼 Project Name 1</h3>
            <h4>E-Commerce Platform with Advanced Features</h4>
            <p>A full-stack e-commerce solution with real-time inventory management, payment gateway integration, and AI-powered product recommendations.</p>
            <div class="project-tech">
                <span>React</span>
                <span>Node.js</span>
                <span>MongoDB</span>
                <span>Stripe API</span>
                <span>AWS S3</span>
            </div>
            <div class="project-links">
                <a href="#" class="btn-demo">🚀 Live Demo</a>
                <a href="#" class="btn-github">📁 GitHub</a>
            </div>
        </div>
        
        <div class="project-card">
            <h3>🎨 Project Name 2</h3>
            <h4>Real-Time Collaborative Design Tool</h4>
            <p>A web-based design tool allowing multiple users to collaborate in real-time, inspired by Figma with a focus on simplicity.</p>
            <div class="project-tech">
                <span>Next.js</span>
                <span>Socket.io</span>
                <span>Canvas API</span>
                <span>TypeScript</span>
                <span>Redis</span>
            </div>
            <div class="project-links">
                <a href="#" class="btn-demo">🚀 Live Demo</a>
                <a href="#" class="btn-github">📁 GitHub</a>
            </div>
        </div>
        
        <div class="project-card">
            <h3>📱 Project Name 3</h3>
            <h4>Task Management App with AI Assistant</h4>
            <p>Smart task manager that uses AI to prioritize tasks, set deadlines, and provide productivity insights based on your work patterns.</p>
            <div class="project-tech">
                <span>React Native</span>
                <span>Python</span>
                <span>FastAPI</span>
                <span>TensorFlow</span>
                <span>PostgreSQL</span>
            </div>
            <div class="project-links">
                <a href="#" class="btn-demo">🚀 Live Demo</a>
                <a href="#" class="btn-github">📁 GitHub</a>
            </div>
        </div>
        
        <hr>
        
        <!-- Quote Section -->
        <h2>💭 Quote of the Day</h2>
        <div class="quote-box">
            <p>"The only way to do great work is to love what you do." - Steve Jobs</p>
        </div>
        
        <hr>
        
        <!-- Footer -->
        <div class="footer">
            <h3>🤝 Let's Connect!</h3>
            <p style="margin: 15px 0;">I'm always open to interesting conversations and collaboration opportunities!</p>
            <p><strong>💬 Ask me about:</strong> Web Development, System Design, or the best coffee spots in Solo ☕</p>
            <p><strong>📫 How to reach me:</strong> your.email@example.com</p>
            <p><strong>⚡ Looking for:</strong> Exciting open-source projects to contribute to!</p>
            
            <div style="margin-top: 30px; font-size: 18px;">
                <strong>Show some ❤️ by starring some of my repositories!</strong>
            </div>
        </div>
    </div>
    
    <script>
        // Typing animation
        const phrases = [
            "Full Stack Developer 💻",
            "Open Source Enthusiast ✨",
            "Always Learning New Things 🚀",
            "Coffee Powered Coder ☕"
        ];
        let phraseIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        const typingElement = document.getElementById('typing');
        
        function type() {
            const currentPhrase = phrases[phraseIndex];
            
            if (isDeleting) {
                typingElement.textContent = currentPhrase.substring(0, charIndex - 1);
                charIndex--;
            } else {
                typingElement.textContent = currentPhrase.substring(0, charIndex + 1);
                charIndex++;
            }
            
            if (!isDeleting && charIndex === currentPhrase.length) {
                isDeleting = true;
                setTimeout(type, 2000);
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                phraseIndex = (phraseIndex + 1) % phrases.length;
                setTimeout(type, 500);
            } else {
                setTimeout(type, isDeleting ? 50 : 100);
            }
        }
        
        type();
    </script>
</body>
</html>