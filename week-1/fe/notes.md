# Конспект: Основы HTML5 и CSS3

## 1. Структура HTML-документа
```html
<!DOCTYPE html> <html lang="ru"> <head>
    <meta charset="UTF-8"> <title>Моя первая страница</title> </head>
<body>
    </body>
</html>
<header>
    <nav>
        <a href="/">Главная</a> | <a href="/about">О нас</a>
    </nav>
</header>

<main>
    <section>
        <h1>Добро пожаловать на стажировку!</h1>
        <article>
            <h2>Новость дня</h2>
            <p>Изучаем базовую теорию HTML и CSS перед практикой.</p>
        </article>
    </section>
</main>

<footer>
    <p>&copy; 2026 Моя Стажировка</p>
</footer>
<div class="card-container">
    <h2 id="main-card-title">Профиль студента</h2>
    <p>Привет! Меня зовут <span>Нурлыбай</span>.</p>
    
    <img src="avatar.jpg" alt="Фотография студента" width="150">
    
    <h3>Мои цели:</h3>
    <ul>
        <li>Освоить терминал</li>
        <li>Понять HTML/CSS</li>
        <li>Изучить JavaScript</li>
    </ul>
    
    <a href="[https://github.com](https://github.com)" target="_blank">Мой GitHub</a>
</div>
/* 1. Селектор по тегу (применится ко всем параграфам) */
p {
    color: #333333; /* Цвет текста */
    font-family: 'Arial', sans-serif; /* Шрифт */
    font-size: 16px; /* Размер шрифта */
}

/* 2. Селектор по классу (начинается с точки) */
.card-container {
    background-color: #f4f4f4; /* Цвет фона */
    text-align: center; /* Выравнивание текста */
}

/* 3. Селектор по ID (начинается с решетки #) */
#main-card-title {
    font-size: 24px;
    color: darkblue;
}

/* 4. Селектор потомка (ищет тег span только внутри класса .card-container) */
.card-container span {
    font-weight: bold;
    color: crimson;
}
.box-example {
    width: 300px;         /* Ширина контента */
    height: 150px;        /* Высота контента */
    padding: 20px;        /* Внутренний отступ (между текстом и рамкой) */
    border: 2px solid #000; /* Рамка элемента */
    margin: 15px;         /* Внешний отступ (отодвигает соседние блоки) */
}