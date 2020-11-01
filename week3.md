## DAY 11 OF PROGRAMMING 10/26/20

## Python

---

### Things we worked on:

1. First half, worked on python projects
2. After lunch, present projects

---

## DAY 12 OF PROGRAMMING 10/27/20

## HTML

---

### Things we worked on:

1. html tags
2. html nested tags
3. html attributes

---

```
-Use <em>To emphasize</em> instead of i
-Use <strong>To bold</strong> instead of bold
--
- id can't have the same name
- classes can have the same name

### Attributes
- href
- src
```

## HTML TAGS

-   HTML - Html is an acronym for Hypertext Markup Language. It is a language
    that only describes the stucture and provided content of a document. All websites are creating using HTML
-   Symantic HTML - symantic HTML is concenpt where the html document is written in a way where each tag has meaning and purpose and tags are not used to change the layout or look of a page
-   HTML Element - The actualy item that the tag represents is the html element

```
  <!-- HTML Comment -->
  <div> Content </div>
```

```
  <!-- HTML doesn't care about spaces for the most part -->
  <div>
      Content
      Is spaced
      But not on the page

```

```
 Common HTML tags

  <div> content </div>
  <span> content </span>
  <h1> Heading 1 </h1>
  <h2> Heading 2 </h2>
  <!-- down to heading h6 -->
  <p> Paragraph content </p>
  <section> Sectional Content </section>
```

## HTML NESTED TAGS

---

-   Nest HTML tags
-   Some tags need nesting
-   Gotchas
-   Exercise

```
 <!-- simple nesting -->
  <div>
      <p>
          I am some content
      </p>
      <p>
          I am more content
      </p>
  </div>

```

```
  <!-- Deep level nesting -->
  <div>
      <section>
          <p>
              Things are good today.
              <span>
                  Really Good!
              </span>
          </p>
      </section>
  </div>

```

```
- Some tags need to be nested

<ul>
      <li> Peas</li>
      <li>Carrots </li>
      <li>Potatoes </li>
  </ul>

  <table>
      <tr>
          <td> Peas</td>
          <td> Carrots</td>
          <td> Potatoes</td>
      </tr>
      <tr>
          <td>Ice Cream</td>
          <td>Pancakes</td>
          <td>Baklava</td>
      </tr>
  </table>

```

```
- GOTCHAS

  <!-- opening and closing tags mixed up -->
  <div>
      <p>
          <span>
          Some content to use
      </p>
          </span>
  </div>

- BAD PRACTICES

  <!-- bad practices -->
  <!-- Using hr to draw line is not symantic -->
  <hr />
  <hr />
  <hr />

  <b>B is bold. IT is not symantic but is a style. HTML is not supposed to use style</b>
  <i> Like B I means itallic. HTML is not supposed to represent style.</i>

```

---

# HTML ATTRIBUTES

---

HTML Attribute - HTML attributes are special words inside of tags that can modifiy the tags behavior or help identify the tag.

## What is a HTML attribute

---

```
  <!-- The 'href' is the attribute -->
  <a href="http://google.com">Goto Google</a>
  <!-- 'src' is the attribute -->
  <img src="kittens.jpg" />

```

```
Most attributes are to be used with a specific tag only. If added to tags that do not deal with that attribute they will be ignored.

  <a href="http://google.com" id="first-link" class="nav-link" >
  Google</a>
  <!-- Each tag can have multiple attributes. Order does not matter. -->

```

## Common Attributes

---

```
  <div id="main-content">Main Content</div>
  <!-- hyphen case is the standard, but not required, for id and class names -->
  <section class="side-content">
      Here is some side content
  </section>

```

## DAY 13 OF PROGRAMMING 10/28/20

---

### Things we worked on:

1. CSS basic
2. CSS Specificity
3. CSS Box Model
4. CSS position
5. Flex box

---

```
/* CSS comment*/

  /* Rule (or ruleset) breakdown */
  selector
  { /* Declaration Block Start  */
      property1:value1; /* <- Declaration */
      property2:value2 value2a value2b;
  }/* Declaration Block End    */

```

## Understanding Inheritance

```
    <style>
          /* Sets the font family */
          body {
              font-family: Arial, Helvetica, sans-serif;
          }
          /* sets background for all 'a's */
          a {
              text-decoration: none;
          }
          /* sets the font-famly for all 'div's */
          div {
              font-family: 'Courier New', Courier, monospace;
          }
          /* makes nav-links bold */
          .nav-link {
              font-weight:bold;
          }
          /* makes active class silver and underline */
          .active {
              background:silver;
          }
      </style>
      <h2>Star Wars Links</h2>
      <div id="navbar">
          <a href="#" class="nav-link">Yoda Facts</a>
          <a href="#" class="nav-link">Han Facts</a>
          <a href="#" class="nav-link active">Jar Jar Facts</a>
      </div>

```

## Using Specificity

---

```
  <style>
  ...
  /* psudo class is more specific than class */
  .nav-link:first-child {
      background:green;
      text-decoration:underline;
  }
  ...
  </style>
```

## Using Combinators

---

```
 <style>
  ...
  /* coma seperates individual selectors */
  h2, h3 {
      background:#efefef;
      border-bottom:3px solid;
  }
  /* spaces indicate parent -> child */
  .main-content .active {
      background:red;
      border: 1px solid #000;
  }
  /* no spaces means has both I all a elements with active class */
  a.active {
      color:green;
      font-weight:bold;
  }

  ...
  </style>
  <body>
  ...
      <div id="content">
          <h3>Mesa Jar Jar Binks</h3>
          <p class="active">mesa your humble servant!</p>
          <p>Yousa should follow me now, okeeday?</p>
      </div>
  </body>
```

# Box model

-   Explain the Box Model
    [hackernoon](https://hackernoon.com/hn-images/1*2jZwpWH9XO_QllhEpyGqMA.png)

```
/* top, right, bottom, left */
  div {
      padding:10px, 20px, 2px, 6px;
  }

  /* top & bottom, left & right */
  span {
      margin: 1em,3em;
  }

  /* all */
  .random-selector {
      padding:50px;
      margin:10px;
  }

  /* size, style, color */
  div:hover {
      border: 4px double red;
  }

  /* height and width */
  a {
      width:50%;
      height:30px;
  }
```

Padding contains the background margin is outside of the background. Think of margin seperating the elements while padding makes the element bigger.

## CSS Position

---

```
<!-- static position is default -->
  <style>
      .item {
          position:static;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item"> Statically positioned </p>
  </div>
  <!-- relative position works like static, but can be moved with othe declerations -->
  <style>
      .item {
          position:relative;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item"> relativly positioned </p>
  </div>
```

```
<!-- absolute position completly takes the element out of the flow -->
  <style>
      .item {
          position:absolute;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item"> relativly positioned </p>
  </div>
```

```
<!-- fixed is like absolute but is based o nthe screen and not document position -->
  <style>
      .item {
          position:fixed;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item"> fixed positioned </p>
  </div>

```

```
<!-- fixed is like absolute but is based o nthe screen and not document position -->
  <style>
      .item {
          position:sticky;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item"> Sticky positioned </p>
  </div>
```

# Top, Right, Bottom, Left

```
 <style>
      .item1 {
          position:relative;
          top:10px;
      }
      .item2 {
          position:absolute;
          right:10px;
          bottom:20px;
      }
      .item3 {
          position:fixed;
          left:30px;
          top:20px;
      }
      .item4 {
          position:sticky;
          left:30px;
          top:20px;
      }
  </style>
  <div>
      <h1>Title</h1>
      <p class="item1"> relativly positioned </p>
      <p class="item2"> absolute positioned </p>
      <p class="item3"> fixed positioned </p>
      <p class="item4"> sticky positioned </p>
  </div>
```

## CSS Flexbox

---

-   Using Flexbox

```
<style>
      .container {
          display:flex;
      }
  </style>

  <div class="container">
      <div> Item 1</div>
      <div> Item 2</div>
      <div> Item 3</div>
      <div> Item 4</div>
  </div>
```

-   Simple Examples

```
<!-- non-flexbox way -->
  <!-- have to keep changing the size, not really responsive -->
  <style>
      .container {
          width:400px;
      }
      .container div{
          width:50px;
          display: inline-block;
          padding:10px;
          border:1px solid;
          margin:6px;
          text-align:center;
      }
  </style>
  <!-- using the div with the 4 items -->
```

```
<!-- flexbox way -->
  <style>
      .container {
          width:400px;
          display:flex;
      }
      .container div{
          width:100%;
          padding:10px;
          border:1px solid;
          margin:6px;
          text-align:center;
      }
  </style>

```

```
  <!-- flex justify-content can change the positions -->
  <style>
   .container {
          width:400px;
          display:flex;
          justify-content: space-between;

      }
      .container div{
          width:40px;
          padding:10px;
          border:1px solid;
          margin:6px;
          text-align:center;
      }
  </style>
```

```
 <!-- flex wrap is really helpful for responsivenes -->
  <style>
      .container {
          width:400px;
          display:flex;
          flex-wrap: wrap;
      }
      .container div{
          width:120px;
          padding:10px;
          border:1px solid;
          margin:6px;
          text-align:center;
      }
  </style>
  <div class="container">
      <div>
          <p>Item 1</p>
          <p>
              Non veniam tempor esse Lorem amet
              Lorem incididunt duis mollit dolor aute
              ad adipisicing duis.
          </p>
      </div>
  ...
  </div>
```

## DAY 14 OF PROGRAMMING 10/29/20

---

### Things we worked on:

1. Using External CSS Libraries
2.
3.

---

-   Library - In software developement a library is a bit of code that is used to preform specific tasks.
-   Framework - In software development a Framework is software that provides a default functionality and it's own standardization for a project.
-   CDN - Content Delivery Network is a way to host software on the internet to be usable by the public

### How to use a CSS Library / framework

```
  <head>
  ...
  <!-- downloaded -->
  <link rel="stylesheet" href="/library-folder/library.css">
  <!-- "/library-folder/library.css" would be replaced with the folder and file name -->
  ...

  <!-- cdn -->
  <link rel="stylesheet" href="https://cdn-network.com/library-name/library-file.css">
  <!-- again the href will be changed with the library's cdn -->
  ...

  <!-- framework with javascript -->
  <link rel="stylesheet" href="https://cdn-network.com/library-name/library-file.css">
  <script src="https://cdn-network.com/library-name/library-file.js">
  ...

     <!-- adding custom css along with library or framework -->
  <link rel="stylesheet" href="https://cdn-network.com/library-name/library-file.css">
  <link rel="stylesheet" href="/styles/my-styles.css">
  ...


```

---

How To read the docs

RETU - Read, Explorer, Try/Test, Understand
Quickly read over the website or readme if it has one to see if you can even use the library. Get a cursery view of how the library works.
Explore the various things the library does. Find some things that can help your project.
Test out a few things. Make sure the docs work the way the library says it does. Make a sample file and just do some of the things the docs say.
Before diving fully into library and dedicating a lot of time with it, look over the code on github and see if you can understand how it works. It is not required to fully understand it (especially with large frameworks) but it is always best to understand tools your are using.

---

Examples

Libraries

http://kazzkiq.github.io/balloon.css/
https://bttn.surge.sh/
http://necolas.github.io/normalize.css/
https://github.com/kognise/water.css
Frameworks

https://getbootstrap.com/
https://bulma.io/
https://purecss.io/
https://materializecss.com/

---

# CSS resources

---

-   (https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)

-   (https://flexboxzombies.com/p/flexbox-zombies)

-   (https://alistapart.com/article/holygrail/)

---

## DAY 15 OF PROGRAMMING 10/30/20

---

### Things we worked on:

1. Algorithm exercises
2. Worked on our HTML/CSS project

---

## DAY 11 OF PROGRAMMING 10/21/20

---

### Things we worked on:

1.
2.
3.

---
