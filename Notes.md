# HTML & CSS

## Elements of an HTML document

We have the following:
    - `<!doctype html>` - Required preamble.
    - `<html></html> - "Root Element", wraps all the content on page.
         - `<lang>` - <html> includes the `lang` attribute, setting primary language for the document.
    - `<head></head>`- Acts as a container for all the stuff you want to include on the HTML. Viewport, keystrokes, charsets, etc...
    - `<meta charset="utf-8">` - Sets the document character element to utf-8, the most universal text reader.
    - `<meta name="viewport" content="width=device-width">` - Prevents you from rendering a page too big for your screen.
    - `<title></title>` - Sets the page title.
    - `<body></body>` - Contains all the content they they would be looking for when they go to a website.


## Paragraphs & Lists
<p>- Paragraphs are written between P-P.
    <ul>- Unordered List
        <li>milk</li>
        <li>sugar</li>
        <li>eggs</li>
    </ul>
    <ol>- Ordered List
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
    </ol>
</p> 


## Creating Links

`<a>` element used to resemble "anchor".
    <a href="https://www.mozilla.org/en-US/about/manifesto/">
        Mozilla Manifesto
    </a>


## Order of operations

There is a way to use grid before your card modifiers
- They continued to be nested. Grid always goes on the outside of card.

<section class="menu">
  <h2>Menu</h2>
  <div class="grid">
    <a href="#cakes" class="btn">Cakes</a>

    or

<section id="pastries">
  <div class="grid">
    <article class="card"></article>
  </div>
</section>


## HTML Attributes
 `rel` - Defines the relationship between a linked resource and the current document. 

 ## index.html structuring
 - Copy and paste the following html into the .html folders. This will ensure they all share the smae architecture.
 This will be easier to scale if  angie decides to get a better website development software.

 <header>Same Nav</header>
<main>
  <h1>Cakes</h1>
  <div class="grid">
    <article class="card">...</article>
  </div>
</main>
<footer>Same Footer</footer>


------
Basically what my index.html looks like, minus a few functions

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>{{ page.title }} | {{ site.title }}</title>
  <link rel="stylesheet" href="/css/style.css">
</head>
<body>

<header class="hero">
  <h1>{{ site.title }}</h1>
</header>

<main>
  {{ content }}
</main>

<footer>
  <p>© 2026 {{ site.title }}</p>
</footer>

</body>
</html>


 ## Removal code I am saving

   <!-- <div class="card">Cakes</div> -->
  <!--- <div class="card">Cupcakes</div> -->
   <!--- <div class="card">Cookies</div>
    <div class="card">Chocolate</div>
    <div class="card">Pastries</div>
    <div class="card">Other</div>-->

--------
<section class="fast-sellers">
    <h2>Fast Sellers</h2>

    <div class="grid">

      <article class="card">
        <img src="images/Other/Yogurt_Cups.jpg" alt="Yogurt Cups">
        <h3>Yogurt & Fruit Cups - Real mixed berries</h3>
        <p class="price">$15.00</p>
      </article>

      <article class="card">
        <img src="images/cakes/No-bake-cheesecake_8.jpg" alt="Cheesecake">
        <h3>Multi-Flavor; No-Bake Cheesecake
          <p>$12.99</p>
        </h3>
      </article>

      <article class="card">
        <img src="images/Other/tamales.jpg" alt="Tamales">
        <h3>Traditional Tamales - Beef or Chicken
          <p>$19.99</p>
        </h3>
      </article>

      <article class="card">
        <img src="images/Other/Dubai-chocolate-recipe-19-scaled.jpg" alt="Dubai Chocolate">
        <h3>Rich and flaky Dubai Chocolate - Pistaccio flavored
          <p>$30.00</p>
        </h3>
      </article>

    </div>
</section>
------



//// Original css///

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

html {
  scroll-behavior: smooth;
}

.description {
  font-size: 0.9rem;
  margin-bottom: 10px;
}

.price {
  font-weight: bold;
  margin-bottom: 10px;
}

body {
  font:  1.2em sans-serif; /*New*/
  background: #fff8f3;
  color: #333;
  line-height: 1.6;
}

.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
  text-align: center;
  background-blend-mode: multiply;
  background-color: rgba(0,0,0,0.4);
}

.hero h1 {
  font-size: 3rem;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 8px 16px; /*12,24*/
  background: #e76f51;
  color: white;
  text-decoration: none;
  border-radius: 20px; /*30*/
}

section {
  padding: 60px 20px;
  text-align: center;
  max-width: 1200px;
  margin: 0 auto;
}

.grid {
  display: grid; /*flex;,grid*/
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
  justify-content: center;
  justify-items: center;
  flex-wrap: wrap;
  margin-top: auto;
}

.card {
  border: 1px solid #999999;
  border-radius: 10px;
  text-align: center;
  background: white;
  margin: 1em auto;
  padding: 20px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  max-width: 350px;
}

/*.card {
  border: 1px solid #999999;
  border-radius: 10px;
  display: grid;
  text-align: center;
  width: 100%;
  max-width: 350px;
  grid-gap: 20px;
  background: white;
  margin: 1em auto;
  padding: 20px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }
*/
.card img {
  width: 100%;
  border-radius: 8px;
  display: block;
  margin: 0 auto;
}

footer {
  padding: 20px;
  background: #e76f51;
  color: white;
}

.error-page {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.error-page h1 {
  font-size: 5rem;
  margin-bottom: 10px;
}

@media (max-width: 600px) {
  .card {
    padding: 12px;
    font-size: 14px;
  }
  
  .card img {
    height: 150px;
    object-fit: cover;
  }
}