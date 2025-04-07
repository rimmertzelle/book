# Handout CSS

Unfortunately, the last lesson contained so much content that we couldn't cover all of it.

All code can be found ont [Github](https://github.com/HZ-HBO-ICT/css-tailwind)

## References

[Tailwind CSS - Rapidly build modern websites without ever leaving your HTML.](https://tailwindcss.com/)

[A Complete Guide to Flexbox | CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

[A Complete Guide to CSS Grid | CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

[Basic concepts of grid layout - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout/Basic_concepts_of_grid_layout)

[State of CSS 2023: CSS Frameworks](https://2023.stateofcss.com/en-US/css-frameworks)

### Assignment

We want to implement this design

![Screenshot 2024-05-27 at 17.05.28.png](Handout%20CSS%20299a2adea95942519d85f5c4dd36a153/Screenshot_2024-05-27_at_17.05.28.png)

We will implement this design using the following step-by-step approach.

1. Step 1 - HTML and CSS with flexbox
2. Step 2 - HTML with tailwind and flexbox
3. Step 3 - HTML with tailwind and cssgrid

### Step 1 - HTML and CSS with flexbox

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="./assets/css/style.css">
  <title>JS example</title>
</head>

<body>
  <header>
    <h1>Starwars</h1>
    <button>menu</button>
  </header>
  <main id="app" class="container">
    <section class="section">
      <article>
        <img src="./assets/img/luke.png" alt="Luke Skywalker" />
        <h2>Luke Skywalker</h2>
      </article>
      <article>
        <img src="./assets/img/c3po.png" alt="C-3PO" />
        <h2>C-3PO</h2>
      </article>
      <article>
        <img src="./assets/img/r2d2.png" alt="R2D2" />
        <h2>R2D2</h2>
      </article>
      <article>
        <img src="./assets/img/darthvader.png" alt="Darth Vader" />
        <h2>Darth Vader</h2>
      </article>
    </section>
  </main>
  <script type="module" src="./assets/js/main.js"></script>
</body>

</html>
```

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #f1f1f1;
    padding: 10px;

}

.container {
    padding: 10px;
    width: 100%;
    display: flex;
    justify-content: center;
    flex-direction: row;
    align-items: center;
}

```

### Step 2 - HTML with tailwind and flexbox

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="./assets/css/style.css">
  <title>JS example</title>
</head>

<body class="h-screen flex flex-col">
  <header class="bg-gray-700 p-3 flex justify-between">
    <h1 class="text-white">Starwars</h1>
    <button class="text-white">menu</button>
  </header>
  <main id="app" class="h-full flex flex-row p-10 justify-center flex-wrap content-center">
    <article>
      <img src="./assets/img/luke.png" alt="Luke Skywalker" />
      <h2>Luke Skywalker</h2>
    </article>
    <article>
      <img src="./assets/img/c3po.png" alt="C-3PO" />
      <h2>C-3PO</h2>
    </article>
    <article>
      <img src="./assets/img/r2d2.png" alt="R2D2" />
      <h2>R2D2</h2>
    </article>
    <article>
      <img src="./assets/img/darthvader.png" alt="Darth Vader" />
      <h2>Darth Vader</h2>
    </article>
  </main>
  <script type="module" src="./assets/js/main.js"></script>
</body>

</html>
```

### Step 3 - HTML with tailwind and cssgrid

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="./assets/css/style.css">
  <title>JS example</title>
</head>

<body class="h-screen flex flex-col">
  <header class="bg-gray-700 p-3 flex justify-between">
    <h1 class="text-white">Starwars</h1>
    <button class="text-white">menu</button>
  </header>
  <main id="app" class="h-full grid grid-cols-2 md:grid-cols-4 gap-4 p-10 justify-items-center content-center">
    <article>
      <img src="./assets/img/luke.png" alt="Luke Skywalker" />
      <h2>Luke Skywalker</h2>
    </article>
    <article>
      <img src="./assets/img/c3po.png" alt="C-3PO" />
      <h2>C-3PO</h2>
    </article>
    <article>
      <img src="./assets/img/r2d2.png" alt="R2D2" />
      <h2>R2D2</h2>
    </article>
    <article>
      <img src="./assets/img/darthvader.png" alt="Darth Vader" />
      <h2>Darth Vader</h2>
    </article>
  </main>
  <script type="module" src="./assets/js/main.js"></script>
</body>

</html>
```