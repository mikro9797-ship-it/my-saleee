<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Code Devil - Dynasty Imperium</title>
    <style>
        /* Основные стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 100%);
            color: #fff;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* Контейнер */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Шапка */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .logo {
            font-size: 28px;
            font-weight: bold;
            background: linear-gradient(45deg, #ff0000, #ff6b6b);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Герой-секция */
        .hero {
            text-align: center;
            padding: 100px 20px;
            position: relative;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            text-shadow: 0 0 30px rgba(255, 0, 0, 0.5);
        }

        .subtitle {
            font-size: 1.5rem;
            color: #aaa;
            margin-bottom: 40px;
        }

        /* Кнопка */
        .cta-button {
            display: inline-block;
            padding: 15px 40px;
            background: linear-gradient(45deg, #ff0000, #8b0000);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: bold;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .cta-button:hover {
            transform: scale(1.05);
            box-shadow: 0 0 30px rgba(255, 0, 0, 0.3);
        }

        /* Особенности */
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 100px 0;
        }

        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 30px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-10px);
            border-color: #ff0000;
        }

        /* Футер */
        footer {
            text-align: center;
            padding: 40px 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            margin-top: 100px;
        }

        /* Адаптивность */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .features {
                grid-template-columns: 1fr;
            }
        }

        /* Анимации */
        @keyframes glow {
            0%, 100% { text-shadow: 0 0 20px rgba(255, 0, 0, 0.5); }
            50% { text-shadow: 0 0 40px rgba(255, 0, 0, 0.8); }
        }

        .glowing-text {
            animation: glow 2s infinite;
        }

        /* Секция кода */
        .code-section {
            background: rgba(0, 0, 0, 0.5);
            padding: 30px;
            border-radius: 10px;
            margin: 50px 0;
            font-family: 'Courier New', monospace;
            border-left: 5px solid #ff0000;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Шапка -->
        <header>
            <div class="logo">DYNASTY IMPERIUM</div>
            <nav>
                <a href="#" style="color: #fff; margin-left: 20px; text-decoration: none;">Главная</a>
                <a href="#" style="color: #aaa; margin-left: 20px; text-decoration: none;">Игра</a>
                <a href="#" style="color: #aaa; margin-left: 20px; text-decoration: none;">Сообщество</a>
            </nav>
        </header>

        <!-- Основной контент -->
        <main>
            <section class="hero">
                <h1 class="glowing-text">CODE <span style="color: #ff0000;">DEVIL</span></h1>
                <p class="subtitle">Раскрой тайны кода. Победи демонов багов.</p>
                <button class="cta-button" id="startGame">НАЧАТЬ ИГРУ</button>
            </section>

            <!-- Особенности -->
            <section class="features">
                <div class="feature-card">
                    <h3>🎮 Игровой процесс</h3>
                    <p>Решай сложные задачи программирования, сражайся с виртуальными демонами багов.</p>
                </div>
                <div class="feature-card">
                    <h3>🏆 Соревнования</h3>
                    <p>Участвуй в турнирах, поднимайся в рейтинге, докажи свое мастерство.</p>
                </div>
                <div class="feature-card">
                    <h3>👥 Сообщество</h3>
                    <p>Присоединяйся к тысячам разработчиков по всему миру.</p>
                </div>
            </section>

            <!-- Пример кода -->
            <section class="code-section">
                <h3>Пример вызова:</h3>
                <pre style="color: #00ff00; margin-top: 20px;">
function solveChallenge() {
    // Твой код здесь
    return "Победа над демоном!";
}</pre>
            </section>
        </main>

        <!-- Футер -->
        <footer>
            <p>© 2024 Dynasty Imperium. Все права защищены.</p>
            <div style="margin-top: 20px;">
                <a href="#" style="color: #aaa; margin: 0 10px;">Условия использования</a>
                <a href="#" style="color: #aaa; margin: 0 10px;">Политика конфиденциальности</a>
                <a href="#" style="color: #aaa; margin: 0 10px;">Контакты</a>
            </div>
        </footer>
    </div>

    <script>
        // Базовый JavaScript для интерактивности
        document.getElementById('startGame').addEventListener('click', function() {
            alert('Игра "Code Devil" запускается! Готовьтесь к вызовам!');
            // Здесь может быть редирект на игру
            // window.location.href = '/game';
        });

        // Эффект печатной машинки для заголовка
        const title = document.querySelector('.hero h1');
        const originalText = title.innerHTML;
        
        // Простой эффект мерцания для кнопки
        setInterval(() => {
            const button = document.querySelector('.cta-button');
            button.style.boxShadow = `0 0 ${20 + Math.random() * 20}px rgba(255, 0, 0, 0.3)`;
        }, 1000);
    </script>
</body>
</html>
