
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Glushnev Mikhail Alekseevich">
    <meta name="description" content="MAG Industries – наши видео, TikTok, YouTube, связь с нами">
    <meta name="keywords" content="MAG industries, видео, TikTok, YouTube, стартап, технологии, 3D-принтер, Arduino, автомобили">
    <title>MAG Industries | Видео и связь</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Roboto:wght@300;400&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #F3A000;
            --red: #FF0000;
            --bg: #CCE1FE;
            --text: #222;
            --shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
            animation: fadeIn 1.5s ease-out;
        }
        
        /* Кнопка "назад" в левом верхнем углу */
        .back-btn {
            position: fixed;
            top: 15px;
            left: 15px;
            padding: 10px 18px;
            background: rgba(255,255,255,0.9);
            color: var(--text);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            border-radius: 30px;
            box-shadow: var(--shadow);
            transition: all 0.3s ease;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }
        
        .back-btn:hover {
            background: var(--primary);
            color: white;
            transform: translateY(-3px);
        }
        
        .hero {
            text-align: center;
            padding: 80px 20px 40px; /* Больше отступ сверху, чтобы кнопка не перекрывала логотип */
        }
        
        .logo {
            max-width: 320px;
            border-radius: 20px;
            box-shadow: var(--shadow);
            margin-bottom: 20px;
            transition: transform 0.5s ease;
            animation: slideUp 1s ease-out;
        }
        
        .logo:hover {
            transform: scale(1.05);
        }
        
        h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 3rem;
            color: var(--primary);
            margin: 0 0 10px 0;
        }
        
        .subtitle {
            font-size: 1.6rem;
            color: #333;
            font-weight: 500;
            margin-bottom: 40px;
        }
        
        .section {
            max-width: 1200px;
            margin: 60px auto;
            padding: 0 20px;
            text-align: center;
        }
        
        .section h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.4rem;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .section small {
            display: block;
            color: #555;
            margin-bottom: 40px;
        }
        
        .videos-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .video-card {
            opacity: 0;
            animation: fadeInUp 1s ease-out forwards;
        }
        
        .video-card a {
            display: block;
            text-decoration: none;
        }
        
        .video-card img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            border-radius: 15px;
            box-shadow: var(--shadow);
            transition: all 0.4s ease;
        }
        
        .video-card img:hover {
            transform: translateY(-10px) scale(1.03);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
            margin: 40px 0;
        }
        
        .social-links a {
            transition: transform 0.3s ease;
        }
        
        .social-links a:hover {
            transform: scale(1.2) translateY(-5px);
        }
        
        .social-links img {
            height: 60px;
            width: auto;
            border-radius: 12px;
            box-shadow: var(--shadow);
        }
        
        .email {
            font-size: 1.3rem;
            font-weight: 600;
            color: var(--red);
            margin: 30px 0;
        }
        
        .email a {
            color: var(--red);
            text-decoration: none;
        }
        
        .email a:hover {
            text-decoration: underline;
        }
        
        footer {
            text-align: center;
            padding: 40px;
            background: rgba(255,255,255,0.9);
            font-size: 0.9rem;
            color: #666;
            margin-top: 60px;
        }
        
        /* Анимации */
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideUp { from { opacity: 0; transform: translateY(50px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
        
        .video-card:nth-child(1) { animation-delay: 0.2s; }
        .video-card:nth-child(2) { animation-delay: 0.4s; }
        .video-card:nth-child(3) { animation-delay: 0.6s; }
        
        /* Мобильная адаптация */
        @media (max-width: 768px) {
            .back-btn {
                top: 10px;
                left: 10px;
                padding: 8px 14px;
                font-size: 0.9rem;
            }
            .hero {
                padding-top: 70px;
            }
            h1 { font-size: 2.4rem; }
            .subtitle { font-size: 1.4rem; }
            .section h2 { font-size: 2rem; }
            .logo { max-width: 280px; }
            .videos-grid { gap: 20px; }
            .video-card img { height: 240px; }
            .social-links { gap: 30px; }
            .social-links img { height: 50px; }
        }
    </style>
</head>
<body>

    <a href="https://mag858.github.io/MAG-industries/" class="back-btn">← На главную</a>

    <section class="hero">
        <img src="sait/logo_2.jpeg" alt="Логотип MAG Industries" class="logo">
        <h1>future - right now</h1>
        <div class="subtitle">(будущее - прямо сейчас)</div>
    </section>

    <section class="section">
        <h2>НАШИ ВИДЕО</h2>
        <small>(кликай на них)</small>
        
        <div class="videos-grid">
            <div class="video-card">
                <a href="https://vm.tiktok.com/ZMh9j81cD" target="_blank">
                    <img src="sait/часы.jpeg" alt="Видео: часы">
                </a>
            </div>
            <div class="video-card">
                <a href="https://vm.tiktok.com/ZMh92W2Lq" target="_blank">
                    <img src="sait/превью.jpeg" alt="Видео: превью">
                </a>
            </div>
            <div class="video-card">
                <a href="https://vm.tiktok.com/ZMh9j4yQW" target="_blank">
                    <img src="sait/колонка.jpeg" alt="Видео: колонка">
                </a>
            </div>
        </div>
    </section>

    <section class="section">
        <h2>СВЯЗЬ С НАМИ</h2>
        
        <div class="social-links">
            <a href="https://www.tiktok.com/@mag.industries?_t=8qtjY9aKcGE" target="_blank">
                <img src="sait/tiktok.jpg" alt="TikTok MAG Industries">
            </a>
            <a href="https://www.youtube.com/@MAGindustries-h4b" target="_blank">
                <img src="sait/youtube.jpg" alt="YouTube MAG Industries">
            </a>
        </div>
        
        <div class="email">
            <a href="mailto:magind000@gmail.com">почта: magind000@gmail.com</a>
        </div>
    </section>

    <footer>
        обновление 3.1 &emsp; январь 2026 г.
    </footer>

</body>
</html>	
		
