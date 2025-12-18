# Basico de html

```html
<body class="grid-container">
    
    <!--Inicio header-->
    <header class="header">
        header
    </header>
    <!--Fin header-->

    <!--Inicio main-->
    <main class="main">
        main
    </main>
    <!--Fin main-->

    <!--Inicio footer-->
    <footer class="footer">
        footer
    </footer>
    <!--Fin footer-->

</body>
```

## Basico de css

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    text-decoration: none;
    list-style: none;
}

body {
    font-family: "Montserrat Alternates", sans-serif;
    background-color: white;
}
```

## Basico body css responsive

```css
.grid-container > * {
    border: 2px solid gray;
    border-radius: 7px;
    padding: 10px;
    text-align: center; 
}

.grid-container {
    display: grid;

    grid-template: 
    "header" 80px
    "main" 1fr
    "footer" 100px /
    100%;

    .header {
        grid-area: header;
        background-color: aqua;
    }

    .main {
        grid-area: main;
        background-color: bisque;
    }

    .footer {
        grid-area: footer;
        background-color: cadetblue;
    }

    @media (min-width: 992px) {
        grid-template: 
            "header" 100px
            "main" 1fr
            "footer" 100px /
            100%;
    }
}
```

## Imagenes responsive css

```css
.cont-img-hero {
    width: 100%;
    min-width: 300px;
}

.cont-img-hero img {
    width: 100%;
}
```

## Cards css

