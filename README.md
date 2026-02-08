<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMM Pro Academy | Профессиональное обучение SMM и digital-маркетингу</title>
    <meta name="description" content="курсы SMM и digital-маркетинга. Стань востребованным специалистом за 3 месяца. Практика с первых дней, помощь с трудоустройством.">
    <meta name="keywords" content="SMM обучение, курсы маркетинга, digital-маркетинг, таргетированная реклама, Instagram продвижение">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Manrope:wght@400;500;600;700&display=swap">
    <style>
        /* Общие стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #4361ee;
            --secondary-color: #3a0ca3;
            --accent-color: #f72585;
            --dark-color: #1a1a2e;
            --light-color: #f8f9fa;
            --text-color: #333;
            --transition: all 0.3s ease;
            --gradient: linear-gradient(135deg, #4361ee 0%, #3a0ca3 100%);
            --gradient-accent: linear-gradient(135deg, #f72585 0%, #b5179e 100%);
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--light-color);
            overflow-x: hidden;
        }

        h1, h2, h3, h4 {
            font-family: 'Manrope', sans-serif;
            font-weight: 700;
            margin-bottom: 1rem;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        section {
            padding: 80px 0;
        }

        .btn {
            display: inline-block;
            background: var(--gradient);
            color: white;
            padding: 14px 35px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            font-size: 16px;
            letter-spacing: 0.3px;
            box-shadow: 0 4px 15px rgba(67, 97, 238, 0.3);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(67, 97, 238, 0.4);
        }

        .btn-accent {
            background: var(--gradient-accent);
            box-shadow: 0 4px 15px rgba(247, 37, 133, 0.3);
        }

        .btn-accent:hover {
            box-shadow: 0 8px 25px rgba(247, 37, 133, 0.4);
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--dark-color);
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background: var(--gradient);
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        /* Шапка и навигация */
        header {
            background-color: white;
            box-shadow: 0 2px 20px rgba(0,0,0,0.08);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 18px 20px;
        }

        .logo {
            font-family: 'Manrope', sans-serif;
            font-size: 1.8rem;
            color: var(--dark-color);
            text-decoration: none;
            font-weight: 800;
            display: flex;
            align-items: center;
        }

        .logo span {
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .logo i {
            margin-right: 8px;
            color: var(--primary-color);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 35px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 600;
            transition: var(--transition);
            position: relative;
            font-size: 15px;
        }

        nav ul li a:hover {
            color: var(--primary-color);
        }

        nav ul li a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            background: var(--gradient);
            bottom: -5px;
            left: 0;
            transition: var(--transition);
        }

        nav ul li a:hover::after {
            width: 100%;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark-color);
            cursor: pointer;
        }

        /* Главный баннер */
        .hero {
            background: linear-gradient(rgba(26, 26, 46, 0.9), rgba(26, 26, 46, 0.85)), url('https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 180px 0 100px;
            margin-top: 70px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2.5rem;
            opacity: 0.9;
            line-height: 1.7;
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 50px;
            margin-top: 60px;
            flex-wrap: wrap;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 800;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 5px;
        }

        .stat-text {
            font-size: 1rem;
            opacity: 0.8;
            font-weight: 500;
        }

        /* Курсы */
        .courses-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .course-card {
            background-color: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            transition: var(--transition);
            border: 1px solid #eee;
        }

        .course-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.12);
        }

        .course-badge {
            background: var(--gradient-accent);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            position: absolute;
            top: 15px;
            right: 15px;
        }

        .course-img {
            height: 200px;
            width: 100%;
            object-fit: cover;
        }

        .course-content {
            padding: 25px;
        }

        .course-content h3 {
            color: var(--dark-color);
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .course-price {
            font-size: 1.8rem;
            font-weight: 800;
            color: var(--primary-color);
            margin: 15px 0;
        }

        .course-price span {
            font-size: 1rem;
            color: #777;
            text-decoration: line-through;
            margin-left: 10px;
        }

        .course-features {
            list-style: none;
            margin: 20px 0;
        }

        .course-features li {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .course-features i {
            color: var(--primary-color);
            margin-right: 10px;
            font-size: 0.9rem;
        }

        /* Преимущества обучения */
        .advantages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }

        .advantage-card {
            text-align: center;
            padding: 35px 25px;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            transition: var(--transition);
        }

        .advantage-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .advantage-icon {
            font-size: 2.8rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 20px;
        }

        .advantage-card h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
        }

        /* Вебинары и видео */
        .webinar-section {
            background-color: #f0f4ff;
        }

        .webinar-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .webinar-content h2 {
            text-align: left;
        }

        .webinar-content h2::after {
            left: 0;
            transform: none;
        }

        .video-container {
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .video-placeholder {
            width: 100%;
            height: 300px;
            background: linear-gradient(135deg, #4361ee 0%, #3a0ca3 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            color: white;
        }

        .video-placeholder i {
            font-size: 4rem;
            margin-bottom: 20px;
        }

        /* Отзывы студентов */
        .reviews-section {
            background-color: var(--light-color);
        }

        .reviews-slider {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
        }

        .review-slide {
            background-color: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
            text-align: center;
            margin: 0 15px;
        }

        .student-photo {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 20px;
            border: 5px solid var(--primary-color);
        }

        .review-text {
            font-style: italic;
            margin-bottom: 20px;
            font-size: 1.1rem;
            line-height: 1.7;
        }

        .student-name {
            font-weight: 700;
            color: var(--dark-color);
            margin-bottom: 5px;
        }

        .student-position {
            color: #777;
            font-size: 0.9rem;
        }

        .slider-controls {
            display: flex;
            justify-content: center;
            margin-top: 30px;
        }

        .slider-btn {
            background: white;
            border: 2px solid #eee;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            color: var(--primary-color);
            cursor: pointer;
            margin: 0 10px;
            transition: var(--transition);
        }

        .slider-btn:hover {
            background: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }

        /* Форма записи на курс */
        .booking-section {
            background: linear-gradient(rgba(26, 26, 46, 0.9), rgba(26, 26, 46, 0.9)), url('https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
        }

        .booking-section .section-title {
            color: white;
        }

        .booking-section .section-title::after {
            background: var(--gradient-accent);
        }

        .booking-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .form-control {
            width: 100%;
            padding: 14px 15px;
            border-radius: 8px;
            border: 1px solid rgba(255,255,255,0.3);
            background-color: rgba(255,255,255,0.1);
            color: white;
            font-family: 'Inter', sans-serif;
            font-size: 16px;
        }

        .form-control::placeholder {
            color: rgba(255,255,255,0.7);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary-color);
        }

        /* Подвал */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-logo {
            font-family: 'Manrope', sans-serif;
            font-size: 2rem;
            font-weight: 800;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }

        .footer-logo span {
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .footer-logo i {
            margin-right: 10px;
            color: var(--primary-color);
        }

        .footer-about p {
            opacity: 0.8;
            margin-bottom: 25px;
            line-height: 1.7;
        }

        .social-links {
            display: flex;
            gap: 15px;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 42px;
            height: 42px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }

        .social-links a:hover {
            background: var(--gradient);
            transform: translateY(-3px);
        }

        .footer-heading {
            font-size: 1.3rem;
            margin-bottom: 25px;
            position: relative;
            font-family: 'Manrope', sans-serif;
        }

        .footer-heading::after {
            content: '';
            position: absolute;
            width: 40px;
            height: 3px;
            background: var(--gradient);
            bottom: -8px;
            left: 0;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links ul li {
            margin-bottom: 12px;
        }

        .footer-links ul li a {
            color: rgba(255,255,255,0.8);
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links ul li a:hover {
            color: var(--primary-color);
            padding-left: 5px;
        }

        .contact-info p {
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            line-height: 1.6;
        }

        .contact-info i {
            margin-right: 10px;
            color: var(--primary-color);
            margin-top: 5px;
            min-width: 20px;
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }

        /* Адаптивность */
        @media (max-width: 1100px) {
            .webinar-container {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            
            .webinar-content h2 {
                text-align: center;
            }
            
            .webinar-content h2::after {
                left: 50%;
                transform: translateX(-50%);
            }
        }

        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
        }

        @media (max-width: 768px) {
            nav ul {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: white;
                flex-direction: column;
                box-shadow: 0 10px 20px rgba(0,0,0,0.1);
                padding: 20px 0;
                z-index: 999;
            }

            nav ul.active {
                display: flex;
            }

            nav ul li {
                margin: 0;
                text-align: center;
                padding: 15px 0;
            }

            .mobile-menu-btn {
                display: block;
            }

            .hero h1 {
                font-size: 2.3rem;
            }
            
            .hero {
                padding: 150px 0 80px;
            }
            
            section {
                padding: 60px 0;
            }
            
            .courses-grid {
                grid-template-columns: 1fr;
            }
            
            .booking-form {
                padding: 30px 20px;
            }
            
            .hero-stats {
                gap: 30px;
            }
        }

        @media (max-width: 576px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .btn {
                padding: 12px 30px;
                font-size: 15px;
            }
            
            .course-card {
                margin-bottom: 20px;
            }
            
            .stat-number {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Шапка сайта -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo"><i class="fas fa-rocket"></i>SMM<span>nuri</span></a>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav>
                <ul id="mainMenu">
                    <li><a href="#home">Главная</a></li>
                    <li><a href="#courses">Курсы</a></li>
                    <li><a href="#advantages">Преимущества</a></li>
                    <li><a href="#webinars">Вебинары</a></li>
                    <li><a href="#reviews">Отзывы</a></li>
                    <li><a href="#booking" class="btn btn-accent" style="padding: 8px 20px;">Записаться</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Главный баннер -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Стань востребованным SMM-специалистом за 3 месяца</h1>
            <p>Практическое обучение digital-маркетингу от экспертов с опытом работы в крупнейших агентствах. Освойте востребованную профессию с нуля или повысьте квалификацию.</p>
            <a href="#booking" class="btn btn-accent">Начать обучение</a>
            
            <div class="hero-stats">
                <div class="stat-item">
                    <div class="stat-number">1500+</div>
                    <div class="stat-text">Выпускников</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">94%</div>
                    <div class="stat-text">Трудоустраиваются</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">28</div>
                    <div class="stat-text">Экспертов-практиков</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">85%</div>
                    <div class="stat-text">Практики в программе</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Курсы -->
    <section id="courses" class="courses">
        <div class="container">
            <h2 class="section-title">Наши курсы</h2>
            <div class="courses-grid">
                <div class="course-card">
                    <div class="course-badge">Топ-курс</div>
                    <img src="https://images.unsplash.com/photo-1611224923853-80b023f02d71?ixlib=rb-4.0.3&auto=format&fit=crop&w=1469&q=80" alt="SMM-специалист" class="course-img">
                    <div class="course-content">
                        <h3>SMM-специалист с нуля до PRO</h3>
                        <p>Полный курс по продвижению в социальных сетях. Научитесь создавать контент, вести рекламные кампании и увеличивать продажи.</p>
                        <ul class="course-features">
                            <li><i class="fas fa-check-circle"></i> Длительность: 4 месяца</li>
                            <li><i class="fas fa-check-circle"></i> 72 практических задания</li>
                            <li><i class="fas fa-check-circle"></i> Диплом о переквалификации</li>
                            <li><i class="fas fa-check-circle"></i> Помощь с трудоустройством</li>
                        </ul>
                        <div class="course-price">24 900 ₽ <span>39 900 ₽</span></div>
                        <a href="#booking" class="btn">Записаться на курс</a>
                    </div>
                </div>
                
                <div class="course-card">
                    <div class="course-badge">Новый</div>
                    <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80" alt="Таргетированная реклама" class="course-img">
                    <div class="course-content">
                        <h3>Таргетированная реклама PRO</h3>
                        <p>Углубленный курс по настройке рекламы в Facebook и Instagram. Научитесь привлекать клиентов с минимальными затратами.</p>
                        <ul class="course-features">
                            <li><i class="fas fa-check-circle"></i> Длительность: 2 месяца</li>
                            <li><i class="fas fa-check-circle"></i> 48 практических заданий</li>
                            <li><i class="fas fa-check-circle"></i> Работа с бизнес-кейсами</li>
                            <li><i class="fas fa-check-circle"></i> Сертификат специалиста</li>
                        </ul>
                        <div class="course-price">18 900 ₽ <span>29 900 ₽</span></div>
                        <a href="#booking" class="btn">Записаться на курс</a>
                    </div>
                </div>
                
                <div class="course-card">
                    <img src="https://images.unsplash.com/photo-1542744095-fcf48d80b0fd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1476&q=80" alt="Контент-маркетинг" class="course-img">
                    <div class="course-content">
                        <h3>Контент-маркетинг и стратегии</h3>
                        <p>Создание контент-стратегий для брендов. Научитесь создавать виральный контент и увеличивать вовлеченность аудитории.</p>
                        <ul class="course-features">
                            <li><i class="fas fa-check-circle"></i> Длительность: 2.5 месяца</li>
                            <li><i class="fas fa-check-circle"></i> 36 практических заданий</li>
                            <li><i class="fas fa-check-circle"></i> Кейсы известных брендов</li>
                            <li><i class="fas fa-check-circle"></i> Сертификат специалиста</li>
                        </ul>
                        <div class="course-price">16 900 ₽ <span>24 900 ₽</span></div>
                        <a href="#booking" class="btn">Записаться на курс</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Преимущества обучения -->
    <section id="advantages" class="advantages">
        <div class="container">
            <h2 class="section-title">Почему выбирают этот курс</h2>
            <div class="advantages-grid">
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-chalkboard-teacher"></i>
                    </div>
                    <h3>Эксперты-практики</h3>
                    <p>Преподает действующие SMM-специалисты с опытом работы в крупных агентствах и с известными брендами.</p>
                </div>
                
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-briefcase"></i>
                    </div>
                    <h3>Трудоустройство</h3>
                    <p>Помогаем с составлением резюме и портфолио, готовим к собеседованию, предлагаем вакансии от партнеров.</p>
                </div>
                
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3>Практика с 1-го дня</h3>
                    <p>85% обучения - практические задания и работа с реальными проектами. Теория закрепляется на практике.</p>
                </div>
                
                <div class="advantage-card">
                    <div class="advantage-icon">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3>Комьюнити</h3>
                    <p>Доступ к закрытому сообществу выпускников, обмен опытом, нетворкинг и поддержка после обучения.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Вебинары -->
    <section id="webinars" class="webinar-section">
        <div class="container">
            <div class="webinar-container">
                <div class="webinar-content">
                    <h2 class="section-title">Бесплатные вебинары от экспертов</h2>
                    <p>Каждую неделю проводим бесплатные вебинары по актуальным темам digital-маркетинга. Участие бесплатное, запись доступна 24 часа.</p>
                    <ul class="course-features" style="margin: 25px 0;">
                        <li><i class="fas fa-check-circle"></i> Тренды SMM 2024</li>
                        <li><i class="fas fa-check-circle"></i> Инструменты для аналитики</li>
                        <li><i class="fas fa-check-circle"></i> Кейсы успешных кампаний</li>
                        <li><i class="fas fa-check-circle"></i> Разбор ошибок начинающих</li>
                    </ul>
                    <a href="#booking" class="btn btn-accent">Записаться на ближайший вебинар</a>
                </div>
                
                <div class="video-container">
                    <div class="video-placeholder">
                        <i class="fas fa-video"></i>
                        <h3>Бесплатный вебинар</h3>
                        <p>"Как увеличить конверсию в Instagram на 300%"</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Отзывы -->
    <section id="reviews" class="reviews-section">
        <div class="container">
            <h2 class="section-title">Отзывы выпускников</h2>
            <div class="reviews-slider">
                <div class="review-slide">
                    <img src="https://randomuser.me/api/portraits/women/45.jpg" alt="Выпускница" class="student-photo">
                    <p class="review-text">"бамбавый курс"</p>
                    <h4 class="student-name">Анна Козлова</h4>
                    <p class="student-position">SMM-менеджер в AdvertFlow</p>
                </div>
                
                <div class="slider-controls">
                    <button class="slider-btn" id="prevBtn"><i class="fas fa-chevron-left"></i></button>
                    <button class="slider-btn" id="nextBtn"><i class="fas fa-chevron-right"></i></button>
                </div>
            </div>
        </div>
    </section>

    <!-- Форма записи -->
    <section id="booking" class="booking-section">
        <div class="container">
            <h2 class="section-title">Начните обучение сегодня</h2>
            <p style="text-align: center; max-width: 700px; margin: 0 auto 40px; opacity: 0.9;">Оставьте заявку, и наш менеджер свяжется с вами в течение 15 минут. Подберем подходящий курс и расскажем о программе обучения.</p>
            
            <form class="booking-form" id="bookingForm">
                <div class="form-group">
                    <label for="name">Ваше имя</label>
                    <input type="text" id="name" class="form-control" placeholder="Введите ваше имя" required>
                </div>
                
                <div class="form-group">
                    <label for="phone">Номер телефона</label>
                    <input type="tel" id="phone" class="form-control" placeholder="+7 (___) ___-__-__" required>
                </div>
                
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" class="form-control" placeholder="your.email@example.com" required>
                </div>
                
                <div class="form-group">
                    <label for="course">Выберите курс</label>
                    <select id="course" class="form-control" required>
                        <option value="" disabled selected>Выберите курс</option>
                        <option value="smm-pro">SMM-специалист с нуля до PRO</option>
                        <option value="target">Таргетированная реклама PRO</option>
                        <option value="content">Контент-маркетинг и стратегии</option>
                        <option value="consultation">Бесплатная консультация</option>
                        <option value="consultation">супер пупер</option>              
                        </select>
                </div>
                
                <button type="submit" class="btn btn-accent" style="width: 100%; padding: 16px;">Отправить заявку на обучение</button>
            </form>
        </div>
    </section>

    <!-- Подвал -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <div class="footer-logo"><i class="fas fa-rocket"></i>SMM<span>nuri</span> курс</div>
                    <p>Онлайн-курс digital-маркетинга №1 в России. Готовим востребованных специалистов с 2018 года. 1500+ выпускников работают в ведущих агентствах и компаниях.(с инета написала)</p>
                    <div class="social-links">
                        <a href="https://www.instagram.com/ssalya.aa?igsh=MTMzYTMzcjZvMW1ncA%3D%3D&utm_source=qr" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
                        <a href="https://facebook.com" target="_blank" title="Facebook"><i class="fab fa-facebook-f"></i></a>
                        <a href="https://vk.com" target="_blank" title="VK"><i class="fab fa-vk"></i></a>
                        <a href="https://youtube.com" target="_blank" title="YouTube"><i class="fab fa-youtube"></i></a>
                        <a href="https://t.me" target="_blank" title="Telegram"><i class="fab fa-telegram"></i></a>
                    </div>
                </div>
                
                <div class="footer-links">
                    <h3 class="footer-heading">Навигация</h3>
                    <ul>
                        <li><a href="#home">Главная</a></li>
                        <li><a href="#courses">Все курсы</a></li>
                        <li><a href="#advantages">Преимущества</a></li>
                        <li><a href="#webinars">Бесплатные вебинары</a></li>
                        <li><a href="#reviews">Отзывы выпускников</a></li>
                        <li><a href="#booking">Запись на курс</a></li>
                    </ul>
                </div>
                
                <div class="contact-info">
                    <h3 class="footer-heading">Контакты</h3>
                    <p><i class="fas fa-map-marker-alt"></i> г. Махачкала ул. Рандомная</p>
                    <p><i class="fas fa-phone"></i> +7 (928) 501-57-28</p>
                    <p><i class="fas fa-envelope"></i> mikro9700@mail.ru</p>
                    <p><i class="fas fa-clock"></i> Пн-Пт: 9:00-20:00, Сб: 10:00-18:00</p>
                    <p><i class="fas fa-headset"></i> Техподдержка: поддерживаю@mail.ru</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2026 SMM Nuri. Все права защищены. <a href="#" style="color: rgba(255,255,255,0.8); text-decoration: underline;">Политика конфиденциальности</a> | <a href="#" style="color: rgba(255,255,255,0.8); text-decoration: underline;">Договор оферты</a></p>
            </div>
        </div>
    </footer>

    <script>
        // Мобильное меню
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainMenu = document.getElementById('mainMenu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mainMenu.classList.toggle('active');
            mobileMenuBtn.innerHTML = mainMenu.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Закрытие меню при клике на ссылку
        const menuLinks = document.querySelectorAll('#mainMenu a');
        menuLinks.forEach(link => {
            link.addEventListener('click', () => {
                if(window.innerWidth <= 768) {
                    mainMenu.classList.remove('active');
                    mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                }
            });
        });
        
        // Слайдер отзывов
        const reviews = [
            {
                name: "Анна Козлова",
                position: "SMM-менеджер в AdvertFlow",
                text: "Прошла курс SMM-специалиста с нуля. Уже через 2 месяца после начала обучения получила первые заказы на ведение соцсетей. Сейчас работаю в digital-агентстве. Огромное спасибо преподавателям за практический подход!",
                photo: "https://randomuser.me/api/portraits/women/45.jpg"
            },
            {
                name: "Максим Петров",
                position: "Таргетолог, фрилансер",
                text: "Курс по таргетированной рекламе превзошел все ожидания. Научился не просто настраивать рекламу, а делать это эффективно с минимальным бюджетом. Первый заказчик окупил стоимость курса за неделю.",
                photo: "https://randomuser.me/api/portraits/men/32.jpg"
            },
            {
                name: "Екатерина Смирнова",
                position: "Контент-менеджер в Retail Group",
                text: "Благодаря курсу по контент-маркетингу смогла систематизировать знания и вывести соцсети компании на новый уровень. Вовлеченность выросла в 3 раза за полгода.",
                photo: "https://randomuser.me/api/portraits/women/68.jpg"
            }
        ];
        
        let currentReview = 0;
        const prevBtn = document.getElementById('prevBtn');
        const nextBtn = document.getElementById('nextBtn');
        const reviewSlide = document.querySelector('.review-slide');
        
        function updateReview() {
            const review = reviews[currentReview];
            reviewSlide.innerHTML = `
                <img src="${review.photo}" alt="Выпускник" class="student-photo">
                <p class="review-text">"${review.text}"</p>
                <h4 class="student-name">${review.name}</h4>
                <p class="student-position">${review.position}</p>
            `;
        }
        
        prevBtn.addEventListener('click', () => {
            currentReview = (currentReview - 1 + reviews.length) % reviews.length;
            updateReview();
        });
        
        nextBtn.addEventListener('click', () => {
            currentReview = (currentReview + 1) % reviews.length;
            updateReview();
        });
        
        // Инициализация первого отзыва
        updateReview();
        
        // Обработка формы
        const bookingForm = document.getElementById('bookingForm');
        bookingForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            const name = document.getElementById('name').value;
            const course = document.getElementById('course').options[document.getElementById('course').selectedIndex].text;
            
            // Здесь обычно отправка данных на сервер
            alert(`Спасибо, ${name}! Ваша заявка на курс "${course}" принята. Наш менеджер свяжется с вами в течение 15 минут для уточнения деталей.`);
            
            bookingForm.reset();
        });
        
        // Плавная прокрутка для якорных ссылок
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                e.preventDefault();
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Маска для телефона
        const phoneInput = document.getElementById('phone');
        phoneInput.addEventListener('input', function(e) {
            let value = this.value.replace(/\D/g, '');
            
            if(value.length > 0) {
                value = '+7 (' + value.substring(1, 4) + ') ' + value.substring(4, 7) + '-' + value.substring(7, 9) + '-' + value.substring(9, 11);
            }
            
            this.value = value.substring(0, 18);
        });
        
        // Анимация при прокрутке
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if(entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);
        
        // Наблюдаем за элементами для анимации
        document.querySelectorAll('.course-card, .advantage-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(20px)';
            el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(el);
        });
    </script>
</body>
</html>
