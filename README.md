
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Меню Кафе</title>
    <style>
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideIn {
            from { transform: translateY(20px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f9fa;
            color: #333;
        }
        .container {
            width: 80%;
            margin: 0 auto;
            padding: 20px;
            animation: fadeIn 2s ease-in;
        }
        .header {
            text-align: center;
            padding: 50px 0;
            background-color: #343a40;
            color: white;
            animation: fadeIn 2s ease-in;
        }
        .header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        .header p {
            margin: 10px 0 0;
            font-size: 1.2em;
        }
        .menu-section {
            margin-bottom: 50px;
        }
        .menu-section h2 {
            background-color: #343a40;
            color: white;
            padding: 10px;
            margin: 0 -20px;
            animation: fadeIn 1.5s ease-in;
        }
        .menu-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px;
            border-bottom: 1px solid #ddd;
            animation: slideIn 1s ease-in;
        }
        .menu-item:last-child {
            border-bottom: none;
        }
        .menu-item img {
            width: 100px;
            height: 100px;
            object-fit: cover;
            border-radius: 10px;
            margin-right: 20px;
            transition: transform 0.3s ease;
            cursor: pointer;
        }
        .menu-item img:hover {
            transform: scale(2.2);
        }
        .menu-item-details {
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }
        .menu-item h3 {
            margin: 0;
            font-size: 1.2em;
        }
        .menu-item p {
            margin: 5px 0;
            color: #777;
        }
        .menu-item span {
            font-weight: bold;
            font-size: 1.2em;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #343a40;
            color: white;
            position: fixed;
            width: 100%;
            bottom: 0;
            animation: fadeIn 2s ease-in;
        }
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.9);
            justify-content: center;
            align-items: center;
        }
        .modal-content {
            position: relative;
            background-color: #fefefe;
            margin: auto;
            padding: 0;
            border: 1px solid #888;
            width: 80%;
            max-width: 700px;
        }
        .modal-content img {
            width: 100%;
        }
        .close {
            position: absolute;
            top: 10px;
            right: 25px;
            color: #fff;
            font-size: 35px;
            font-weight: bold;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Меню Кафе</h1>
        <p>Ласкаво просимо до нашого кафе!</p>
    </div>
    <div class="container">
        <div class="menu-section">
            <h2>Сніданки</h2>
            <div class="menu-item">
                <img src="img/p_O.jpg" alt="Яєшня з беконом">
                <div class="menu-item-details">
                    <h3>Яєшня з беконом</h3>
                    <p>Смажені яйця з хрустким беконом (150 г)</p>
                </div>
                <span>85 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/3b425e0e930b187d5c782c8cf1623e38.jpeg" alt="Омлет з овочами">
                <div class="menu-item-details">
                    <h3>Омлет з овочами</h3>
                    <p>Омлет з свіжими овочами (200 г)</p>
                </div>
                <span>75 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/018c39fc-2159-728b-8487-0b7537edd70f-826x0.png" alt="Вівсянка з фруктами">
                <div class="menu-item-details">
                    <h3>Вівсянка з фруктами</h3>
                    <p>Вівсянка з сезонними фруктами (250 г)</p>
                </div>
                <span>60 грн</span>
            </div>
        </div>
        <div class="menu-section">
            <h2>Основні страви</h2>
            <div class="menu-item">
                <img src="img/145111-ed4_wide.jpg" alt="Курячий стейк">
                <div class="menu-item-details">
                    <h3>Курячий стейк</h3>
                    <p>Грильований курячий стейк з овочами (300 г)</p>
                </div>
                <span>150 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/maxresdefault.jpg" alt="Рибне філе">
                <div class="menu-item-details">
                    <h3>Рибне філе</h3>
                    <p>Філе риби з лимонним соусом (250 г)</p>
                </div>
                <span>200 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/r7cvy7---c2000x1050x0sx215s-up--13374247a14860206d3917b925633a80.jpg" alt="Вегетаріанське карі">
                <div class="menu-item-details">
                    <h3>Вегетаріанське карі</h3>
                    <p>Карі з овочами та нутом (280 г)</p>
                </div>
                <span>120 грн</span>
            </div>
        </div>
        <div class="menu-section">
            <h2>Десерти</h2>
            <div class="menu-item">
                <img src="img/002d5e930aab5f9ba840f374a3e142aa.jpg" alt="Шоколадний торт">
                <div class="menu-item-details">
                    <h3>Шоколадний торт</h3>
                    <p>Ніжний торт з темного шоколаду (150 г)</p>
                </div>
                <span>70 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/Chizkeyk-iz-tvoroga-500350-scaled.jpg" alt="Чизкейк">
                <div class="menu-item-details">
                    <h3>Чизкейк</h3>
                    <p>Класичний чизкейк з полуничним соусом (160 г)</p>
                </div>
                <span>80 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/original.jpg" alt="Фруктовий салат">
                <div class="menu-item-details">
                    <h3>Фруктовий салат</h3>
                    <p>Свіжий салат з сезонних фруктів (200 г)</p>
                </div>
                <span>65 грн</span>
            </div>
        </div>
        <div class="menu-section">
            <h2>Напої</h2>
            <div class="menu-item">
                <img src="img/coffesourse.jpg" alt="Кава">
                <div class="menu-item-details">
                    <h3>Кава</h3>
                    <p>Чорна кава, капучино, латте (200 мл)</p>
                </div>
                <span>40 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/7c664063ba5e6215cb3567de3330c187.jpg" alt="Чай">
                <div class="menu-item-details">
                    <h3>Чай</h3>
                    <p>Зелений, чорний, трав'яний чай (300 мл)</p>
                </div>
                <span>30 грн</span>
            </div>
            <div class="menu-item">
                <img src="img/18347-ed4_wide.jpg" alt="Смузі">
                <div class="menu-item-details">
                    <h3>Смузі</h3>
                    <p>Смузі з фруктів та ягід (250 мл)</p>
                </div>
                <span>50 грн</span>
            </div>
        </div>
    </div>
