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