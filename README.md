# Base layout by Lexx

Рабочий пример можно посмотреть в демо!
[Live Demo!](https://alexriz.github.io/layout/)

## CSS Rules

1. Базовый фон страницы устанавливается на html
2. Основной шрифт, его размер и цвет устанавливаются в html. Это позволяет гибко настраивать поведение относительных единиц измерения **rem** и настроить общее поведение шрифтов на странице. Так же мы можем разрешить или запретить изменения размеров шрифта в зависимости от параметров браузера.
3. Основные параметры страницы, такие как width, min-width указываются в body. Так же допустимо установка **дополнительного фона**, если необходимо.
4. Запрещенно ограничивать высоту (height: 100%; max-height: 100%;) для html и body

## SASS Template
```scss
html {
    font: 1em/normal sans-serif;
}

body {
    width: 100%;
    min-width: 320px;
    min-height: 100vh;
    margin: 0;
    display: flex;
    flex-direction: column;
}

textarea, input, button, select {
    font-size: 1rem;
    font-family: sans-serif;
}

button::-moz-focus-inner {
    margin: 0;
    padding: 0;
    border: 0
}

template {
    display: none;
}

a {
    color: #1194c4;
    text-decoration: underline;

    &:hover {
        text-decoration: none;
    }
}

:focus {
    outline: none;
}

img {
    border: 0;
}

.header {
    flex: 0 0 auto;
}

.main {
    flex: 1 0 auto;
}

.footer {
    flex: 0 0 auto;
}
```

## HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Title</title>
    <link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
    <header class="header">
        #Header
    </header>
    <main class="main">
        #Main
    </main>
    <footer class="footer">
        #Footer
    </footer>
</body>
</html>

```

### Say NO!
Скажи нет ресетам, нормалайзам и прочему мусору. **Пиши чистый код - будь Pro!**

Good Luck & Have Fun :zap::zap::zap:
