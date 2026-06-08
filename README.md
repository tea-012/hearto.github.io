
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>О мастере — HEARTO</title>

<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link rel="stylesheet" href="сайт/style/adabtive.css">
<style>
/* перья */
.feather {
    position: fixed;
    top: -60px;
    font-size: 20px;
    opacity: 0.3;
    pointer-events: none;
    z-index: 0;
}

.feather img {
    width: 60px;
    height: auto;
    opacity: 0.5;
}

.f1 { left: 8%; animation: fall1 12s linear infinite; }
.f2 { left: 75%; animation: fall2 14s linear infinite; }
.f3 { left: 90%; animation: fall2 16s linear infinite; }

@keyframes fall1 {
    0% { transform: translate(0,0) rotate(0); }
    100% { transform: translate(120px,110vh) rotate(260deg); }
}
@keyframes fall2 {
    0% { transform: translate(0,0) rotate(0); }
    100% { transform: translate(-100px,110vh) rotate(320deg); }
}

/* блок */
.about-master {
    padding: 110px 0 80px;
    overflow-x: hidden;
}

.about-container {
    max-width: 1200px;
    margin: auto;
    padding: 0 40px;
    display: flex;
    gap: 50px;
    align-items: center;
    flex-wrap: wrap;
    justify-content: center;
}

/* ГИФКА — УМЕРЕННЫЙ РАЗМЕР, не больше текстового блока */
.about-gif {
    flex: 0.9;
    min-width: 300px;
    max-width: 380px;
    text-align: center;
}

.about-gif img {
    width: 100%;
    max-width: 100%;
    height: auto;
    border-radius: 28px;
    box-shadow: 0 20px 40px rgba(91,75,255,0.2);
    display: block;
    margin: 0 auto;
    transition: transform 0.3s ease;
}

.about-gif img:hover {
    transform: scale(1.02);
}

/* ТЕКСТ — чуть шире гифки */
.about-text {
    flex: 1.1;
    background: rgba(255,255,255,0.82);
    backdrop-filter: blur(4px);
    border-radius: 36px;
    padding: 35px 40px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.05);
    position: relative;
}

/* декор в углах */
.decor {
    position: absolute;
    font-size: 22px;
    opacity: 0.2;
    pointer-events: none;
}

.decor i {
    background: linear-gradient(135deg,#5B4BFF,#97277A);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.d1 { top: 12px; right: 18px; }
.d2 { bottom: 12px; left: 18px; }

/* заголовок */
.about-text h1 {
    font-size: 36px;
    margin-bottom: 20px;
    color: #1E1B4B;
}

.about-text h1::after {
    content:"";
    display:block;
    width: 65px;
    height: 3px;
    margin-top: 10px;
    background: linear-gradient(90deg,#5B4BFF,#97277A);
    border-radius: 2px;
}

/* текст */
.about-text p {
    font-size: 15.5px;
    line-height: 1.7;
    margin-bottom: 16px;
    color: #2d2a35;
}

/* подпись */
.signature {
    margin-top: 24px;
    font-style: italic;
    color: #97277A;
    border-left: 3px solid #97277A;
    padding-left: 18px;
    font-size: 14.5px;
}

/* заметка */
.small-note {
    margin-top: 20px;
    font-size: 13px;
    color: #8a7aad;
    text-align: center;
    border-top: 1px dashed rgba(151,39,122,0.2);
    padding-top: 14px;
}

.small-note i {
    background: linear-gradient(135deg,#5B4BFF,#97277A);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    margin-right: 6px;
}

/* адаптив */
@media (max-width: 850px) {
    .about-container {
        flex-direction: column;
        gap: 35px;
        padding: 0 25px;
    }
    
    .about-gif {
        max-width: 320px;
        min-width: auto;
    }
    
    .about-text {
        padding: 28px 25px;
        width: 100%;
    }
    
    .about-text h1 {
        text-align: center;
        font-size: 30px;
    }
    
    .about-text h1::after {
        margin-left: auto;
        margin-right: auto;
    }
    
    .about-text p {
        text-align: center;
    }
    
    .signature {
        border-left: none;
        border-top: 2px solid #97277A;
        padding-top: 14px;
        text-align: center;
    }
}

@media (max-width: 550px) {
    .about-container {
        padding: 0 18px;
    }
    
    .about-text {
        padding: 22px 18px;
    }
    
    .about-text h1 {
        font-size: 26px;
    }
    
    .about-text p {
        font-size: 14px;
        line-height: 1.65;
    }
    
    .about-gif {
        max-width: 260px;
    }
}
</style>
</head>

<body>

<!-- перья -->
<div class="feather f1">
    <img src="images/pngwing.com.png" alt="">
</div>

<div class="feather f2">
    <img src="images/pngwing.com.png" alt="">
</div>

<div class="feather f3">
    <img src="images/pngwing.com.png" alt="">
</div>

<!-- ХЕДЕР -->
<header id="header">
    <div class="container header-inner">
        <div class="logo" onclick="location.href='index.html'">HEARTO</div>
        <button class="burger" id="burgerBtn">☰</button>
        <nav>
            <a href="index.html#portfolio">Работы</a>
            <a href="about.html" style="color:#5B4BFF;">О мастере</a>
            <a href="index.html#process">Процесс</a>
            <a href="delivery.html">Доставка</a>
            <a href="order.html" class="btn">Заказать</a>
        </nav>
    </div>
</header>
<div class="menu-overlay" id="menuOverlay"></div>

<!-- ОСНОВА -->
<section class="about-master">
<div class="about-container">

    <!-- ГИФКА — УМЕРЕННЫЙ РАЗМЕР -->
    <div class="about-gif">
        <img src="images/master.gif" alt="Процесс создания">
    </div>

    <!-- ТЕКСТ -->
    <div class="about-text">

        <div class="decor d1"><i class="fas fa-star"></i></div>
        <div class="decor d2"><i class="fas fa-moon"></i></div>

        <h1>Мастерская </h1>

        <p><strong>Дорогие посетители</strong></p>

        <p>
        Вы оказались в небольшой мастерской, которую я открыла совсем недавно.  
        Я только начинаю этот путь, но уже сейчас создаю работы вручную, уделяя внимание форме, деталям и общему ощущению.
        </p>

        <p>
        Пока мастерская только начинает свою историю, каждая работа становится частью этого пути — аккуратного, немного экспериментального и по-своему особенного.
        Я принимаю идеи и эскизы, иногда даже просто образы без точного описания — этого достаточно, чтобы появилась форма.
        </p>

        <p>
        Работы могут немного отличаться, иногда быть неидеальными, но именно это делает их живыми и настоящими.
        </p>

        <p>
        В процессе я соединяю разные материалы и техники, чтобы добиться нужного характера и настроения.
        </p>

        <div class="signature">
             Спасибо, что заглянули<br>
            Здесь всё создаётся вручную
        </div>

        <div class="small-note">
            <i class="fas fa-feather-alt"></i> Имя пока не публикуется — важнее сами игрушки
        </div>

    </div>

</div>
</section>

<!-- ФУТЕР -->
<footer>
    <div class="container">
        <div class="footer-grid">
            <div>
                <h3>HEARTO</h3>
                <p>Авторские игрушки</p>
            </div>
            <div>
                <h4>Навигация</h4>
                <a href="index.html#portfolio">Работы</a>
                <a href="about.html">О мастере</a>
                <a href="index.html#process">Процесс</a>
                <a href="delivery.html">Доставка</a>
                <a href="order.html">Заказать</a>
            </div>
            <div>
                <h4>Документы</h4>
                <a href="privacy.html">Политика конфиденциальности</a>
                <a href="terms.html">Пользовательское соглашение</a>
            </div>
            </div>
        </div>
        <div class="copyright">
            <p>© 2026 HEARTO</p>
        </div>
    </div>
</footer>

<!-- ПОМОЩНИК -->
<div id="assistantOpen" class="assistant-open">💬</div>
<div id="assistant" class="assistant">
<div id="questions" class="assistant-questions"></div>
<div id="message" class="assistant-text"></div>
<div class="assistant-character">
<img id="characterImg" src="images/talk.jfif" alt="Помощник">
</div>
<button id="assistantClose" class="assistant-close">⭐</button>
</div>

<audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>
<script src="script.js"></script>

</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <title>Доставка и возврат — HEARTO</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="style/adabtive.css">
    <style>
        /* Дополнительные стили, сохраняющие цветовую гамму сайта */
        .delivery-hero {
            text-align: center;
            padding: 140px 0 40px;
        }
        .delivery-hero h1 {
            font-size: 42px;
            margin-bottom: 16px;
            color: #1E1B4B;
        }
        .delivery-hero h1::after {
            content: "";
            display: block;
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, #5B4BFF, #C93367);
            margin: 12px auto 0;
            border-radius: 2px;
        }
        .delivery-hero .sub {
            font-size: 16px;
            color: #6b5f7a;
            max-width: 550px;
            margin: 0 auto;
        }

        /* Важный блок об оплате */
        .important-block {
            background: linear-gradient(135deg, #f7f4fc, #faf7ff);
            border-radius: 28px;
            padding: 28px 32px;
            margin: 30px 0 50px;
            border-left: 5px solid #97277A;
            display: flex;
            gap: 20px;
            align-items: flex-start;
            flex-wrap: wrap;
        }
        .important-icon {
            background: rgba(151, 39, 122, 0.1);
            width: 56px;
            height: 56px;
            border-radius: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }
        .important-icon i {
            font-size: 28px;
            color: #97277A;
        }
        .important-text {
            flex: 1;
        }
        .important-text h3 {
            font-size: 20px;
            margin-bottom: 8px;
            color: #1E1B4B;
        }
        .important-text p {
            color: #4a4568;
            margin-bottom: 8px;
            line-height: 1.5;
        }
        .important-text strong {
            color: #C93367;
        }

        /* Карточки доставки */
        .delivery-grid-custom {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 70px;
        }
        .delivery-card-custom {
            background: white;
            border-radius: 24px;
            padding: 32px 24px;
            text-align: center;
            transition: all 0.3s ease;
            box-shadow: 0 8px 24px rgba(0,0,0,0.04);
            border: 1px solid rgba(91, 75, 255, 0.08);
        }
        .delivery-card-custom:hover {
            transform: translateY(-6px);
            box-shadow: 0 20px 35px rgba(91, 75, 255, 0.12);
            border-color: rgba(91, 75, 255, 0.2);
        }
        .delivery-card-custom i {
            font-size: 48px;
            background: linear-gradient(135deg, #5B4BFF, #97277A);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 18px;
            display: inline-block;
        }
        .delivery-card-custom h3 {
            font-size: 22px;
            margin-bottom: 12px;
            color: #1E1B4B;
        }
        .delivery-card-custom p {
            font-size: 14px;
            color: #6b5f7a;
            line-height: 1.5;
        }

        /* Секция возврата */
        .return-wrapper {
            background: #F6F5FF;
            border-radius: 32px;
            padding: 50px 40px;
            margin-bottom: 60px;
        }
        .return-wrapper h2 {
            text-align: center;
            margin-bottom: 35px;
            font-size: 30px;
        }
        .return-wrapper h2::after {
            margin-left: auto;
            margin-right: auto;
        }
        .return-two-columns {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }
        .return-box {
            background: white;
            border-radius: 24px;
            padding: 28px;
            transition: 0.2s;
        }
        .return-box h4 {
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 18px;
            margin-bottom: 20px;
            padding-bottom: 12px;
            border-bottom: 2px solid;
        }
        .return-box.possible h4 {
            color: #5B4BFF;
            border-bottom-color: #5B4BFF;
        }
        .return-box.impossible h4 {
            color: #C93367;
            border-bottom-color: #C93367;
        }
        .return-box ul {
            list-style: none;
            padding: 0;
        }
        .return-box li {
            margin-bottom: 14px;
            padding-left: 28px;
            position: relative;
            color: #4a4568;
            line-height: 1.45;
        }
        .return-box.possible li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: #5B4BFF;
            font-weight: bold;
        }
        .return-box.impossible li::before {
            content: "✗";
            position: absolute;
            left: 0;
            color: #C93367;
            font-weight: bold;
        }
        .return-footer {
            text-align: center;
            margin-top: 35px;
            padding-top: 20px;
            border-top: 1px solid rgba(91, 75, 255, 0.15);
        }
        .return-footer p {
            color: #6b5f7a;
            font-size: 15px;
            line-height: 1.6;
        }
        .return-footer i {
            color: #97277A;
            margin-right: 6px;
        }

        @media (max-width: 768px) {
            .delivery-hero { padding-top: 100px; }
            .delivery-hero h1 { font-size: 32px; }
            .important-block { flex-direction: column; align-items: center; text-align: center; }
            .return-wrapper { padding: 30px 20px; }
            .return-two-columns { grid-template-columns: 1fr; gap: 20px; }
        }
    </style>
</head>
<body>

    <!-- ХЕДЕР -->
    <header id="header">
        <div class="container header-inner">
            <div class="logo" onclick="location.href='index.html'">HEARTO</div>
            <button class="burger" id="burgerBtn">☰</button>
            <nav>
                <a href="index.html#portfolio">Работы</a>
                <a href="about.html">О мастере</a>
                <a href="index.html#process">Процесс</a>
                <a href="delivery.html" style="color: #5B4BFF; font-weight: 500;">Доставка</a>
                <a href="order.html" class="btn">Заказать</a>
            </nav>
        </div>
    </header>
    <div class="menu-overlay" id="menuOverlay"></div>

    <!-- ОСНОВНОЙ КОНТЕНТ -->
    <div class="container">
        
        <!-- Начальный блок -->
        <div class="delivery-hero">
            <h1>Доставка и возврат</h1>
            <p class="sub">Отправляю заказы по всей России. Каждая игрушка доставляется бережно и с трек-номером.</p>
        </div>

        <!-- Блок об оплате доставки -->
        <div class="important-block">
            <div class="important-icon">
                <i class="fas fa-ruble-sign"></i>
            </div>
            <div class="important-text">
                <h3>Доставка оплачивается отдельно</h3>
                <p>Стоимость пересылки <strong>не входит</strong> в цену игрушки и полностью <strong>оплачивается заказчиком</strong>.</p>
                <p>Сумма зависит от вашего города, веса посылки и выбранной службы доставки. Я сообщаю точную стоимость после упаковки заказа. Обычно это <strong>350–700 рублей</strong>.</p>
            </div>
        </div>

        <!-- Службы доставки -->
        <div class="delivery-grid-custom">
            <div class="delivery-card-custom">
                <i class="fas fa-box"></i>
                <h3>СДЭК</h3>
                <p>Доставка до пункта выдачи или курьером на дом. Быстрый трекинг, бережная обработка посылок.</p>
            </div>
            <div class="delivery-card-custom">
                <i class="fas fa-truck"></i>
                <h3>ТК КИТ</h3>
                <p>Надёжная транспортная компания. Хорошо подходит для отправки нескольких игрушек или крупных заказов.</p>
            </div>
            <div class="delivery-card-custom">
                <i class="fas fa-envelope"></i>
                <h3>Почта России</h3>
                <p>Отправляю в любой город России. Посылка приходит с трек-номером, который можно отследить.</p>
            </div>
        </div>

        <!-- ВОЗВРАТ -->
        <div class="return-wrapper">
            <h2>Условия возврата</h2>
            <div class="return-two-columns">
                <div class="return-box possible">
                    <h4><i class="fas fa-check-circle"></i> Когда можно вернуть</h4>
                    <ul>
                        <li>Игрушка повреждена при пересылке (нужно фото упаковки)</li>
                        <li>Обнаружен брак: отклеилась деталь, трещина, скол</li>
                        <li>Размер отличается от заявленного больше чем на 1 см</li>
                        <li>Вы обратились <strong>в течение 7 дней</strong> после получения</li>
                    </ul>
                </div>
                <div class="return-box impossible">
                    <h4><i class="fas fa-times-circle"></i> Когда вернуть нельзя</h4>
                    <ul>
                        <li>Прошло больше 7 дней с момента получения</li>
                        <li>Игрушка уже использовалась или повреждена вами</li>
                        <li>Вам не понравился оттенок или лёгкая асимметрия (это особенности ручной работы)</li>
                        <li>Товар качественный, но вы просто передумали</li>
                    </ul>
                </div>
            </div>
            <div class="return-footer">
                <p><i class="fas fa-comment-dots"></i> <strong>Как оформить возврат:</strong> Напишите мне на почту в течение 7 дней после получения посылки. Приложите фото брака и фото упаковки. Я отвечу в течение двух дней. Если брак подтвердится — я дам скидку, сделаю новую игрушку или верну деньги за неё (стоимость доставки не возвращается).</p>
                <p style="margin-top: 12px;"><i class="fas fa-camera"></i> Перед отправкой я всегда фотографирую готовую игрушку и согласовываю с вами. Это помогает избежать споров о внешнем виде.</p>
            </div>
        </div>
    </div>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div><h3>HEARTO</h3><p>Авторские игрушки</p></div>
                <div>
                    <h4>Навигация</h4>
                    <a href="index.html#portfolio">Работы</a>
                    <a href="about.html">О мастере</a>
                    <a href="index.html#process">Процесс</a>
                    <a href="delivery.html">Доставка</a>
                    <a href="order.html">Заказать</a>
                </div>
                <div>
                    <h4>Документы</h4>
                    <a href="privacy.html">Политика конфиденциальности</a>
                    <a href="terms.html">Пользовательское соглашение</a>
                </div>
                </div>
            </div>
            <div class="copyright"><p>© 2026 HEARTO</p></div>
        </div>
    </footer>

    <!-- Помощник -->
    <div id="assistantOpen" class="assistant-open">💬</div>
    <div id="assistant" class="assistant">
        <div id="questions" class="assistant-questions"></div>
        <div id="message" class="assistant-text"></div>
        <div class="assistant-character">
            <img id="characterImg" src="images/talk.jfif" alt="Помощник">
        </div>
        <button id="assistantClose" class="assistant-close">⭐</button>
    </div>

    <audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>
    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<title>HEARTO — авторские игрушки</title>
<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="style/adabtive.css">
</head>
<body>

<!-- HEADER -->
<header id="header">
<div class="container header-inner">
<div class="logo" onclick="location.href='index.html'">Мастерская</div>
<button class="burger" id="burgerBtn">☰</button>
<nav>
<a href="#portfolio">Работы</a>
<a href="about.html">О мастере</a>
<a href="#process">Процесс</a>
<a href="delivery.html">Доставка</a>
<a href="order.html" class="btn">Заказать</a>
</nav>
</div>
</header>

<!-- HERO -->
<section class="hero">
<div class="container hero-inner">
<div class="hero-text">
<h1>Авторские игрушки<br>в смешанных техниках</h1>
<p class="hero-sub">Глина. Шерсть. Характер.<br>Каждая — единственная.</p>
<a href="#portfolio" class="btn">Смотреть работы</a>
</div>
</div>
</section>

<!-- ПРОЦЕСС СОЗДАНИЯ -->
<section id="process" class="fade">
  <div class="container">
    <h2>Процесс создания</h2>
    <div class="process-thread-wrap">
    <div class="process-grid">
      
      <div class="step-card">
        <div class="icon"><i class="fas fa-lightbulb"></i></div>
        <h3>Идея</h3>
        <p>Ты описываешь, что хочешь — я предлагаю концепт</p>
      </div>

      <div class="step-card">
        <div class="icon"><i class="fas fa-pencil-alt"></i></div>
        <h3>Эскиз</h3>
        <p>Создаю набросок и согласовываю все детали</p>
      </div>

      <div class="step-card">
        <div class="icon"><i class="fas fa-hands"></i></div>
        <h3>Создание</h3>
        <p>Шью или леплю вручную с любовью к деталям</p>
      </div>

      <div class="step-card">
        <div class="icon"><i class="fas fa-box-open"></i></div>
        <h3>Отправка</h3>
        <p>Аккуратно упаковываю и отправляю вам</p>
      </div>

    </div>
    </div>
  </div>
</section>

<!-- ПРИМЕРЫ РАБОТ -->
<section id="portfolio" class="fade">
  <div class="container">
    <h2>Примеры работ</h2>
    <div class="grid">
      <div class="card">
        <img src="images/rabota/679.png" alt="Осьминожка">
        <div class="card-info">
          <h4>Осьминожка</h4>
          <p>глина, акрил. Подобного формата малыши стоят от...</p>
          <div class="card-price">200 ₽</div>
        </div>
      </div>
      <div class="card">
        <img src="images/rabota/rab1.jpg" alt="Лягушка">
        <div class="card-info">
          <h4>Лягушка</h4>
          <p>глина, акрил. Стоит подобный...</p>
          <div class="card-price">300 ₽</div>
        </div>
      </div>
      <div class="card">
        <img src="images/rabota/corova.png" alt="Коровка">
        <div class="card-info">
          <h4>Коровка</h4>
          <p>глина, шерсть, акрил. Подобный формат стоит...</p>
          <div class="card-price">850 ₽</div>
        </div>
      </div>
      <!-- Дополнительные работы -->
      <div class="card extra-work" style="display: none;">
        <img src="images/extra1.jpg" alt="Доп. работа">
        <div class="card-info">
          <h4>В процессе</h4>
          <p>В процессе</p>
          <div class="card-price"></div>
        </div>
      </div>
      <div class="card extra-work" style="display: none;">
        <img src="images/extra2.jpg" alt="Доп. работа">
        <div class="card-info">
          <h4>В процессе</h4>
          <p>В процессе</p>
          <div class="card-price"></div>
        </div>
      </div>
    </div>
    <div class="portfolio-footer">
      <button id="toggleExtraBtn" class="btn-toggle">Показать ещё работы</button>
    </div>
  </div>
</section>

<!-- ===== АВТОРСКИЙ МЕРЧ ===== -->
<section id="merch">
  <div class="container">
    <div class="merch-content">
      <h2>Авторский мерч</h2>
      <p>Брелки, наклейки, значки и так далее. Что-то из этих предметов пойдёт в подарок к вашему мягкому или не очень другу. В будущем планируется расшириться, и можно будет заказывать у меня подобные вещички отдельно.</p>
    </div>
    
    <!-- CSS-декорации -->
    <div class="merch-decorations">
      <div class="css-planet planet-main parallax-item" data-speed="15">
        <div class="planet-ring"></div>
      </div>
      <div class="css-planet planet-pink parallax-item" data-speed="8"></div>
      <div class="css-star star-yellow parallax-item" data-speed="12"></div>
      <div class="css-star star-small parallax-item" data-speed="6"></div>
      <div class="css-star star-tiny parallax-item" data-speed="9"></div>
    </div>
  </div>
</section>

<!-- ПОМОЩНИК -->
<div id="assistantOpen" class="assistant-open">💬</div>
<div id="assistant" class="assistant">
<div id="questions" class="assistant-questions"></div>
<div id="message" class="assistant-text"></div>
<div class="assistant-character">
<img id="characterImg" src="images/talk.png" alt="Помощник">
</div>
<button id="assistantClose" class="assistant-close">⭐</button>
</div>

<!-- FOOTER -->
<footer>
<div class="container">
<div class="footer-grid">
<div><h3>HEARTO</h3><p>Авторские игрушки</p></div>
<div>
<h4>Навигация</h4>
<a href="#portfolio">Работы</a>
<a href="about.html">О мастере</a>
<a href="#process">Процесс</a>
<a href="delivery.html">Доставка</a>
<a href="order.html">Заказать</a>
</div>
<div>
    <h4>Документы</h4>
    <a href="privacy.html">Политика конфиденциальности</a>
    <a href="terms.html">Пользовательское соглашение</a>
</div>
<div>
</div>
</div>
</div>
<div class="copyright"><p>© 2026 HEARTO</p></div>
</div>
</footer>

<!-- МОДАЛКА -->
<div id="workModal" class="modal-overlay">
<div class="modal-box">
<button class="modal-close">&times;</button>
<img class="modal-img" src="" alt="">
<div class="modal-info">
<h3 class="modal-title"></h3>
<p class="modal-desc"></p>
</div>
</div>
</div>

<div class="menu-overlay" id="menuOverlay"></div>
<audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>
<script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<title>HEARTO — Заказать фигурку</title>
<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="style/adabtive.css">
<style>
:root {
    --blue-main: #5B4BFF;
    --blue-light: #8A7CFF;
    --purple-text: #4A3D8F;
    --purple-dark: #3A2D7A;
    --raspberry: #97277A;
    --raspberry-bright: #C93367;
    --hint-text: #7B70B0;
    --card-bg: rgba(255, 255, 255, 0.55);
    --card-border: rgba(91, 75, 255, 0.2);
    
    /* ===== ЦВЕТ ГРАНИЦ ПОЛЕЙ ===== */
    --input-border: #878cd4;
    --input-focus: #B4356C;
    --input-focus-ring: rgba(180, 53, 108, 0.18);
}

/* ===== ФОНОВАЯ СЕКЦИЯ + ПЛАВНЫЙ ПЕРЕХОД К ФУТЕРУ ===== */
.order-page {
    position: relative;
    z-index: 1;
    min-height: 100vh;
    /* Градиент плавно темнеет внизу для органичного слияния с футером */
    background: linear-gradient(
        180deg,
        #EEEDFF 0%,
        #d2cdf7 25%,
        #b7aceb 50%,
        #afa0eb 70%,
        #9386d6 82%,
        #62538b 100%
    );
    padding-top: 80px;
    padding-bottom: 60px;
    overflow: hidden;
}

/* Если у вас футер конкретного цвета, замените #7B68AE в градиенте на него */

/* ===== ЗВЁЗДЫ ===== */
.stars-bg {
    position: absolute;
    inset: 0;
    z-index: 0;
    pointer-events: none;
    overflow: hidden;
}

.star {
    position: absolute;
    border-radius: 50%;
    background: #ffffff;
    box-shadow: 0 0 6px rgba(255, 255, 255, 0.9), 0 0 12px rgba(138, 124, 255, 0.5);
    animation: twinkle var(--dur) ease-in-out infinite var(--del);
}

@keyframes twinkle {
    0%, 100% { opacity: 0.25; transform: scale(0.8); }
    50% { opacity: 1; transform: scale(1.15); }
}

.order-container {
    position: relative;
    z-index: 2;
    max-width: 520px;
    margin: 0 auto;
    padding: 0 16px;
}

.order-info {
    background: var(--card-bg);
    backdrop-filter: blur(12px);
    border-radius: 20px;
    padding: 24px 20px;
    margin-bottom: 20px;
    border: 1px solid var(--card-border);
}

.order-info__title {
    font-size: 20px;
    font-weight: 700;
    color: var(--purple-dark);
    margin-bottom: 14px;
    text-align: center;
    line-height: 1.3;
}

.order-info__title span {
    display: block;
    font-size: 16px;
    color: var(--blue-main);
    font-weight: 600;
    margin-top: 4px;
}

.order-info__text {
    font-size: 13px;
    color: var(--purple-text);
    line-height: 1.65;
    margin-bottom: 14px;
}

.order-info__hint {
    font-size: 13px;
    font-weight: 600;
    color: var(--blue-main);
    line-height: 1.5;
    margin-top: 0;
}

.order-form-card {
    background: var(--card-bg);
    backdrop-filter: blur(12px);
    border-radius: 20px;
    padding: 24px 20px;
    margin-bottom: 20px;
    border: 1px solid var(--card-border);
}

.form-group { margin-bottom: 14px; }

.form-group label {
    display: block;
    font-size: 13px;
    font-weight: 700;
    color: var(--purple-dark);
    margin-bottom: 6px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 12px 16px;
    border: 2px solid var(--input-border); /* #B4356C */
    border-radius: 14px;
    background: rgba(255, 255, 255, 0.7);
    font-size: 14px;
    color: var(--purple-dark);
    font-family: inherit;
    outline: none;
    transition: border-color 0.3s, box-shadow 0.3s, background 0.3s;
    box-sizing: border-box;
}

.form-group input::placeholder,
.form-group textarea::placeholder {
    color: #AFA4E0;
    font-size: 13px;
}

.form-group input:focus,
.form-group textarea:focus {
    border-color: var(--input-focus);
    box-shadow: 0 0 0 3px var(--input-focus-ring);
    background: rgba(255, 255, 255, 0.9);
}

.form-group textarea { min-height: 140px; resize: vertical; }

.form-group .hint {
    font-size: 11.5px;
    color: var(--hint-text);
    margin-top: 4px;
    padding-left: 2px;
    font-style: italic;
}

.form-group label .req { color: var(--raspberry); font-size: 14px; }

.contact-note {
    background: rgba(91, 75, 255, 0.08);
    border: 1px dashed rgba(91, 75, 255, 0.35);
    border-radius: 12px;
    padding: 12px 14px;
    margin-bottom: 18px;
    font-size: 12.5px;
    color: var(--purple-text);
    line-height: 1.5;
}

.contact-note i { margin-right: 6px; color: var(--raspberry); }
.contact-note strong { color: var(--raspberry); }

.file-upload-area { margin-bottom: 14px; }
.file-upload-area > label {
    display: block;
    font-size: 13px;
    font-weight: 700;
    color: var(--purple-dark);
    margin-bottom: 6px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
}

.file-drop-zone {
    border: 2px dashed var(--input-border);
    border-radius: 14px;
    padding: 28px 16px;
    text-align: center;
    transition: border-color 0.3s, background 0.3s;
    background: rgba(255, 255, 255, 0.4);
    position: relative;
    user-select: none;
    -webkit-user-select: none;
}

.file-drop-zone:hover {
    border-color: var(--input-focus);
    background: rgba(180, 53, 108, 0.06);
}

.file-drop-zone.dragover {
    border-color: var(--input-focus);
    background: rgba(180, 53, 108, 0.1);
    border-style: solid;
}

.file-drop-zone__icon {
    font-size: 28px;
    margin-bottom: 8px;
    pointer-events: none;
}

.file-drop-zone__text {
    font-size: 13px;
    color: var(--hint-text);
    line-height: 1.5;
    pointer-events: none;
}

.file-drop-zone__text strong {
    color: var(--input-focus);
    text-decoration: underline;
    text-underline-offset: 3px;
}

.file-drop-zone input[type="file"] { display: none; }
.file-drop-zone__clickable { cursor: pointer; display: block; }

.file-preview-list {
    margin-top: 10px;
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
}

.file-preview-item {
    position: relative;
    width: 70px;
    height: 70px;
    border-radius: 10px;
    overflow: hidden;
    border: 2px solid var(--input-border);
    -webkit-user-drag: none;
    user-select: none;
    -webkit-user-select: none;
}

.file-preview-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    pointer-events: none;
    -webkit-user-drag: none;
}

.file-preview-item__remove {
    position: absolute;
    top: 2px;
    right: 2px;
    width: 20px;
    height: 20px;
    background: var(--raspberry);
    color: #fff;
    border: none;
    border-radius: 50%;
    font-size: 11px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    line-height: 1;
    z-index: 2;
}

.btn-submit {
    width: 100%;
    padding: 16px;
    background: linear-gradient(135deg, #97277A, #C93367);
    color: #fff;
    border: none;
    border-radius: 14px;
    font-size: 16px;
    font-weight: 700;
    font-family: inherit;
    cursor: pointer;
    letter-spacing: 1px;
    text-transform: uppercase;
    transition: transform 0.2s, box-shadow 0.2s, opacity 0.2s;
    box-shadow: 0 4px 20px rgba(151, 39, 122, 0.3);
    margin-bottom: 20px;
}

.btn-submit:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 28px rgba(151, 39, 122, 0.4);
}
.btn-submit:active { transform: translateY(0); }
.btn-submit:disabled { opacity: 0.6; cursor: not-allowed; transform: none; }

.example-card {
    background: var(--card-bg);
    backdrop-filter: blur(12px);
    border-radius: 20px;
    padding: 24px 20px;
    border: 1px solid var(--card-border);
    margin-bottom: 40px;
}

.example-card__title {
    font-size: 14px;
    font-weight: 700;
    color: var(--purple-dark);
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 14px;
    text-align: center;
}

.example-card__text {
    font-size: 13px;
    color: var(--purple-text);
    line-height: 1.7;
    white-space: pre-line;
}

.success-message {
    display: none;
    text-align: center;
    padding: 40px 20px;
}
.success-message.show { display: block; }
.success-message__icon { font-size: 48px; margin-bottom: 16px; }
.success-message__title { font-size: 20px; font-weight: 700; color: var(--purple-dark); margin-bottom: 10px; }
.success-message__text { font-size: 14px; color: var(--blue-main); line-height: 1.6; }

@media (max-width: 480px) {
    .order-info, .order-form-card, .example-card { padding: 20px 16px; border-radius: 16px; }
    .order-info__title { font-size: 18px; }
    .form-group input, .form-group textarea { padding: 11px 14px; font-size: 13px; }
}
</style>
</head>
<body>

<!-- HEADER -->
<header id="header">
<div class="container header-inner">
<div class="logo" onclick="location.href='index.html'">HEARTO</div>
<button class="burger" id="burgerBtn">☰</button>
<nav>
<a href="index.html#portfolio">Работы</a>
<a href="about.html">О мастере</a>
<a href="index.html#process">Процесс</a>
<a href="delivery.html">Доставка</a>
<a href="order.html" class="btn">Заказать</a>
</nav>
</div>
</header>

<!-- ORDER PAGE -->
<section class="order-page">
    <div class="stars-bg" id="starsBg"></div>

    <div class="order-container">
        <div class="order-info">
            <div class="order-info__title">
                Заявка на изготовление фигурки
                <span>Как оформить заявку?</span>
            </div>
            <p class="order-info__text">
                Опишите свою идею подробно: примерный размер, цвета, стиль, материалы и
                особенности фигурки. Прикрепите фото или рисунки, которые помогут
                точнее понять ваши пожелания.
            </p>
            <p class="order-info__hint">
                Ваши личные данные — чтобы я могла с вами связаться 💌
            </p>
        </div>

        <div class="order-form-card" id="orderFormCard">
<form action="https://formspree.io/f/mjgzwoaw" method="POST" enctype="multipart/form-data">
    <!-- Скрытые поля для настройки -->
    <input type="hidden" name="_subject" value="Новый заказ HEARTO!">
    <input type="hidden" name="_captcha" value="false">
    <input type="hidden" name="_template" value="table">
                <div class="contact-note">
                    <i class="fas fa-info-circle"></i>
                    <strong>Обязательно:</strong> заполните <u>описание заказа</u> и хотя бы один способ связи — <strong>почту</strong> или <strong>вконтакте</strong>. Остальное — на ваше усмотрение.
                </div>

                <div class="form-group">
                    <label>Почта <span class="req">*</span></label>
                    <input type="email" id="email"  name="email" placeholder="example@mail.ru" autocomplete="email">
                    <div class="hint">* или заполните Месседжер</div>
                </div>

                <div class="form-group">
                    <label>Месседжер<span class="req">*</span></label>
                    <input type="text" id="telegram" name="telegram" placeholder="@username" autocomplete="username">
                    <div class="hint">* или заполните Почту</div>
                </div>

                <div class="form-group">
                    <label>ФИО</label>
                    <input type="text" id="fio" name="name" placeholder="Иванова Иван Иванович" autocomplete="name">
                    <div class="hint">можно не заполнять</div>
                </div>

                <div class="form-group">
                    <label>Адрес доставки</label>
                    <input type="text" id="address" name="address" placeholder="Город, индекс, адрес" autocomplete="street-address">
                    <div class="hint">можно не заполнять — обсудим лично</div>
                </div>

                <div class="form-group">
                    <label>Телефон</label>
                    <input type="tel" id="phone" name="phone" placeholder="+7 (___) ___-__-__" autocomplete="tel">
                    <div class="hint">можно не заполнять</div>
                </div>

                <div class="form-group">
                    <label>Описание заказа <span class="req">*</span></label>
                    <textarea id="description" name="description" placeholder="Опишите вашу идею: размер, цвета, стиль, материалы, особенности фигурки..." required></textarea>
                    <div class="hint">самое важное поле — опишите максимально подробно</div>
                </div>

                <div class="file-upload-area">
                    <label>Прикрепить референсы</label>
                    <div class="file-drop-zone" id="fileDropZone">
                        <div class="file-drop-zone__clickable" id="fileClickTrigger">
                            <div class="file-drop-zone__icon">📎</div>
                            <div class="file-drop-zone__text">
                                <strong>Нажмите для загрузки</strong> или перетащите файлы сюда<br>
                                <small style="color:#AFA4E0;">Фото, рисунки — jpg, png, pdf</small>
                            </div>
                        </div>
                    </div>
                   <input type="file" id="fileInput" name="file" multiple accept="image/*,.pdf" 
       style="position:absolute; opacity:0; width:0; height:0; pointer-events:none;">
                    <div class="file-preview-list" id="filePreviewList"></div>
                </div>

                <button type="submit" class="btn-submit" id="submitBtn">
                    <span id="submitText">Отправить</span>
                </button>
            </form>

            <div class="success-message" id="successMessage">
                <div class="success-message__icon">🎉</div>
                <div class="success-message__title">Заявка отправлена!</div>
                <div class="success-message__text">
                    Спасибо! Я свяжусь с вами в ближайшее время<br>
                    для обсуждения деталей ✨
                </div>
            </div>
        </div>

        <div class="example-card">
            <div class="example-card__title">Примеры описаний</div>
            <div class="example-card__text">
• Маленькая фигурка котика. 10 см в высоту. Белый, с милой улыбкой и закрытыми глазами.

• Мой персонаж, хочется чиби версию. У нее яркие волосы зеленого цвета, поза стоит на ногах. Руки держит по бокам, самоуверенная улыбка. Рассчитываю на сумму 700 рублей.
            </div>
        </div>
    </div>
</section>

<!-- ПОМОЩНИК -->
<div id="assistantOpen" class="assistant-open">💬</div>
<div id="assistant" class="assistant">
    <div id="questions" class="assistant-questions"></div>
    <div id="message" class="assistant-text"></div>
    <div class="assistant-character">
        <img id="characterImg" src="images/talk.jfif" alt="Помощник">
    </div>
    <button id="assistantClose" class="assistant-close">⭐</button>
</div>

<!-- FOOTER -->
<footer>
<div class="container">
<div class="footer-grid">
<div><h3>HEARTO</h3><p>Авторские игрушки</p></div>
<div>
<h4>Навигация</h4>
<a href="index.html#portfolio">Работы</a>
<a href="about.html">О мастере</a>
<a href="index.html#process">Процесс</a>
<a href="delivery.html">Доставка</a>
<a href="order.html">Заказать</a>
</div>
<div>
    <h4>Документы</h4>
    <a href="privacy.html">Политика конфиденциальности</a>
    <a href="terms.html">Пользовательское соглашение</a>
</div>
</div>
</div>
<div class="copyright"><p>© 2026 HEARTO</p></div>
</div>
</footer>

<div class="menu-overlay" id="menuOverlay"></div>
<audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>

<script src="script.js"></script>
<script>
// ===== ГЕНЕРАЦИЯ ЗВЁЗД =====
(function createStars() {
    const container = document.getElementById('starsBg');
    if (!container) return;
    const count = 80;
    for (let i = 0; i < count; i++) {
        const star = document.createElement('div');
        star.className = 'star';
        const size = Math.random() * 3 + 2;
        star.style.width = size + 'px';
        star.style.height = size + 'px';
        star.style.top = Math.random() * 100 + '%';
        star.style.left = Math.random() * 100 + '%';
        star.style.setProperty('--dur', (Math.random() * 4 + 2.5) + 's');
        star.style.setProperty('--del', (Math.random() * 6) + 's');
        container.appendChild(star);
    }
})();


/* =========================
FORMSUBMIT + ПРЕВЬЮ ФАЙЛОВ (FIXED)
========================= */
document.addEventListener('DOMContentLoaded', () => {
    const orderForm = document.getElementById('orderForm');
    const fileInput = document.getElementById('fileInput');
    const dropZone = document.getElementById('fileDropZone');
    const trigger = document.getElementById('fileClickTrigger');
    const previewList = document.getElementById('filePreviewList');
    const submitBtn = document.getElementById('submitBtn');
    const successMessage = document.getElementById('successMessage');

    // Массив для хранения выбранных файлов (чтобы можно было удалять по одному)
    let selectedFiles = [];

    // 1. Клик по зоне -> открываем выбор
    if (trigger && fileInput) {
        trigger.addEventListener('click', (e) => { 
            e.preventDefault(); 
            fileInput.click(); 
        });
    }

    // 2. Обработка выбора файлов через диалоговое окно
    if (fileInput) {
        fileInput.addEventListener('change', () => {
            addFiles(Array.from(fileInput.files));
            fileInput.value = ''; // Очищаем инпут, чтобы можно было выбрать тот же файл снова
        });
    }

    // 3. Drag & Drop логика
    if (dropZone) {
        ['dragenter', 'dragover', 'dragleave', 'drop'].forEach(evt => {
            dropZone.addEventListener(evt, (e) => { e.preventDefault(); e.stopPropagation(); });
        });
        
        dropZone.addEventListener('dragover', () => dropZone.classList.add('drag-active'));
        dropZone.addEventListener('dragleave', () => dropZone.classList.remove('drag-active'));
        
        dropZone.addEventListener('drop', (e) => {
            dropZone.classList.remove('drag-active');
            const files = e.dataTransfer.files;
            if (files.length) addFiles(Array.from(files));
        });
    }

    // Функция добавления файлов в массив
    function addFiles(newFiles) {
        newFiles.forEach(file => {
            // Проверка на дубликаты
            if (!selectedFiles.some(f => f.name === file.name && f.size === file.size)) {
                selectedFiles.push(file);
            }
        });
        renderPreviews();
    }

    // Функция отрисовки превью
    function renderPreviews() {
        if (!previewList) return;
        previewList.innerHTML = '';
        
        selectedFiles.forEach((file, index) => {
            const item = document.createElement('div');
            item.className = 'file-preview-item';

            if (file.type.startsWith('image/')) {
                const img = document.createElement('img');
                const reader = new FileReader();
                reader.onload = e => { img.src = e.target.result; };
                reader.readAsDataURL(file);
                item.appendChild(img);
            } else {
                // Иконка для не-картинок
                item.style.display = 'flex';
                item.style.alignItems = 'center';
                item.style.justifyContent = 'center';
                item.style.background = '#EEEDFF';
                item.style.fontSize = '24px';
                item.textContent = '📄';
            }

            // Кнопка удаления
            const removeBtn = document.createElement('button');
            removeBtn.type = 'button';
            removeBtn.className = 'file-preview-item__remove';
            removeBtn.innerHTML = '✕';
            removeBtn.addEventListener('click', (e) => {
                e.stopPropagation();
                selectedFiles.splice(index, 1); // Удаляем из массива
                renderPreviews(); // Перерисовываем
            });
            
            item.appendChild(removeBtn);
            previewList.appendChild(item);
        });
    }

    // 4. Отправка формы через Fetch (чтобы не перезагружать страницу)
    if (orderForm) {
        orderForm.addEventListener('submit', async (e) => {
            e.preventDefault();
            
            // Простая валидация перед отправкой
            const email = document.getElementById('email').value.trim();
            const desc = document.getElementById('description').value.trim();
            
            if (!email || !desc) {
                alert('Пожалуйста, заполните Email и Описание заказа ✨');
                return;
            }

            const originalBtnText = submitBtn.innerHTML;
            submitBtn.disabled = true;
            submitBtn.innerHTML = 'Отправляю... ⏳';

            // Создаем FormData
            const formData = new FormData(orderForm);
            
            // ВАЖНО: FormSubmit ожидает файлы в поле с именем "attachment" (как в HTML)
            // Но так как мы используем свой массив selectedFiles, нам нужно добавить их вручную
            // Сначала очищаем поле attachment в formData, если там что-то осталось
            formData.delete('attachment');
            
            selectedFiles.forEach(file => {
                formData.append('attachment', file);
            });

            try {
                const response = await fetch(orderForm.action, {
                    method: 'POST',
                    body: formData,
                    headers: { 'Accept': 'application/json' }
                });

                if (response.ok) {
                    orderForm.style.display = 'none';
                    if (successMessage) successMessage.style.display = 'block';
                    // Очистка
                    selectedFiles = [];
                    renderPreviews();
                } else {
                    alert('Ошибка при отправке. Попробуйте позже.');
                }
            } catch (err) {
                console.error(err);
                alert('Ошибка сети. Проверьте подключение.');
            } finally {
                submitBtn.disabled = false;
                submitBtn.innerHTML = originalBtnText;
            }
        });
    }
});


</script>
</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <title>Политика конфиденциальности — HEARTO</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="style/adabtive.css">
    <style>
        /* Дополнительные стили для страницы политики */
        .policy-hero {
            text-align: center;
            padding: 140px 20px 40px;
        }
        .policy-hero h1 {
            font-size: 42px;
            margin-bottom: 16px;
            color: #1E1B4B;
            word-break: break-word;
            hyphens: auto;
        }
        .policy-hero h1::after {
            content: "";
            display: block;
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, #5B4BFF, #781C4F);
            margin: 12px auto 0;
            border-radius: 2px;
        }
        .policy-hero .sub {
            font-size: 16px;
            color: #6b5f7a;
            max-width: 600px;
            margin: 0 auto;
            word-break: break-word;
        }

        /* Основной контент политики */
        .policy-content {
            max-width: 900px;
            margin: 0 auto 80px;
            background: white;
            border-radius: 32px;
            padding: 50px 60px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.04);
            overflow-x: hidden;
            word-wrap: break-word;
        }
        .policy-content h2 {
            font-size: 26px;
            margin: 30px 0 15px;
            color: #1E1B4B;
            word-break: break-word;
        }
        .policy-content h2:first-of-type {
            margin-top: 0;
        }
        .policy-content h2::after {
            display: none;
        }
        .policy-content h3 {
            font-size: 20px;
            margin: 25px 0 12px;
            color: #781C4F;
            word-break: break-word;
        }
        .policy-content p {
            color: #4a4568;
            line-height: 1.7;
            margin-bottom: 16px;
            font-size: 15px;
            word-break: break-word;
        }
        .policy-content ul {
            margin: 15px 0 20px;
            padding-left: 25px;
        }
        .policy-content li {
            color: #4a4568;
            margin-bottom: 10px;
            line-height: 1.6;
            word-break: break-word;
        }
        .policy-content strong {
            color: #781C4F;
        }
        .policy-date {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #e0d6f0;
            font-size: 14px;
            color: #8a7aad;
            text-align: center;
        }
        .policy-contact {
            background: #F6F5FF;
            border-radius: 20px;
            padding: 20px 28px;
            margin-top: 35px;
            text-align: center;
        }
        .policy-contact p {
            margin-bottom: 8px;
            word-break: break-word;
        }
        .policy-contact a {
            color: #781C4F;
            text-decoration: none;
            font-weight: 500;
            word-break: break-all;
        }
        .policy-contact a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .policy-hero { 
                padding-top: 100px; 
                padding-left: 16px;
                padding-right: 16px;
            }
            .policy-hero h1 { 
                font-size: 28px; 
                line-height: 1.3;
            }
            .policy-content { 
                padding: 28px 20px; 
                margin-left: 16px;
                margin-right: 16px;
                width: calc(100% - 32px);
                box-sizing: border-box;
            }
            .policy-content h2 { 
                font-size: 22px; 
            }
            .policy-content h3 { 
                font-size: 18px; 
            }
            .policy-content ul {
                padding-left: 20px;
            }
        }

        @media (max-width: 480px) {
            .policy-content {
                padding: 22px 16px;
            }
            .policy-content h2 {
                font-size: 20px;
            }
            .policy-contact {
                padding: 16px;
            }
        }

        /* Переопределение цветов футера */
        footer {
            background: #681844;
        }
        footer .footer-grid h3,
        footer .footer-grid h4,
        footer .footer-grid a,
        footer .copyright p {
            color: #ffffff;
        }
        footer .footer-grid a:hover {
            color: #1E1B4B;
        }
        footer .copyright {
            border-top-color: rgba(120, 28, 79, 0.15);
        }
        .social-icons a {
            color: #1E1B4B;
        }
        .social-icons a:hover {
            color: #781C4F;
        }
    </style>
</head>
<body>

    <!-- ХЕДЕР -->
    <header id="header">
        <div class="container header-inner">
            <div class="logo" onclick="location.href='index.html'">HEARTO</div>
            <button class="burger" id="burgerBtn">☰</button>
            <nav>
                <a href="index.html#portfolio">Работы</a>
                <a href="about.html">О мастере</a>
                <a href="index.html#process">Процесс</a>
                <a href="delivery.html">Доставка</a>
                <a href="order.html" class="btn">Заказать</a>
            </nav>
        </div>
    </header>
    <div class="menu-overlay" id="menuOverlay"></div>

    <!-- ОСНОВНОЙ КОНТЕНТ -->
    <div class="container" style="width: 100%; padding-left: 0; padding-right: 0;">
        <div class="policy-hero">
            <h1>Политика конфиденциальности</h1>
        </div>

        <div class="policy-content">
            <h2>1. Общие положения</h2>
            <p>Настоящая Политика конфиденциальности определяет порядок обработки и защиты персональных данных пользователей интернет-магазина авторских игрушек HEARTO (далее — «Сайт»).</p>
            <p>Я, как владелец Сайта, уважаю ваше право на конфиденциальность и обязуюсь защищать любую информацию, которую вы предоставляете при оформлении заказа или общении со мной.</p>

            <h2>2. Какие данные собираются</h2>
            <p>При оформлении заказа или связи со мной через формы обратной связи, мессенджеры или электронную почту могут собираться следующие данные:</p>
            <ul>
                <li>Ваше имя (или псевдоним);</li>
                <li>Адрес электронной почты;</li>
                <li>Данные, необходимые для отправки заказа через службы доставки (СДЭК, ТК КИТ, Почта России).</li>
            </ul>

            <h2>3. Цели сбора данных</h2>
            <p>Ваши персональные данные используются исключительно для:</p>
            <ul>
                <li>Обработки и оформления вашего заказа;</li>
                <li>Связи с вами для уточнения деталей заказа, доставки или возврата;</li>
                <li>Отправки готовой игрушки по указанному адресу;</li>
                <li>Информирования о статусе заказа и его отправке.</li>
            </ul>
            <p><strong>Важно:</strong> Я НЕ передаю ваши данные третьим лицам, кроме случаев, предусмотренных законодательством РФ или когда это необходимо для работы служб доставки (им передаётся только адрес и контактный телефон).</p>

            <h2>4. Хранение и защита данных</h2>
            <p>Я принимаю все необходимые меры для защиты ваших данных от несанкционированного доступа, изменения, раскрытия или уничтожения. Все данные хранятся на защищённых устройствах и не передаются посторонним.</p>
            <p>Личная переписка (мессенджерах и почта) не разглашается и используется только для решения вопросов, связанных с вашим заказом.</p>

            <h2>5. Сроки хранения данных</h2>
            <p>Ваши данные хранятся до момента выполнения заказа и в течение <strong>6 месяцев</strong> после этого для решения возможных вопросов по возврату или гарантии. По истечении этого срока данные удаляются, если вы не дали согласие на дальнейшее хранение.</p>

            <h2>6. Ваши права</h2>
            <p>Вы имеете право:</p>
            <ul>
                <li>Запросить информацию о том, какие ваши данные хранятся у меня;</li>
                <li>Потребовать удалить или исправить ваши персональные данные;</li>
                <li>Отозвать согласие на обработку данных в любое время.</li>
            </ul>
            <p>Для этого достаточно написать мне на почту.</p>

            <h2>7. Использование файлов cookie</h2>
            <p>Сайт может использовать файлы cookie для улучшения работы и анализа посещаемости. Вы можете отключить cookie в настройках вашего браузера, но это может повлиять на удобство использования сайта.</p>

            <h2>8. Ссылки на сторонние сайты</h2>
            <p>На Сайте могут быть ссылки на другие ресурсы (соцсети, службы доставки). Я не несу ответственности за политику конфиденциальности этих сайтов.</p>

            <h2>9. Изменения в политике</h2>
            <p>Я оставляю за собой право вносить изменения в настоящую Политику конфиденциальности. Актуальная версия всегда доступна на этой странице. Если изменения существенные — я уведомлю вас через сайт или в соцсетях.</p>

            <div class="policy-contact">
                <p><strong>📬 Контакты для вопросов о персональных данных:</strong></p>
                <p>Email: hearto@example.com</p>
                <p style="font-size: 13px; margin-top: 12px;">Вы можете связаться со мной в любое время для уточнения, изменения или удаления ваших данных.</p>
            </div>

            <div class="policy-date">
                <p>© 2026 HEARTO. Все права защищены.</p>
                <p>Дата последнего обновления: 01.04.2026</p>
            </div>
        </div>
    </div>

    <!-- FOOTER с цветом EFEAFF и акцентом 781C4F -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div><h3>HEARTO</h3><p>Авторские игрушки</p></div>
                <div>
                    <h4>Навигация</h4>
                    <a href="index.html#portfolio">Работы</a>
                    <a href="about.html">О мастере</a>
                    <a href="index.html#process">Процесс</a>
                    <a href="delivery.html">Доставка</a>
                    <a href="order.html">Заказать</a>
                </div>
                <div>
                    <h4>Документы</h4>
                    <a href="privacy.html" style="color: #1E1B4B; font-weight: 500;">Политика конфиденциальности</a>
                    <a href="terms.html">Пользовательское соглашение</a>
                </div>
                </div>
            </div>
            <div class="copyright"><p>© 2026 HEARTO</p></div>
        </div>
    </footer>

    <!-- ПОМОЩНИК -->
    <div id="assistantOpen" class="assistant-open">💬</div>
    <div id="assistant" class="assistant">
        <div id="questions" class="assistant-questions"></div>
        <div id="message" class="assistant-text"></div>
        <div class="assistant-character">
            <img id="characterImg" src="images/talk.jfif" alt="Помощник">
        </div>
        <button id="assistantClose" class="assistant-close">⭐</button>
    </div>

    <audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>
    <script src="script.js"></script>
</body>
</html>
// Header blur
window.addEventListener('scroll', () => {
    const header = document.getElementById('header');
    if (header) header.classList.toggle('scrolled', window.scrollY > 50);
});

// Плавное появление
const observer = new IntersectionObserver(entries => {
    entries.forEach(e => e.isIntersecting && e.target.classList.add('show'));
});
document.querySelectorAll('section, .card').forEach(el => {
    el.classList.add('fade');
    observer.observe(el);
});

/* =========================
   КНОПКА ПОКАЗАТЬ/СКРЫТЬ ДОП. РАБОТЫ
========================= */
document.addEventListener('DOMContentLoaded', () => {
    const toggleBtn = document.getElementById('toggleExtraBtn');
    const extraWorks = document.querySelectorAll('.extra-work');
    
    if (toggleBtn && extraWorks.length > 0) {
        let isVisible = false; // сначала скрыты
        
        toggleBtn.addEventListener('click', () => {
            if (!isVisible) {
                // ПОКАЗЫВАЕМ дополнительные работы
                extraWorks.forEach(work => {
                    work.style.display = 'block';
                    work.style.animation = 'slideUp 0.4s ease forwards';
                });
                toggleBtn.innerHTML = 'Скрыть дополнительные работы';
                toggleBtn.style.background = 'linear-gradient(135deg, #97277A, #C93367)';
                isVisible = true;
                
                if (typeof starRain === 'function') {
                    starRain({ particleCount: 80, spread: 60, origin: { y: 0.7 } });
                }
            } else {
                // СКРЫВАЕМ дополнительные работы
                extraWorks.forEach(work => {
                    work.style.display = 'none';
                });
                toggleBtn.innerHTML = 'Показать ещё работы';
                toggleBtn.style.background = 'linear-gradient(135deg, #5B4BFF, #8A7CFF)';
                isVisible = false;
            }
        });
    }
});

// Анимация появления для доп. работ
const style = document.createElement('style');
style.textContent = `
    @keyframes slideUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }
`;
document.head.appendChild(style);



/* =========================
МОДАЛЬНОЕ ОКНО (ИСПРАВЛЕНО)
========================= */
const modal = document.getElementById('workModal');
if (modal) {
  const modalImg = modal.querySelector('.modal-img');
  const modalTitle = modal.querySelector('.modal-title');
  const modalDesc = modal.querySelector('.modal-desc');
  const grid = document.querySelector('#portfolio .grid'); // Ищем сетку в портфолио

  grid?.addEventListener('click', (e) => {
    const card = e.target.closest('.card');
    if (!card) return;
    
    modalImg.src = card.querySelector('img')?.src || '';
    // ВАЖНО: в HTML используется h4, а не h3
    modalTitle.textContent = card.querySelector('h4')?.textContent || ''; 
    modalDesc.textContent = card.querySelector('p')?.textContent || '';
    
    modal.classList.add('is-active');
    document.body.style.overflow = 'hidden';
  });

  modal.querySelector('.modal-close')?.addEventListener('click', () => {
    modal.classList.remove('is-active');
    document.body.style.overflow = '';
  });
  modal.addEventListener('click', (e) => { 
    if (e.target === modal) {
      modal.classList.remove('is-active');
      document.body.style.overflow = '';
    }
  });
}

/* =========================
   ПОМОЩНИК
========================= */
const openBtn = document.getElementById('assistantOpen');
const assistant = document.getElementById('assistant');
const message = document.getElementById('message');
const questions = document.getElementById('questions');
const characterImg = document.getElementById('characterImg');
const closeBtn = document.getElementById('assistantClose');
const typingAudio = document.getElementById('typingSound');

let talkingInterval = null;
let typingInterval = null;
let soundInterval = null;

// Управление звуком
function startSound() {
    if (soundInterval) clearInterval(soundInterval);
    if (typingAudio && !window._soundBlocked) {
        typingAudio.volume = 0.1;
        typingAudio.play().catch(() => { window._soundBlocked = true; });
        soundInterval = setInterval(() => {
            if (typingAudio && !window._soundBlocked) {
                typingAudio.currentTime = 0;
                typingAudio.play().catch(() => {});
            }
        }, 100);
    }
}

function stopSound() {
    if (soundInterval) clearInterval(soundInterval);
    soundInterval = null;
    if (typingAudio) {
        typingAudio.pause();
        typingAudio.currentTime = 0;
    }
}

// Эффект печатания текста
function typeText(text, callback) {
    if (!message) return;
    message.innerText = '';
    message.classList.add('active');

    let i = 0;
    const speed = 55; // скорость печати (мс)

    startSound();     // звук сразу
    startTalking();   // анимация рта сразу

    typingInterval = setInterval(() => {
        if (i < text.length) {
            message.innerText += text.charAt(i); // корректно добавляет пробелы
            i++;
        } else {
            clearInterval(typingInterval);
            typingInterval = null;
            stopSound();
            if (callback) callback();
        }
    }, speed);
}

function showIntro() {
    if (questions) questions.style.display = 'none';
    message?.classList.remove('active');
    typeText("Привет! Я помогу тебе ✨", () => {
        setTimeout(() => {
            stopTalking();
            showQuestions();
        }, 2000);
    });
}

function showQuestions() {
    if (!questions) return;
    if (typingInterval) { clearInterval(typingInterval); typingInterval = null; }
    stopSound();
    stopTalking();

    message?.classList.remove('active');
    questions.style.display = 'flex';
    questions.innerHTML = '';

    const qData = [
        { id: 1, text: "Как заказать?" },
        { id: 2, text: "Доставка?" },
        { id: 3, text: "Материалы?" },
        { id: 4, text: "Как посмотреть отзовы?" }
    ];

    qData.forEach((q, i) => {
        const bubble = document.createElement("div");
        bubble.className = "question-bubble";
        bubble.innerText = q.text;
        bubble.style.animationDelay = `${i * 0.1}s`;
        bubble.addEventListener('click', () => answer(q.id));
        questions.appendChild(bubble);
    });
}

function answer(id) {
    let text = "";
    if (id === 1) text = "Заполни форму заказа ✨";
    else if (id === 2) text = "Перейдите во вкладку доставки и там вы все можите узнать";
    else if (id === 3) text = "Глина, искуственная шерсть, акрил и лак для акрила";
    else if (id === 4) text = "Посмотреть отзовы вы можите на страничке в вк";

    if (questions) {
        questions.innerHTML = '';
        questions.style.display = 'none';
    }

    typeText(text, () => {
        setTimeout(() => {
            stopTalking();
            showQuestions();
        }, 2500);
    });
}

function startTalking() {
    if (!characterImg) return;
    characterImg.classList.add('talking');
    let isOpen = false;
    characterImg.src = "images/talk.png";

    if (talkingInterval) clearInterval(talkingInterval);
    talkingInterval = setInterval(() => {
        if (characterImg) {
            characterImg.src = isOpen ? "images/talk.png" : "images/GAKUPO CATZ.png";
        }
        isOpen = !isOpen;
    }, 200);
}

function stopTalking() {
    if (talkingInterval) {
        clearInterval(talkingInterval);
        talkingInterval = null;
    }
    if (characterImg) {
        characterImg.src = "images/GAKUPO CATZ.png";
        characterImg.classList.remove('talking');
    }
}

// События
if (openBtn && assistant) {
    openBtn.addEventListener('click', () => {
        assistant.classList.add('is-open');
        openBtn.classList.add('is-hidden');
        showIntro();
    });

    closeBtn?.addEventListener('click', () => {
        assistant.classList.remove('is-open');
        openBtn.classList.remove('is-hidden');
        if (typingInterval) { clearInterval(typingInterval); typingInterval = null; }
        stopTalking();
        stopSound();
        message?.classList.remove('active');
        if (questions) questions.innerHTML = '';
    });

    // Клик по персонажу сбрасывает ответ и возвращает к вопросам
    characterImg?.addEventListener('click', () => {
        if (message && message.classList.contains('active')) {
            if (typingInterval) { clearInterval(typingInterval); typingInterval = null; }
            stopTalking();
            stopSound();
            message.classList.remove('active');
            showQuestions();
        }
    });
}

/* =========================
БУРГЕР-МЕНЮ (ФИНАЛЬНОЕ ИСПРАВЛЕНИЕ)
========================= */
document.addEventListener('DOMContentLoaded', () => {
  const burger = document.getElementById('burgerBtn');
  const nav = document.querySelector('nav');
  const overlay = document.getElementById('menuOverlay');

  if (!burger || !nav) return;

  const openMenu = () => {
    nav.classList.add('is-open');
    burger.classList.add('is-active');
    overlay?.classList.add('is-active');
    document.body.style.overflow = 'hidden';
  };

  const closeMenu = () => {
    nav.classList.remove('is-open');
    burger.classList.remove('is-active');
    overlay?.classList.remove('is-active');
    document.body.style.overflow = '';
  };

  // Клик по бургеру открывает/закрывает
  burger.addEventListener('click', () => {
    nav.classList.contains('is-open') ? closeMenu() : openMenu();
  });

  // Закрываем ТОЛЬКО если клик попал строго по серому фону, а не по меню
  overlay?.addEventListener('click', (e) => {
    if (e.target === overlay) closeMenu();
  });

  // Клик по любой ссылке закрывает меню (не ломая переход/скролл)
  nav.querySelectorAll('a').forEach(link => {
    link.addEventListener('click', closeMenu);
  });
});
/* =========================
   ПЛАВНЫЙ СКРОЛЛ
========================= */
document.querySelectorAll('a[href^="#"]').forEach(link => {
    link.addEventListener('click', function(e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) target.scrollIntoView({ behavior: 'smooth' });
    });
});

/* =========================
ПАРАЛЛАКС — МЕРЧ (ЛЕГКОЕ КОЛЕБАНИЕ)
========================= */
(() => {
    const merchSection = document.getElementById('merch');
    if (!merchSection) return;
    
    // Полностью отключаем параллакс на мобильных устройствах
    if (window.innerWidth <= 768) return;
    
    const items = merchSection.querySelectorAll('.parallax-item');
    if (items.length === 0) return;
    
    let targetX = 0, targetY = 0;
    let currentX = 0, currentY = 0;
    
    document.addEventListener('mousemove', (e) => {
        targetX = (e.clientX / window.innerWidth - 0.5) * 2;
        targetY = (e.clientY / window.innerHeight - 0.5) * 2;
    });
    
    function animate() {
        currentX += (targetX - currentX) * 0.08;
        currentY += (targetY - currentY) * 0.08;
        
        items.forEach((item) => {
            const speed = parseFloat(item.dataset.speed) || 10;
            // Максимальный сдвиг будет равен speed (например, 10-15px), 
            // что гарантирует, что объекты не уйдут далеко от своей позиции
            const moveX = currentX * speed;
            const moveY = currentY * speed;
            item.style.transform = `translate(${moveX}px, ${moveY}px)`;
        });
        
        requestAnimationFrame(animate);
    }
    animate();
})();

/* =========================
   ВОЛНИСТАЯ НИТКА — ПРОЦЕСС
========================= */
document.addEventListener('DOMContentLoaded', () => {
  const wrap = document.querySelector('.process-thread-wrap');
  if (!wrap) return;

  const W = 2000;
  const H = 28;
  const amp = 5;      // амплитуда волны
  const freq = 0.008; // частота

  // Строим волнистый path через весь блок
  function buildPath(offset) {
    let d = `M -100 ${H / 2}`;
    for (let x = -100; x <= W + 100; x += 4) {
      const y = H / 2 + Math.sin((x + offset) * freq * Math.PI * 2) * amp;
      d += ` L ${x} ${y.toFixed(2)}`;
    }
    return d;
  }

  const svgNS = 'http://www.w3.org/2000/svg';
  const svg = document.createElementNS(svgNS, 'svg');
  svg.setAttribute('class', 'process-thread-svg');
  svg.setAttribute('viewBox', `0 0 ${W} ${H}`);
  svg.setAttribute('preserveAspectRatio', 'none');

  const defs = document.createElementNS(svgNS, 'defs');
  const grad = document.createElementNS(svgNS, 'linearGradient');
  grad.setAttribute('id', 'threadGrad');
  grad.setAttribute('x1', '0%'); grad.setAttribute('x2', '100%');
  [
    { offset: '0%',   color: '#b8a9ff' },
    { offset: '30%',  color: '#8A7CFF' },
    { offset: '50%',  color: '#C93367' },
    { offset: '70%',  color: '#8A7CFF' },
    { offset: '100%', color: '#b8a9ff' },
  ].forEach(s => {
    const stop = document.createElementNS(svgNS, 'stop');
    stop.setAttribute('offset', s.offset);
    stop.setAttribute('stop-color', s.color);
    grad.appendChild(stop);
  });
  defs.appendChild(grad);
  svg.appendChild(defs);

  const path = document.createElementNS(svgNS, 'path');
  path.setAttribute('fill', 'none');
  path.setAttribute('stroke', 'url(#threadGrad)');
  path.setAttribute('stroke-width', '2');
  path.setAttribute('stroke-linecap', 'round');
  svg.appendChild(path);

  wrap.insertBefore(svg, wrap.firstChild);

  path.setAttribute('d', buildPath(0));
});
(() => {
    const merchSection = document.getElementById('merch');
    if (!merchSection) return;
    
    // Полностью отключаем параллакс на мобильных устройствах
    if (window.innerWidth <= 768) return;
    
    const items = merchSection.querySelectorAll('.parallax-item');
    if (items.length === 0) return;
    
    let targetX = 0, targetY = 0;
    let currentX = 0, currentY = 0;
    
    document.addEventListener('mousemove', (e) => {
        targetX = (e.clientX / window.innerWidth - 0.5) * 2;
        targetY = (e.clientY / window.innerHeight - 0.5) * 2;
    });
    
    function animate() {
        currentX += (targetX - currentX) * 0.08;
        currentY += (targetY - currentY) * 0.08;
        
        items.forEach((item) => {
            const speed = parseFloat(item.dataset.speed) || 10;
            // Максимальный сдвиг будет равен speed (например, 10-15px), 
            // что гарантирует, что объекты не уйдут далеко от своей позиции
            const moveX = currentX * speed;
            const moveY = currentY * speed;
            item.style.transform = `translate(${moveX}px, ${moveY}px)`;
        });
        
        requestAnimationFrame(animate);
    }
    animate();
})();
/* ===== БАЗА ===== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@font-face {
    font-family: 'MyFont';
    src: url('fonts/BubbleSans-Regular.otf') format('woff2');
    font-weight: normal;
    font-style: normal;
}

body {
    font-family: 'MyFont', sans-serif;
    background: #F6F5FF;
    color: #1E1B4B;
    line-height: 1.6;
}

/* ===== КОНТЕЙНЕР ===== */
.container {
    width: 90%;
    max-width: 1100px;
    margin: auto;
}

/* ===== ХЕДЕР ===== */
header {
    position: fixed;
    width: 100%;
    top: 0;
    padding: 16px 0;
    z-index: 1000;
    transition: 0.3s;
}

header.scrolled {
    background: rgba(246, 245, 255, 0.7);
    backdrop-filter: blur(12px);
}

.header-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-weight: 600;
    font-size: 20px;
    cursor: pointer;
}

nav {
    display: flex;
    align-items: center;
    gap: 20px;
}

nav a {
    text-decoration: none;
    color: #1E1B4B;
    font-size: 14px;
    position: relative;
}

nav a:not(.btn)::after {
    content: "";
    position: absolute;
    bottom: -4px;
    left: 0;
    width: 0%;
    height: 2px;
    background: #5B4BFF;
    transition: 0.3s;
}

nav a:not(.btn):hover::after {
    width: 100%;
}

/* ===== HERO ===== */
.hero {
    min-height: 85vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 100px 40px 60px;
    background: #faf7ff;
}

.hero-inner {
    width: 100%;
    max-width: 1600px;
    min-height: 700px;
    border-radius: 30px;
    overflow: hidden;
    position: relative;
    background: url('images/hero.gif') center/cover no-repeat;
}

.hero-inner::before {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(20, 10, 30, 0.35);
}

.hero-text {
    position: relative;
    z-index: 2;
    padding: 80px 60px;
}

.hero h1 {
    font-size: 42px;
    line-height: 1.2;
    font-weight: 400;
    margin-bottom: 20px;
    color: white;
    text-shadow: 0 8px 30px rgba(0,0,0,0.6);
}

.hero-sub {
    color: rgba(255,255,255,0.85);
    font-size: 16px;
    margin: 16px 0;
    line-height: 1.5;
}

/* ===== КНОПКИ ===== */
.btn {
    background: linear-gradient(135deg, #5B4BFF, #8A7CFF);
    color: white;
    padding: 10px 20px;
    border-radius: 30px;
    text-decoration: none;
    font-size: 14px;
    transition: 0.3s;
}

.btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(91, 75, 255, 0.3);
}

.btn:active {
    transform: scale(0.96);
}

/* ===== СЕКЦИИ ===== */
section {
    padding: 100px 0;
}

h2 {
    font-size: 30px;
    margin-bottom: 30px;
}

h2::after {
    content: "";
    display: block;
    width: 50px;
    height: 3px;
    background: linear-gradient(90deg, #5B4BFF, #C93367); /* ГРАДИЕНТ */
    border-radius: 2px;
}
/* ===== ПРОЦЕСС ===== */
#process {
  padding: 80px 0 100px;
  background: #f7f4fb;
  text-align: center;
  overflow: hidden;
}

#process h2 {
  font-size: 34px;
  margin-bottom: 70px;
  color: #1E1B4B;
}

#process h2::after { display: none; }

/* Обёртка — нитка идёт через весь блок секции за карточками */
.process-thread-wrap {
  position: relative;
}

/* SVG-нитка вставляется через JS */
.process-thread-svg {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 100vw;
  height: 28px;
  overflow: visible;
  z-index: 0;
  pointer-events: none;
}

.process-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 24px;
  position: relative;
  z-index: 1;
}

/* Карточка — подвешена под ниткой */
.step-card {
  background: #ffffff;
  padding: 36px 20px 28px;
  border-radius: 16px;
  box-shadow: 0 8px 28px rgba(91, 75, 255, 0.10), 0 2px 6px rgba(0,0,0,0.04);
  transition: transform 0.35s cubic-bezier(0.34, 1.56, 0.64, 1),
              box-shadow 0.3s ease;
  position: relative;
  transform-origin: top center;
  z-index: 1;
}

.step-card:hover {
  transform: rotate(-1.5deg) translateY(4px);
  box-shadow: 0 14px 36px rgba(91, 75, 255, 0.16), 0 4px 12px rgba(0,0,0,0.06);
}

/* Булавка — точка сверху каждой карточки */
.step-card::before {
  content: "";
  position: absolute;
  top: -6px;
  left: 50%;
  transform: translateX(-50%);
  width: 12px;
  height: 12px;
  border-radius: 50%;
  background: radial-gradient(circle at 35% 35%, #ffffff 0%, #C93367 60%, #97277A 100%);
  box-shadow: 0 2px 6px rgba(201, 51, 103, 0.5);
  z-index: 4;
}

/* Нитка от булавки до верха карточки */
.step-card::after {
  content: "";
  position: absolute;
  top: -1px;
  left: 50%;
  transform: translateX(-50%);
  width: 1.5px;
  height: 7px;
  background: linear-gradient(to bottom, #C93367, rgba(201,51,103,0.2));
  z-index: 2;
}

.step-card .icon {
  font-size: 40px;
  margin-bottom: 15px;
}

.step-card h3 {
  font-size: 18px;
  margin-bottom: 10px;
  color: #1E1B4B;
}

.step-card p {
  font-size: 14px;
  color: #666;
}

/* Однотонные иконки-кружки */
.icon {
  width: 64px;
  height: 64px;
  background: #f3e8ff;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 28px;
  margin: 0 auto 15px;
  box-shadow: inset 0 2px 6px rgba(91, 75, 255, 0.1);
}


/* ===== ПОРТФОЛИО ===== */
/* ===== КНОПКА ВНИЗУ ПОРТФОЛИО ===== */
.portfolio-footer {
    text-align: center;
    margin-top: 50px;
}

.btn-toggle {
    background: linear-gradient(135deg, #5B4BFF, #8A7CFF);
    color: white;
    border: none;
    padding: 12px 32px;
    border-radius: 40px;
    cursor: pointer;
    font-family: inherit;
    font-size: 15px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(91, 75, 255, 0.3);
}

.btn-toggle:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(91, 75, 255, 0.4);
}

.btn-toggle:active {
    transform: scale(0.96);
}

/* ===== КАРТОЧКИ ===== */
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
  align-items: stretch; /* Все карточки в ряду одной высоты */
}

.card {
  background: white;
  border-radius: 20px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(30,27,75,0.1);
  transition: all 0.3s ease;
  cursor: pointer;
  display: flex;
  flex-direction: column;
  height: 100%; /* Растягиваем на всю ячейку */
}

.card img {
  width: 100%;
  height: 240px;
  object-fit: cover;
  flex-shrink: 0;
}

.card-info {
  padding: 18px;
  display: flex;
  flex-direction: column;
  flex: 1; /* Занимает всё свободное место */
  justify-content: space-between;
}

.card-info h4 { font-size: 18px; margin-bottom: 6px; color: #1E1B4B; }
.card-info p { font-size: 13px; color: #6b5f7a; margin-bottom: 12px; }

/* Цена всегда видна и не обрезается */
.card-price {
  margin-top: auto; /* Прижимает к низу */
  padding: 10px 16px;
  background: linear-gradient(135deg, #f3e8ff, #e9d5ff);
  color: #5B4BFF;
  font-weight: 600;
  font-size: 15px;
  border-radius: 14px;
  align-self: flex-start;
  box-shadow: 0 3px 10px rgba(91,75,255,0.12);
  transition: all 0.3s ease;
  white-space: nowrap; /* Запрещаем перенос и обрезку текста */
  overflow: visible;
}

.card:hover .card-price {
  transform: scale(1.04);
  background: linear-gradient(135deg, #5B4BFF, #8A7CFF);
  color: #fff;
}

/* ===== КНОПКА СКРЫТЬ/ПОКАЗАТЬ ===== */
.toggle-works-btn {
    text-align: center;
    margin-bottom: 30px;
}

.btn-toggle {
    background: linear-gradient(135deg, #5B4BFF, #8A7CFF);
    color: white;
    border: none;
    padding: 10px 28px;
    border-radius: 40px;
    cursor: pointer;
    font-family: inherit;
    font-size: 14px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 12px rgba(91,75,255,0.2);
}

.btn-toggle:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(91,75,255,0.3);
}

.btn-toggle:active {
    transform: scale(0.96);
}

/* Скрытие работ */
.grid.hidden-works .card {
    display: none;
}
/* ===== МОДАЛЬНОЕ ОКНО ===== */
.modal-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(30, 27, 75, 0.9);
    backdrop-filter: blur(6px);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 3000;
    padding: 20px;
    opacity: 0;
    visibility: hidden;
    pointer-events: none;
    transition: opacity 0.3s ease, visibility 0.3s ease;
}

.modal-overlay.is-active {
    opacity: 1;
    visibility: visible;
    pointer-events: auto;
}

.modal-box {
    background: white;
    border-radius: 20px;
    max-width: 700px;
    width: 100%;
    overflow: hidden;
    position: relative;
    box-shadow: 0 20px 60px rgba(0,0,0,0.4);
    transform: scale(0.9) translateY(20px);
    transition: transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
}

.modal-overlay.is-active .modal-box {
    transform: scale(1) translateY(0);
}

.modal-close {
    position: absolute;
    top: 12px;
    right: 12px;
    background: rgba(0,0,0,0.6);
    color: white;
    border: none;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    font-size: 24px;
    cursor: pointer;
    z-index: 10;
    transition: 0.2s;
}

.modal-close:hover {
    background: rgba(0,0,0,0.8);
    transform: rotate(90deg);
}

.modal-overlay.is-active .modal-box { transform: scale(1) translateY(0); }
.modal-img {
  width: 100%; max-height: 65vh; object-fit: contain; background: #faf8ff;
  display: block; border-bottom: 1px solid #eee;
}
.modal-info { padding: 20px; }
.modal-info h3 { margin: 0 0 8px; font-size: 20px; }
.modal-info p { margin: 0; color: #6b5f7a; }

/* ===== Процесс ===== */
.steps {
    display: flex;
    gap: 24px;
    flex-wrap: wrap;
    margin-top: 40px;
}

.step {
    flex: 1;
    min-width: 180px;
    background: white;
    padding: 30px 20px;
    border-radius: 24px;
    text-align: center;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.04);
    transition: 0.2s;
}

.step:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 28px rgba(151, 39, 122, 0.1);
}

.icon {
    font-size: 32px;
    margin-bottom: 16px;
    color: #97277A;
}

.step h3 {
    font-size: 18px;
    margin-bottom: 8px;
}

.step p {
    font-size: 14px;
    color: #6b5f7a;
}

/* ===== АНИМАЦИЯ ПОЯВЛЕНИЯ ===== */
.fade {
    opacity: 0;
    transform: translateY(40px);
    transition: 0.6s;
}

.fade.show {
    opacity: 1;
    transform: translateY(0);
}

/* ===== ПОМОЩНИК ===== */
.assistant-open {
  position: fixed;
  bottom: 16px; /* ОДИНАКОВОЕ значение с панелью */
  right: 16px;
  width: 64px;
  height: 64px;
  background: linear-gradient(135deg, #5B4BFF, #8A7CFF);
  color: white;
  border-radius: 50%;
  cursor: pointer;
  z-index: 2000;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 28px;
  box-shadow: 0 6px 20px rgba(91, 75, 255, 0.4);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  animation: pulse 2s infinite;
}
.assistant-open:hover {
  transform: scale(1.1) rotate(8deg);
  box-shadow: 0 8px 25px rgba(91, 75, 255, 0.6);
}
.assistant-open.is-hidden {
  opacity: 0;
  transform: scale(0.6);
  pointer-events: none;
}
@keyframes pulse {
  0%, 100% { box-shadow: 0 0 0 0 rgba(91, 75, 255, 0.4); }
  50% { box-shadow: 0 0 0 10px rgba(91, 75, 255, 0); }
}

.assistant {
  position: fixed;
  bottom: 16px; /* <-- ГЛАВНОЕ ИСПРАВЛЕНИЕ: привязка к низу */
  right: -360px;
  width: 340px;
  max-height: 85vh; /* Не даёт улететь за экран */
  overflow-y: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 12px;
  z-index: 2001;
  transition: right 0.5s cubic-bezier(0.34, 1.56, 0.64, 1);
  pointer-events: none;
  padding-bottom: 15px;
}
.assistant.is-open {
  right: 12px; /* Выезжает ровно к кнопке */
  pointer-events: auto;
}

.assistant-character img {
  width: 190px; /* Увеличенный персонаж */
  height: auto;
  display: block;
  transition: 0.3s;
  filter: drop-shadow(0 10px 20px rgba(0,0,0,0.15));
}
.talking {
  animation: bounce 0.25s infinite alternate;
}
@keyframes bounce {
  from { transform: translateY(0); }
  to { transform: translateY(-5px); }
}

.assistant-questions {
  display: none;
  flex-direction: column;
  gap: 12px;
  width: 100%;
}
.question-bubble {
  background: white;
  padding: 14px 18px;
  border-radius: 18px;
  border-bottom-left-radius: 6px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  font-size: 15px;
  cursor: pointer;
  transition: all 0.2s ease;
  text-align: center;
  width: fit-content;
  max-width: 95%;
  align-self: flex-start;
  color: #1E1B4B;
  position: relative;
  border: 1px solid rgba(91, 75, 255, 0.1);
  animation: fadeInUp 0.3s ease forwards;
  opacity: 0;
}
.question-bubble:hover {
  background: #5B4BFF;
  color: white;
  transform: translateX(4px) scale(1.02);
  box-shadow: 0 6px 16px rgba(91, 75, 255, 0.25);
}
.question-bubble::after {
  content: "";
  position: absolute;
  bottom: -6px;
  left: 12px;
  width: 0;
  height: 0;
  border-left: 7px solid transparent;
  border-right: 7px solid transparent;
  border-top: 7px solid white;
  transition: 0.2s;
}
.question-bubble:hover::after { border-top-color: #5B4BFF; }
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

.assistant-text {
  background: white;
  padding: 16px 20px;
  border-radius: 18px;
  border-bottom-left-radius: 6px;
  margin-bottom: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.12);
  font-size: 15px;
  line-height: 1.6;
  display: none;
  width: 100%;
  text-align: left;
  color: #1E1B4B;
  border: 1px solid rgba(91, 75, 255, 0.1);
  position: relative;
  white-space: pre-wrap;
  word-break: break-word;
}
.assistant-text.active {
  display: block;
  animation: slideIn 0.3s ease forwards;
}
.assistant-text::after {
  content: "";
  position: absolute;
  bottom: -6px;
  left: 16px;
  width: 0;
  height: 0;
  border-left: 7px solid transparent;
  border-right: 7px solid transparent;
  border-top: 7px solid white;
}
@keyframes slideIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

.assistant-close {
  background: none;
  border: none;
  font-size: 32px;
  cursor: pointer;
  position: absolute;
  bottom: 18px;
  right: 12px;
  transition: all 0.2s ease;
  z-index: 2002;
  filter: drop-shadow(0 2px 4px rgba(0,0,0,0.2));
}
.assistant-close:hover {
  transform: scale(1.2) rotate(15deg);
  filter: drop-shadow(0 4px 8px rgba(0,0,0,0.3));
}

/* ===== FOOTER ===== */
footer {
    background: #1e1b4bde;
    color: white;
    padding: 50px 0;
}

.footer-grid {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 40px;
    padding-bottom: 40px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    margin-bottom: 30px;
}

.footer-grid h3, .footer-grid h4 {
    margin-bottom: 12px;
    font-weight: 500;
}

.footer-grid a {
    display: block;
    color: #ccc;
    text-decoration: none;
    margin-bottom: 8px;
    font-size: 14px;
    transition: 0.2s;
}

.footer-grid a:hover {
    color: #C93367;
}

.social-icons {
    display: flex;
    gap: 16px;
}

.social-icons a {
    font-size: 22px;
    margin-bottom: 0;
}

.copyright {
    text-align: center;
    font-size: 12px;
    color: #aaa;
}

/* ===== БУРГЕР ===== */
.burger {
    display: none;
    background: none;
    border: none;
    font-size: 28px;
    cursor: pointer;
    z-index: 1002;
}

.menu-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.4);
    opacity: 0;
    visibility: hidden;
    transition: 0.3s;
    z-index: 999;
}

.menu-overlay.is-active {
    opacity: 1;
    visibility: visible;
}

/* ===== АВТОРСКИЙ МЕРЧ — ДЕКОР ===== */
 
/* Большое размытое пятно — правый верх */
.merch-content {
    position: relative;
    z-index: 2;
    max-width: 550px;
    padding-top: 40px;
}
 
.merch-decorations {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 1;
}
 
/* ===== ПЛАНЕТЫ ===== */
.css-planet {
    position: absolute;
    border-radius: 50%;
}

/* Планета 1: Большая — лавандово-фиолетовая с кольцом */
.planet-main {
    width: 200px;
    height: 200px;
    top: 10%;
    right: 8%;
    z-index: 3;
    background:
        /* Блик сверху-слева */
        radial-gradient(ellipse 55% 35% at 30% 25%, rgba(255,255,255,0.55) 0%, transparent 60%),
        /* Полосы-атмосфера */
        repeating-linear-gradient(
            160deg,
            transparent 0px,
            transparent 18px,
            rgba(167, 139, 250, 0.18) 18px,
            rgba(167, 139, 250, 0.18) 22px,
            transparent 22px,
            transparent 38px,
            rgba(124, 58, 237, 0.12) 38px,
            rgba(124, 58, 237, 0.12) 41px
        ),
        /* Основной цвет */
        radial-gradient(circle at 38% 38%, #DDD6FE 0%, #A78BFA 45%, #7C3AED 80%, #4C1D95 100%);
    box-shadow:
        inset -18px -18px 40px rgba(76, 29, 149, 0.45),
        inset 6px 6px 20px rgba(255, 255, 255, 0.15),
        0 20px 60px rgba(124, 58, 237, 0.25),
        0 4px 20px rgba(76, 29, 149, 0.2);
}

/* Кольцо вокруг планеты */
.planet-main .planet-ring {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 310px;
    height: 75px;
    border-radius: 50%;
    transform: translate(-50%, -50%) rotate(-28deg);
    background: transparent;
    border: none;
    /* Два кольца через outline + border */
    box-shadow:
        0 0 0 5px rgba(167, 139, 250, 0.35),
        0 0 0 11px rgba(139, 92, 246, 0.15),
        0 0 0 16px rgba(124, 58, 237, 0.08);
    /* Кольцо обрезается за планетой через clip */
    overflow: visible;
}

/* Передняя часть кольца (поверх планеты) */
.planet-main .planet-ring::after {
    content: "";
    position: absolute;
    top: 50%;
    left: 50%;
    width: 310px;
    height: 75px;
    border-radius: 50%;
    transform: translate(-50%, -50%);
    border-top: 5px solid rgba(167, 139, 250, 0.55);
    border-bottom: 5px solid transparent;
    border-left: 5px solid transparent;
    border-right: 5px solid transparent;
}

/* Планета 2: Средняя — тёплая розово-персиковая */
.planet-pink {
    width: 120px;
    height: 120px;
    top: 55%;
    left: 6%;
    z-index: 2;
    background:
        radial-gradient(ellipse 50% 30% at 32% 28%, rgba(255,255,255,0.6) 0%, transparent 55%),
        repeating-linear-gradient(
            140deg,
            transparent 0px,
            transparent 14px,
            rgba(251, 113, 133, 0.15) 14px,
            rgba(251, 113, 133, 0.15) 17px,
            transparent 17px,
            transparent 28px,
            rgba(244, 63, 94, 0.1) 28px,
            rgba(244, 63, 94, 0.1) 30px
        ),
        radial-gradient(circle at 35% 35%, #FFE4E6 0%, #FDA4AF 40%, #FB7185 70%, #E11D48 100%);
    box-shadow:
        inset -12px -12px 28px rgba(190, 18, 60, 0.4),
        inset 5px 5px 14px rgba(255, 255, 255, 0.2),
        0 12px 35px rgba(251, 113, 133, 0.3),
        0 3px 12px rgba(225, 29, 72, 0.2);
}

/* ===== ЗВЁЗДЫ — четырёхлучевые ===== */
.css-star {
    position: absolute;
}

/* Четырёхлучевая звезда через clip-path */
.star-yellow {
    width: 22px;
    height: 22px;
    bottom: 22%;
    right: 18%;
    z-index: 4;
    background: radial-gradient(circle at 50% 50%, #FEF08A 0%, #FDE047 40%, #EAB308 100%);
    clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
    filter: drop-shadow(0 0 6px rgba(250, 204, 21, 0.7));
    animation: starSpin 8s linear infinite, twinkle 3s ease-in-out infinite;
}

.star-small {
    width: 14px;
    height: 14px;
    bottom: 30%;
    left: 20%;
    z-index: 4;
    background: radial-gradient(circle at 50% 50%, #FEF9C3 0%, #FDE047 50%, #CA8A04 100%);
    clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
    filter: drop-shadow(0 0 4px rgba(250, 204, 21, 0.6));
    animation: starSpin 12s linear infinite reverse, twinkle 2.5s ease-in-out infinite 1s;
}

.star-tiny {
    width: 10px;
    height: 10px;
    top: 28%;
    right: 28%;
    z-index: 4;
    background: radial-gradient(circle at 50% 50%, #ffffff 0%, #E9D5FF 40%, #A78BFA 100%);
    clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
    filter: drop-shadow(0 0 4px rgba(167, 139, 250, 0.8));
    animation: starSpin 10s linear infinite, twinkle 2s ease-in-out infinite 0.5s;
}

@keyframes starSpin {
    from { transform: rotate(0deg); }
    to   { transform: rotate(360deg); }
}

/* Анимация мерцания (более мягкая) */
@keyframes twinkle {
    0%, 100% { 
        opacity: 0.6; 
        transform: scale(1);
    }
    50% { 
        opacity: 1; 
        transform: scale(1.2);
    }
}
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <title>Пользовательское соглашение — HEARTO</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="style/adabtive.css">
    <style>
        /* Цвет фона страницы */
        body {
            background: #E5C4D6;
        }

        /* Дополнительные стили для страницы соглашения */
        .terms-hero {
            text-align: center;
            padding: 140px 20px 40px;
        }
        .terms-hero h1 {
            font-size: 42px;
            margin-bottom: 16px;
            color: #1E1B4B;
            word-break: break-word;
            hyphens: auto;
        }
        .terms-hero h1::after {
            content: "";
            display: block;
            width: 60px;
            height: 3px;
            background: linear-gradient(90deg, #5B4BFF, #781C4F);
            margin: 12px auto 0;
            border-radius: 2px;
        }
        .terms-hero .sub {
            font-size: 16px;
            color: #4a3858;
            max-width: 600px;
            margin: 0 auto;
            word-break: break-word;
        }

        /* Основной контент */
        .terms-content {
            max-width: 900px;
            margin: 0 auto 80px;
            background: white;
            border-radius: 32px;
            padding: 50px 60px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.06);
            overflow-x: hidden;
            word-wrap: break-word;
        }
        .terms-content h2 {
            font-size: 26px;
            margin: 30px 0 15px;
            color: #1E1B4B;
            word-break: break-word;
        }
        .terms-content h2:first-of-type {
            margin-top: 0;
        }
        .terms-content h2::after {
            display: none;
        }
        .terms-content h3 {
            font-size: 20px;
            margin: 25px 0 12px;
            color: #781C4F;
            word-break: break-word;
        }
        .terms-content p {
            color: #4a4568;
            line-height: 1.7;
            margin-bottom: 16px;
            font-size: 15px;
            word-break: break-word;
        }
        .terms-content ul {
            margin: 15px 0 20px;
            padding-left: 25px;
        }
        .terms-content li {
            color: #4a4568;
            margin-bottom: 10px;
            line-height: 1.6;
            word-break: break-word;
        }
        .terms-content strong {
            color: #781C4F;
        }
        .terms-date {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #e0d6f0;
            font-size: 14px;
            color: #8a7aad;
            text-align: center;
        }
        .terms-contact {
            background: #F6F5FF;
            border-radius: 20px;
            padding: 20px 28px;
            margin-top: 35px;
            text-align: center;
        }
        .terms-contact p {
            margin-bottom: 8px;
            word-break: break-word;
        }
        .terms-contact a {
            color: #781C4F;
            text-decoration: none;
            font-weight: 500;
            word-break: break-all;
        }
        .terms-contact a:hover {
            text-decoration: underline;
        }

        @media (max-width: 768px) {
            .terms-hero { 
                padding-top: 100px; 
                padding-left: 16px;
                padding-right: 16px;
            }
            .terms-hero h1 { 
                font-size: 28px; 
                line-height: 1.3;
            }
            .terms-content { 
                padding: 28px 20px; 
                margin-left: 16px;
                margin-right: 16px;
                width: calc(100% - 32px);
                box-sizing: border-box;
            }
            .terms-content h2 { 
                font-size: 22px; 
            }
            .terms-content h3 { 
                font-size: 18px; 
            }
            .terms-content ul {
                padding-left: 20px;
            }
        }

        @media (max-width: 480px) {
            .terms-content {
                padding: 22px 16px;
            }
            .terms-content h2 {
                font-size: 20px;
            }
            .terms-contact {
                padding: 16px;
            }
        }

        /* Футер остаётся как в основных стилях (без переопределения) */
        /* Убираем возможный конфликт — футер использует стандартный background из style.css */
    </style>
</head>
<body>

    <!-- ХЕДЕР -->
    <header id="header">
        <div class="container header-inner">
            <div class="logo" onclick="location.href='index.html'">HEARTO</div>
            <button class="burger" id="burgerBtn">☰</button>
            <nav>
                <a href="index.html#portfolio">Работы</a>
                <a href="about.html">О мастере</a>
                <a href="index.html#process">Процесс</a>
                <a href="delivery.html">Доставка</a>
                <a href="order.html" class="btn">Заказать</a>
            </nav>
        </div>
    </header>
    <div class="menu-overlay" id="menuOverlay"></div>

    <!-- ОСНОВНОЙ КОНТЕНТ -->
    <div class="container" style="width: 100%; padding-left: 0; padding-right: 0;">
        <div class="terms-hero">
            <h1>Пользовательское соглашение</h1>
        </div>

        <div class="terms-content">
            <h2>1. Общие положения</h2>
            <p>Настоящее Пользовательское соглашение (далее — «Соглашение») регулирует отношения между мастером-создателем HEARTO (далее — «Исполнитель») и посетителем сайта / заказчиком (далее — «Пользователь» или «Заказчик») при оформлении и приобретении авторских игрушек ручной работы.</p>
            <p>Оформляя заказ на Сайте или через мессенджеры, вы автоматически соглашаетесь с условиями настоящего Соглашения.</p>

            <h2>2. Порядок оформления заказа</h2>
            <p>2.1. Заказ оформляется через форму на странице <a href="order.html" style="color: #781C4F;">«Заказать»</a>.
            <p>2.2. После получения заявки Исполнитель связывается с Заказчиком для уточнения деталей: размера, цвета, материалов, стоимости и сроков изготовления.</p>
            <p>2.3. Эскиз и все особенности игрушки согласовываются с Заказчиком до начала работы. После согласования изменения вносятся только за дополнительную плату.</p>

            <h2>3. Оплата</h2>
            <p>3.1. Цена на игрушку формируется индивидуально и зависит от сложности, размера и используемых материалов.</p>
            <p>3.2. <strong>Предоплата составляет 100%</strong> от стоимости игрушки + стоимость доставки (если она известна на момент оплаты). Если стоимость доставки уточняется после упаковки — она оплачивается отдельно перед отправкой.</p>
            <p>3.3. Способы оплаты: перевод на банковскую карту или по номеру телефона (реквизиты предоставляются при оформлении).</p>
            <p>3.4. После получения предоплаты Исполнитель приступает к созданию игрушки.</p>

            <h2>4. Сроки изготовления</h2>
            <p>4.1. Средний срок изготовления игрушки — от 7 до 21 дня, в зависимости от сложности и текущей загруженности.</p>
            <p>4.2. Точные сроки оговариваются индивидуально. При задержке Исполнитель обязан предупредить Заказчика не позднее чем за 3 дня до истечения срока.</p>

            <h2>5. Доставка</h2>
            <p>5.1. Исполнитель отправляет заказы только по России через службы: <strong>СДЭК, ТК КИТ, Почта России</strong>.</p>
            <p>5.2. Доставка оплачивается Заказчиком отдельно и не входит в стоимость игрушки.</p>
            <p>5.3. После отправки Заказчику предоставляется трек-номер для отслеживания.</p>
            <p>5.4. Риски, связанные с повреждением посылки при пересылке, несёт Исполнитель до момента передачи посылки в службу доставки. После отправки ответственность за сохранность несёт служба доставки. Претензии по повреждениям решаются в рамках <a href="delivery.html" style="color: #781C4F;">условий возврата</a>.</p>

            <h2>6. Возврат и обмен</h2>
            <p>6.1. Возврат возможен только в случаях, указанных в <a href="delivery.html" style="color: #781C4F;">разделе «Доставка и возврат»</a>.</p>
            <p>6.2. Срок обращения по возврату — <strong>7 календарных дней</strong> с момента получения посылки.</p>
            <p>6.3. При подтверждении брака Исполнитель обязуется бесплатно отремонтировать игрушку или вернуть деньги за неё (стоимость доставки не возвращается).</p>
            <p>6.4. Возврат качественного товара (если Заказчик передумал) не осуществляется.</p>

            <h2>7. Права и обязанности сторон</h2>
            <p><strong>Исполнитель обязуется:</strong></p>
            <ul>
                <li>Изготовить игрушку в соответствии с согласованным эскизом;</li>
                <li>Использовать безопасные материалы;</li>
                <li>Упаковать игрушку надёжно для пересылки;</li>
                <li>Предоставить трек-номер после отправки.</li>
            </ul>
            <p><strong>Заказчик обязуется:</strong></p>
            <ul>
                <li>Своевременно оплатить заказ и доставку;</li>
                <li>Предоставить корректные данные для отправки (адрес, телефон);</li>
                <li>Получить посылку в отделении или у курьера в течение срока хранения.</li>
            </ul>

            <h2>8. Ответственность сторон</h2>
            <p>8.1. Исполнитель не несёт ответственности за задержки доставки со стороны служб перевозки.</p>
            <p>8.2. Исполнитель не несёт ответственности за естественные особенности ручной работы: лёгкая асимметрия, разница в оттенках, небольшие неровности. Эти особенности не являются браком.</p>
            <p>8.3. В случае форс-мажора (болезнь, технические проблемы и т.д.) сроки изготовления могут быть сдвинуты — Исполнитель обязуется уведомить Заказчика.</p>

            <h2>9. Конфиденциальность</h2>
            <p>Ваши персональные данные (имя, адрес, телефон) используются исключительно для выполнения заказа и не передаются третьим лицам, кроме как службам доставки. Подробнее — в <a href="privacy.html" style="color: #781C4F;">Политике конфиденциальности</a>.</p>

            <h2>10. Заключительные положения</h2>
            <p>10.1. Исполнитель оставляет за собой право вносить изменения в настоящее Соглашение без предварительного уведомления. Актуальная версия всегда доступна на этой странице.</p>
            <p>10.2. Все споры решаются путём переговоров. Если согласие не достигнуто — в соответствии с законодательством РФ по месту нахождения Исполнителя.</p>
            <p>10.3. Оформляя заказ, вы подтверждаете, что ознакомлены и согласны со всеми пунктами Соглашения.</p>

            <div class="terms-contact">
                <p><strong>📬 Контакты для связи:</strong></p>
                <p>Email: hearto@example.com</p>
                <p style="font-size: 13px; margin-top: 12px;">По всем вопросам, связанным с заказами, доставкой и возвратом, обращайтесь к мастеру напрямую.</p>
            </div>

            <div class="terms-date">
                <p>© 2026 HEARTO. Все права защищены.</p>
            </div>
        </div>
    </div>

    <!-- FOOTER (из style.css — стандартный, без изменений) -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div><h3>HEARTO</h3><p>Авторские игрушки</p></div>
                <div>
                    <h4>Навигация</h4>
                    <a href="index.html#portfolio">Работы</a>
                    <a href="about.html">О мастере</a>
                    <a href="index.html#process">Процесс</a>
                    <a href="delivery.html">Доставка</a>
                    <a href="order.html">Заказать</a>
                </div>
                <div>
                    <h4>Документы</h4>
                    <a href="privacy.html">Политика конфиденциальности</a>
                    <a href="terms.html" style="color: #C93367; font-weight: 500;">Пользовательское соглашение</a>
                </div>
                </div>
            </div>
            <div class="copyright"><p>© 2026 HEARTO</p></div>
        </div>
    </footer>

    <!-- ПОМОЩНИК -->
    <div id="assistantOpen" class="assistant-open">💬</div>
    <div id="assistant" class="assistant">
        <div id="questions" class="assistant-questions"></div>
        <div id="message" class="assistant-text"></div>
        <div class="assistant-character">
            <img id="characterImg" src="images/talk.jfif" alt="Помощник">
        </div>
        <button id="assistantClose" class="assistant-close">⭐</button>
    </div>

    <audio id="typingSound" src="sounds/typing.wav" preload="auto"></audio>
    <script src="script.js"></script>
</body>
</html>
