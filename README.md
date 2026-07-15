<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BEZEEEEETTTTTT - Developer Profile</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@400;500;600;700&family=Share+Tech+Mono&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #0a0a0a;
            color: #e0e0e0;
            font-family: 'Rajdhani', sans-serif;
            min-height: 100vh;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* ===== HEADER BANNER ===== */
        .header-banner {
            background: linear-gradient(135deg, #1a0000 0%, #0d0d0d 50%, #1a0000 100%);
            border: 1px solid #ff1a1a;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 20px;
            position: relative;
            overflow: hidden;
        }

        .header-banner::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(ellipse at 20% 50%, rgba(255, 0, 0, 0.1) 0%, transparent 50%),
                radial-gradient(ellipse at 80% 50%, rgba(255, 0, 0, 0.05) 0%, transparent 50%);
            pointer-events: none;
        }

        .header-top {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        .header-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 3rem;
            font-weight: 900;
            color: #ff1a1a;
            text-shadow: 0 0 20px rgba(255, 26, 26, 0.5), 0 0 40px rgba(255, 26, 26, 0.3);
            letter-spacing: 4px;
        }

        .header-subtitle {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.2rem;
            color: #ffffff;
            letter-spacing: 6px;
            text-align: center;
            margin-top: 5px;
        }

        .header-image {
            display: flex;
            gap: 15px;
            align-items: center;
        }

        .spiderman-img {
            width: 120px;
            height: 120px;
            border-radius: 8px;
            object-fit: cover;
        }

        /* ===== STATS BADGES ===== */
        .stats-bar {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .stat-badge {
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 26, 26, 0.15);
            border: 1px solid #ff1a1a;
            border-radius: 25px;
            padding: 8px 20px;
            font-family: 'Share Tech Mono', monospace;
            font-size: 0.95rem;
            color: #ff4444;
            transition: all 0.3s ease;
        }

        .stat-badge:hover {
            background: rgba(255, 26, 26, 0.3);
            transform: translateY(-2px);
            box-shadow: 0 4px 15px rgba(255, 26, 26, 0.3);
        }

        .stat-badge .icon {
            font-size: 1.1rem;
        }

        .stat-badge .count {
            color: #ffffff;
            font-weight: 700;
        }

        /* ===== TYPING ANIMATION CONTAINER ===== */
        .typing-container {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 20px;
            text-align: center;
        }

        .typing-container img {
            max-width: 100%;
            height: auto;
        }

        /* ===== MAIN CONTENT ===== */
        .main-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin-bottom: 20px;
        }

        /* ===== CONTENT AREA ===== */
        .content-area {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        /* ===== ABOUT ME SECTION ===== */
        .about-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 30px;
            position: relative;
            overflow: hidden;
        }

        .about-section::before {
            content: '🕷️';
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 3rem;
            opacity: 0.1;
        }

        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.8rem;
            color: #ff1a1a;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .about-list {
            list-style: none;
            padding: 0;
        }

        .about-list li {
            font-size: 1.1rem;
            margin-bottom: 12px;
            padding-left: 30px;
            position: relative;
            color: #cccccc;
            line-height: 1.6;
        }

        .about-list li::before {
            content: '▹';
            position: absolute;
            left: 0;
            color: #ff1a1a;
            font-size: 1.3rem;
            font-weight: bold;
        }

        /* ===== TECH STACK SECTION ===== */
        .tech-stack-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 30px;
            text-align: center;
        }

        .tech-icons-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .tech-icons-container img {
            height: 50px;
            transition: all 0.3s ease;
        }

        .tech-icons-container img:hover {
            transform: translateY(-5px) scale(1.1);
            filter: drop-shadow(0 0 10px rgba(255, 26, 26, 0.5));
        }

        /* ===== SNAKE ANIMATION SECTION ===== */
        .snake-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 20px;
            text-align: center;
        }

        .snake-section img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
        }

        /* ===== WHO AM I SECTION ===== */
        .whoami-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 25px;
            position: relative;
        }

        .whoami-header {
            text-align: right;
            margin-bottom: 20px;
        }

        .whoami-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.3rem;
            color: #ffffff;
            margin-bottom: 15px;
        }

        .whoami-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            align-items: center;
        }

        @media (max-width: 768px) {
            .whoami-content {
                grid-template-columns: 1fr;
            }
        }

        .spider-mask {
            width: 100%;
            max-width: 280px;
            margin: 0 auto;
            display: block;
        }

        .whoami-text {
            font-size: 0.95rem;
            line-height: 1.8;
            color: #cccccc;
        }

        .whoami-text p {
            margin-bottom: 15px;
        }

        .highlight-text {
            color: #ff4444;
            font-weight: 600;
        }

        /* ===== SOCIAL LINKS ===== */
        .social-section {
            text-align: center;
            padding: 20px;
        }

        .social-title {
            font-family: 'Share Tech Mono', monospace;
            color: #888888;
            margin-bottom: 15px;
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .social-link {
            display: flex;
            align-items: center;
            gap: 8px;
            background: rgba(255, 26, 26, 0.1);
            border: 1px solid #ff1a1a;
            border-radius: 8px;
            padding: 10px 20px;
            color: #ff4444;
            text-decoration: none;
            font-family: 'Share Tech Mono', monospace;
            font-size: 0.9rem;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background: rgba(255, 26, 26, 0.25);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255, 26, 26, 0.3);
        }

        /* ===== CAUTION SECTION ===== */
        .caution-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 25px;
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .caution-icon {
            font-size: 2rem;
            color: #ff4444;
        }

        .caution-content {
            flex: 1;
        }

        .caution-title {
            font-family: 'Orbitron', sans-serif;
            color: #ff4444;
            font-size: 1.1rem;
            margin-bottom: 10px;
        }

        .caution-quote {
            font-style: italic;
            color: #cccccc;
            line-height: 1.6;
            font-size: 0.95rem;
        }

        .caution-spider {
            font-size: 3rem;
            opacity: 0.8;
        }

        /* ===== CONTRIBUTIONS SECTION ===== */
        .contributions-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 25px;
            text-align: center;
        }

        .section-header {
            position: relative;
            display: inline-block;
            margin-bottom: 20px;
        }

        .section-header-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem;
            color: #ff1a1a;
            text-shadow: 0 0 10px rgba(255, 26, 26, 0.5);
            padding: 10px 30px;
            position: relative;
        }

        .section-header-title::before,
        .section-header-title::after {
            content: '◆';
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            color: #ff1a1a;
            font-size: 1rem;
        }

        .section-header-title::before {
            left: 5px;
        }

        .section-header-title::after {
            right: 5px;
        }

        .contribution-chart {
            width: 100%;
            height: 200px;
            background: rgba(0, 0, 0, 0.5);
            border: 1px solid #2a2a2a;
            border-radius: 8px;
            position: relative;
            overflow: hidden;
        }

        .chart-svg {
            width: 100%;
            height: 100%;
        }

        /* ===== TOP TRACKS SECTION ===== */
        .toptracks-section {
            background: linear-gradient(180deg, #111111 0%, #0a0a0a 100%);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 25px;
        }

        .toptracks-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        @media (max-width: 768px) {
            .toptracks-grid {
                grid-template-columns: 1fr;
            }
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
        }

        .tech-icon {
            width: 45px;
            height: 45px;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 0.8rem;
            color: white;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .tech-icon:hover {
            transform: scale(1.15) rotate(5deg);
        }

        .tech-html { background: #e34f26; }
        .tech-css { background: #1572b6; }
        .tech-js { background: #f7df1e; color: #000; }
        .tech-ts { background: #3178c6; }
        .tech-c { background: #00599c; }
        .tech-cpp { background: #004482; }
        .tech-python { background: #3776ab; }
        .tech-java { background: #007396; }
        .tech-php { background: #777bb4; }
        .tech-ruby { background: #cc342d; }
        .tech-go { background: #00add8; }
        .tech-rust { background: #dea584; color: #000; }
        .tech-swift { background: #f05138; }
        .tech-kotlin { background: #7f52ff; }
        .tech-dart { background: #0175c2; }
        .tech-react { background: #61dafb; color: #000; }
        .tech-vue { background: #4fc08d; }
        .tech-angular { background: #dd0031; }
        .tech-node { background: #339933; }
        .tech-mongo { background: #47a248; }
        .tech-git { background: #f05032; }
        .tech-docker { background: #2496ed; }
        .tech-aws { background: #ff9900; color: #000; }
        .tech-figma { background: #f24e1e; }

        /* ===== PROJECT CARD ===== */
        .project-card {
            background: rgba(0, 0, 0, 0.5);
            border: 1px solid #2a2a2a;
            border-radius: 10px;
            padding: 20px;
        }

        .project-name {
            font-family: 'Share Tech Mono', monospace;
            color: #ff4444;
            font-size: 1rem;
            margin-bottom: 10px;
        }

        .project-desc {
            font-size: 0.85rem;
            color: #aaaaaa;
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .project-stats {
            display: flex;
            gap: 15px;
            font-size: 0.85rem;
            color: #888888;
        }

        .project-stat {
            display: flex;
            align-items: center;
            gap: 5px;
        }

        /* ===== STATS CARDS ===== */
        .stats-cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .stats-cards {
                grid-template-columns: 1fr;
            }
        }

        .stats-card {
            background: rgba(0, 0, 0, 0.5);
            border: 1px solid #2a2a2a;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
        }

        .stats-card-number {
            font-family: 'Orbitron', sans-serif;
            font-size: 2rem;
            font-weight: 900;
            color: #ffffff;
            margin-bottom: 5px;
        }

        .stats-card-label {
            font-size: 0.8rem;
            color: #888888;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .stats-card-sub {
            font-size: 0.7rem;
            color: #666666;
            margin-top: 5px;
        }

        /* ===== ANIMATIONS ===== */
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }

        @keyframes glow {
            0%, 100% { box-shadow: 0 0 5px rgba(255, 26, 26, 0.3); }
            50% { box-shadow: 0 0 20px rgba(255, 26, 26, 0.6); }
        }

        .glow-effect {
            animation: glow 2s ease-in-out infinite;
        }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .animate-in {
            animation: slideIn 0.6s ease-out forwards;
        }

        /* ===== SCROLLBAR ===== */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: #0a0a0a;
        }

        ::-webkit-scrollbar-thumb {
            background: #ff1a1a;
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: #ff4444;
        }

        /* ===== WEB SPIDER DECORATION ===== */
        .web-decoration {
            position: fixed;
            top: 0;
            right: 0;
            width: 200px;
            height: 200px;
            opacity: 0.05;
            pointer-events: none;
            z-index: 0;
        }

        .web-decoration svg {
            width: 100%;
            height: 100%;
        }
    </style>
</head>
<body>

    <!-- Web Decoration Background -->
    <div class="web-decoration">
        <svg viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M100 0 L100 200 M0 100 L200 100 M29 29 L171 171 M171 29 L29 171" stroke="#ff1a1a" stroke-width="1"/>
            <circle cx="100" cy="100" r="30" stroke="#ff1a1a" stroke-width="1" fill="none"/>
            <circle cx="100" cy="100" r="60" stroke="#ff1a1a" stroke-width="1" fill="none"/>
            <circle cx="100" cy="100" r="90" stroke="#ff1a1a" stroke-width="1" fill="none"/>
        </svg>
    </div>

    <div class="container">
        
        <!-- ===== HEADER BANNER ===== -->
        <div class="header-banner animate-in">
            <div class="header-top">
                <div>
                    <h1 class="header-title">BEZEEEEETTTTTT</h1>
                    <p class="header-subtitle">DEVELOPER</p>
                </div>
                <div class="header-image">
                    <svg class="spiderman-img" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg">
                        <!-- Spider-Man Classic -->
                        <circle cx="60" cy="40" r="25" fill="#e31e24"/>
                        <circle cx="60" cy="40" r="25" fill="none" stroke="#1a1a2e" stroke-width="2"/>
                        <ellipse cx="50" cy="35" rx="10" ry="12" fill="white" stroke="#1a1a2e" stroke-width="2"/>
                        <ellipse cx="70" cy="35" rx="10" ry="12" fill="white" stroke="#1a1a2e" stroke-width="2"/>
                        <path d="M35 65 Q60 55 85 65 L90 110 Q60 100 30 110 Z" fill="#e31e24"/>
                        <path d="M35 65 Q60 55 85 65" fill="none" stroke="#1a1a2e" stroke-width="2"/>
                        <path d="M60 65 L60 110" stroke="#1a1a2e" stroke-width="1.5"/>
                        <path d="M45 70 Q60 65 75 70" stroke="#1a1a2e" stroke-width="1"/>
                        <path d="M40 80 Q60 75 80 80" stroke="#1a1a2e" stroke-width="1"/>
                        <path d="M35 90 Q60 85 85 90" stroke="#1a1a2e" stroke-width="1"/>
                        <path d="M32 100 Q60 95 88 100" stroke="#1a1a2e" stroke-width="1"/>
                    </svg>
                    <svg class="spiderman-img" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg">
                        <!-- Miles Morales Spider-Man -->
                        <circle cx="60" cy="40" r="25" fill="#1a1a1a"/>
                        <circle cx="60" cy="40" r="25" fill="none" stroke="#e31e24" stroke-width="2"/>
                        <ellipse cx="50" cy="35" rx="10" ry="12" fill="#e31e24" stroke="#1a1a1a" stroke-width="2"/>
                        <ellipse cx="70" cy="35" rx="10" ry="12" fill="#e31e24" stroke="#1a1a1a" stroke-width="2"/>
                        <path d="M35 65 Q60 55 85 65 L90 110 Q60 100 30 110 Z" fill="#1a1a1a"/>
                        <path d="M35 65 Q60 55 85 65" fill="none" stroke="#e31e24" stroke-width="2"/>
                        <path d="M60 65 L60 110" stroke="#e31e24" stroke-width="1.5"/>
                        <path d="M45 70 Q60 65 75 70" stroke="#e31e24" stroke-width="1"/>
                        <path d="M40 80 Q60 75 80 80" stroke="#e31e24" stroke-width="1"/>
                        <path d="M35 90 Q60 85 85 90" stroke="#e31e24" stroke-width="1"/>
                        <!-- Lightning bolt -->
                        <path d="M55 75 L65 85 L58 85 L62 95" fill="#e31e24" stroke="none"/>
                    </svg>
                </div>
            </div>

            <!-- Stats Bar -->
            <div class="stats-bar">
                <div class="stat-badge">
                    <span class="icon">⭐</span>
                    <span>STARS</span>
                    <span class="count">28</span>
                </div>
                <div class="stat-badge">
                    <span class="icon">🍴</span>
                    <span>FORKS</span>
                    <span class="count">2</span>
                </div>
                <div class="stat-badge">
                    <span class="icon">👥</span>
                    <span>FOLLOWERS</span>
                    <span class="count">32</span>
                </div>
            </div>
        </div>

        <!-- ===== TYPING ANIMATION ===== -->
        <div class="typing-container animate-in">
            <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=1000&color=FF0000&center=true&vCenter=true&width=700&lines=Hi,+I'm+Bezeeetttt+🕸️;Web+Developer+—+coding+to+save+the+day." alt="Typing Animation" />
        </div>

        <!-- ===== MAIN CONTENT ===== -->
        <div class="main-grid">
            
            <!-- ===== CONTENT AREA ===== -->
            <div class="content-area">
                
                <!-- About Me Section -->
                <div class="about-section animate-in">
                    <h2 class="section-title">🕷️ About Me:</h2>
                    <ul class="about-list">
                        <li>🕸️ UI/UX & Design Enthusiast</li>
                        <li>💻 Web Developer — coding with great power and responsibility</li>
                        <li> Love building dynamic and responsive projects</li>
                        <li>🎮 Gamer at heart</li>
                    </ul>
                </div>

                <!-- Tech Stack Section -->
                <div class="tech-stack-section animate-in">
                    <h2 class="section-title" style="justify-content: center;">💻 Tech Stack:</h2>
                    <div class="tech-icons-container">
                        <img src="https://skillicons.dev/icons?i=mysql,js,figma,github,gitlab" alt="Tech Stack" />
                    </div>
                </div>

                <!-- Snake Animation Section -->
                <div class="snake-section animate-in">
                    <img src="https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg" alt="GitHub Contribution Snake" />
                </div>

                <!-- Who Am I Section -->
                <div class="whoami-section animate-in">
                    <div class="whoami-header">
                        <h2 class="whoami-title">Who Am I?</h2>
                    </div>
                    <div class="whoami-content">
                        <div class="whoami-text">
                            <p>I am a graduated <span class="highlight-text">Software Developer</span> with a degree in System, analyst and <span class="highlight-text">develop</span>ment, currently working as a freelancer while actively seeking an opportunity in the technology field. My professional journey is driven by continuous learning, practical commitment, and a strong commitment to delivering complete and functional systems for real-world needs.</p>
                            <p>Over time, I have developed solid experience across the web development ecosystem, with a strong passion for <span class="highlight-text">Front-End Development</span>, where logic meets creativity and visual design. Alongside web technologies, I have expanded my skills into mobile development, focusing on building modern applications using <span class="highlight-text">Android Studio</span> and <span class="highlight-text">React Native</span>.</p>
                        </div>
                        <div>
                            <svg class="spider-mask" viewBox="0 0 280 280" xmlns="http://www.w3.org/2000/svg">
                                <!-- Spider-Man Mask -->
                                <defs>
                                    <radialGradient id="maskGrad" cx="50%" cy="50%" r="50%">
                                        <stop offset="0%" style="stop-color:#ff3333"/>
                                        <stop offset="100%" style="stop-color:#cc0000"/>
                                    </radialGradient>
                                    <filter id="glow">
                                        <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
                                        <feMerge>
                                            <feMergeNode in="coloredBlur"/>
                                            <feMergeNode in="SourceGraphic"/>
                                        </feMerge>
                                    </filter>
                                </defs>
                                <!-- Mask shape -->
                                <path d="M140 20 C200 20, 260 60, 260 140 C260 220, 200 270, 140 270 C80 270, 20 220, 20 140 C20 60, 80 20, 140 20 Z" 
                                      fill="url(#maskGrad)" stroke="#ff1a1a" stroke-width="2" filter="url(#glow)"/>
                                <!-- Web pattern -->
                                <path d="M140 20 L140 270" stroke="#1a0000" stroke-width="1.5" opacity="0.6"/>
                                <path d="M20 140 L260 140" stroke="#1a0000" stroke-width="1.5" opacity="0.6"/>
                                <path d="M55 55 L225 225" stroke="#1a0000" stroke-width="1.5" opacity="0.6"/>
                                <path d="M225 55 L55 225" stroke="#1a0000" stroke-width="1.5" opacity="0.6"/>
                                <path d="M140 20 Q140 140 260 140" stroke="#1a0000" stroke-width="1" fill="none" opacity="0.4"/>
                                <path d="M140 20 Q140 140 20 140" stroke="#1a0000" stroke-width="1" fill="none" opacity="0.4"/>
                                <path d="M140 270 Q140 140 260 140" stroke="#1a0000" stroke-width="1" fill="none" opacity="0.4"/>
                                <path d="M140 270 Q140 140 20 140" stroke="#1a0000" stroke-width="1" fill="none" opacity="0.4"/>
                                <!-- Eyes -->
                                <path d="M70 120 Q90 80, 130 100 Q140 120, 120 150 Q90 160, 70 140 Z" 
                                      fill="#1a0000" stroke="#ff1a1a" stroke-width="2"/>
                                <path d="M210 120 Q190 80, 150 100 Q140 120, 160 150 Q190 160, 210 140 Z" 
                                      fill="#1a0000" stroke="#ff1a1a" stroke-width="2"/>
                                <!-- Eye inner glow -->
                                <path d="M80 120 Q95 95, 120 108 Q128 120, 115 140 Q95 148, 80 135 Z" 
                                      fill="#ff1a1a" opacity="0.3"/>
                                <path d="M200 120 Q185 95, 160 108 Q152 120, 165 140 Q185 148, 200 135 Z" 
                                      fill="#ff1a1a" opacity="0.3"/>
                            </svg>
                        </div>
                    </div>
                    <div class="whoami-text" style="margin-top: 20px;">
                        <p>At the moment, I am working as a freelancer, developing complete systems for companies in my city, from planning and interface design to implementation and delivery. This hands-on experience has strengthened my problem-solving skills, technical versatility, and ability to understand business needs, while constantly pushing me to grow as a developer and professional.</p>
                    </div>
                </div>

                <!-- Social Links -->
                <div class="social-section animate-in">
                    <p class="social-title">You can Click here</p>
                    <div class="social-links">
                        <a href="#" class="social-link">
                            <span>📌</span> PINTEREST
                        </a>
                        <a href="#" class="social-link">
                            <span>💼</span> LINKEDIN
                        </a>
                        <a href="#" class="social-link">
                            <span>📧</span> GMAIL
                        </a>
                    </div>
                </div>

                <!-- Caution Section -->
                <div class="caution-section animate-in">
                    <span class="caution-icon">⚠️</span>
                    <div class="caution-content">
                        <h3 class="caution-title">Caution</h3>
                        <p class="caution-quote">Code is never finished, it only gets better.</p>
                        <p class="caution-quote">What you see here is built with practice, curiosity, and persistence.</p>
                    </div>
                    <span class="caution-spider">🕷️</span>
                </div>

                <!-- Contributions Section -->
                <div class="contributions-section animate-in">
                    <div class="section-header">
                        <h2 class="section-header-title">My Contributions</h2>
                    </div>
                    <div class="contribution-chart">
                        <svg class="chart-svg" viewBox="0 0 800 200" xmlns="http://www.w3.org/2000/svg">
                            <!-- Grid lines -->
                            <line x1="50" y1="20" x2="50" y2="180" stroke="#2a2a2a" stroke-width="1"/>
                            <line x1="50" y1="180" x2="780" y2="180" stroke="#2a2a2a" stroke-width="1"/>
                            <line x1="50" y1="140" x2="780" y2="140" stroke="#2a2a2a" stroke-width="0.5" stroke-dasharray="4"/>
                            <line x1="50" y1="100" x2="780" y2="100" stroke="#2a2a2a" stroke-width="0.5" stroke-dasharray="4"/>
                            <line x1="50" y1="60" x2="780" y2="60" stroke="#2a2a2a" stroke-width="0.5" stroke-dasharray="4"/>
                            <line x1="50" y1="20" x2="780" y2="20" stroke="#2a2a2a" stroke-width="0.5" stroke-dasharray="4"/>
                            
                            <!-- Y-axis labels -->
                            <text x="40" y="183" fill="#666" font-size="10" text-anchor="end">0</text>
                            <text x="40" y="143" fill="#666" font-size="10" text-anchor="end">5</text>
                            <text x="40" y="103" fill="#666" font-size="10" text-anchor="end">10</text>
                            <text x="40" y="63" fill="#666" font-size="10" text-anchor="end">15</text>
                            <text x="40" y="23" fill="#666" font-size="10" text-anchor="end">20</text>
                            
                            <!-- X-axis labels -->
                            <text x="100" y="195" fill="#666" font-size="10" text-anchor="middle">Jan</text>
                            <text x="200" y="195" fill="#666" font-size="10" text-anchor="middle">Mar</text>
                            <text x="300" y="195" fill="#666" font-size="10" text-anchor="middle">May</text>
                            <text x="400" y="195" fill="#666" font-size="10" text-anchor="middle">Jul</text>
                            <text x="500" y="195" fill="#666" font-size="10" text-anchor="middle">Sep</text>
                            <text x="600" y="195" fill="#666" font-size="10" text-anchor="middle">Nov</text>
                            <text x="700" y="195" fill="#666" font-size="10" text-anchor="middle">Dec</text>
                            
                            <!-- Area fill -->
                            <path d="M80 170 L130 165 L180 160 L230 155 L280 150 L330 140 L380 130 L430 110 L480 80 L530 50 L580 35 L630 45 L680 70 L730 100 L760 130 L760 180 L80 180 Z" 
                                  fill="rgba(255, 26, 26, 0.15)"/>
                            
                            <!-- Line -->
                            <path d="M80 170 L130 165 L180 160 L230 155 L280 150 L330 140 L380 130 L430 110 L480 80 L530 50 L580 35 L630 45 L680 70 L730 100 L760 130" 
                                  fill="none" stroke="#ff1a1a" stroke-width="2.5" filter="url(#glow)"/>
                            
                            <!-- Data points -->
                            <circle cx="80" cy="170" r="4" fill="#ff1a1a"/>
                            <circle cx="180" cy="160" r="4" fill="#ff1a1a"/>
                            <circle cx="280" cy="150" r="4" fill="#ff1a1a"/>
                            <circle cx="380" cy="130" r="4" fill="#ff1a1a"/>
                            <circle cx="480" cy="80" r="4" fill="#ff1a1a"/>
                            <circle cx="580" cy="35" r="5" fill="#ff1a1a" stroke="#fff" stroke-width="1.5"/>
                            <circle cx="680" cy="70" r="4" fill="#ff1a1a"/>
                            <circle cx="760" cy="130" r="4" fill="#ff1a1a"/>
                            
                            <!-- Title -->
                            <text x="400" y="15" fill="#ff4444" font-size="12" text-anchor="middle" font-family="Orbitron">My Contributions</text>
                        </svg>
                    </div>
                </div>

                <!-- Top Tracks Section -->
                <div class="toptracks-section animate-in">
                    <div class="section-header">
                        <h2 class="section-header-title">My Top Tracks</h2>
                    </div>
                    <div class="toptracks-grid">
                        <!-- Tech Stack Icons -->
                        <div>
                            <div class="tech-stack">
                                <div class="tech-icon tech-html">HTML</div>
                                <div class="tech-icon tech-css">CSS</div>
                                <div class="tech-icon tech-js">JS</div>
                                <div class="tech-icon tech-ts">TS</div>
                                <div class="tech-icon tech-c">C</div>
                                <div class="tech-icon tech-cpp">C++</div>
                                <div class="tech-icon tech-python">PY</div>
                                <div class="tech-icon tech-java">JV</div>
                                <div class="tech-icon tech-php">PHP</div>
                                <div class="tech-icon tech-ruby">RB</div>
                                <div class="tech-icon tech-go">GO</div>
                                <div class="tech-icon tech-rust">RS</div>
                                <div class="tech-icon tech-swift">SW</div>
                                <div class="tech-icon tech-kotlin">KT</div>
                                <div class="tech-icon tech-dart">DT</div>
                                <div class="tech-icon tech-react"></div>
                                <div class="tech-icon tech-vue">V</div>
                                <div class="tech-icon tech-angular">A</div>
                                <div class="tech-icon tech-node">N</div>
                                <div class="tech-icon tech-mongo">M</div>
                                <div class="tech-icon tech-git">G</div>
                                <div class="tech-icon tech-docker">D</div>
                                <div class="tech-icon tech-aws">AWS</div>
                                <div class="tech-icon tech-figma">F</div>
                            </div>
                        </div>

                        <!-- Project Card -->
                        <div class="project-card">
                            <h4 class="project-name">📱 Lembre-Plus-note-app</h4>
                            <p class="project-desc">
                                A clean and organized note-taking app for iOS and Android. 
                                Built with React Native, featuring cloud sync, categories, 
                                and a minimalist UI. Perfect for daily notes, goals, and reminders.
                            </p>
                            <div class="project-stats">
                                <span class="project-stat">⭐ 0</span>
                                <span class="project-stat">🍴 0</span>
                            </div>
                        </div>
                    </div>

                    <!-- Stats Cards -->
                    <div class="stats-cards">
                        <div class="stats-card">
                            <div class="stats-card-number">573</div>
                            <div class="stats-card-label">Total</div>
                            <div class="stats-card-sub">Sep 3, 2024</div>
                        </div>
                        <div class="stats-card">
                            <div class="stats-card-number">2</div>
                            <div class="stats-card-label">Current Streak</div>
                            <div class="stats-card-sub">Oct 13 - Oct 14</div>
                        </div>
                        <div class="stats-card">
                            <div class="stats-card-number">42</div>
                            <div class="stats-card-label">Contributions</div>
                            <div class="stats-card-sub">Max: 12 · 2024</div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>

    <script>
        // Intersection Observer for animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.animate-in').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(el);
        });

        // Add hover effect to tech icons
        document.querySelectorAll('.tech-icon').forEach(icon => {
            icon.addEventListener('mouseenter', function() {
                this.style.transform = 'scale(1.15) rotate(5deg)';
            });
            icon.addEventListener('mouseleave', function() {
                this.style.transform = 'scale(1) rotate(0deg)';
            });
        });

        // Animate stats numbers on load
        function animateNumber(element, target, duration = 1500) {
            let start = 0;
            const increment = target / (duration / 16);
            const timer = setInterval(() => {
                start += increment;
                if (start >= target) {
                    element.textContent = target;
                    clearInterval(timer);
                } else {
                    element.textContent = Math.floor(start);
                }
            }, 16);
        }

        // Trigger number animations when stats cards are visible
        const statsObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const numbers = entry.target.querySelectorAll('.stats-card-number');
                    numbers.forEach(num => {
                        const target = parseInt(num.textContent);
                        animateNumber(num, target);
                    });
                    statsObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.5 });

        const statsCards = document.querySelector('.stats-cards');
        if (statsCards) {
            statsObserver.observe(statsCards);
        }
    </script>

</body>
</html>
