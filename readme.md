# Web Application Development

## 2. Basic HTML

**HTML** is a **H**yper**T**ext **M**arkup **L**anguage

### Structure of an HTML Page

```html
<!DOCTYPE html>
<html>
  <head>
      information about the page
  </head>
  <body>
      page contents
  </body>
</html>
```

### Page title: `<title>`

Describes the title of the web page

```html
<title>Chapter 2: HTML Basics</title>
```

### Paragraph: `<p>`

```html
<p>You're not your job.
You're not how much money you have in the bank.
You're not the car you drive.   You're not the contents
of your wallet. You're not your         khakis.  You're
   the all-singing, all-dancing crap of the world.</p>
```

### Headings: `<h1>,<h2>,<h3>,,,<h6>`

headings to separate major areas of the page (block)

```html
<h1>University of Whoville</h1>
<h2>Department of Computer Science</h2>
<h3>Sponsored by Micro$oft</h3>
```

### Horizontal rule: `<hr>`

```html
<p>First paragraph</p>
<hr />
<p>Second paragraph</p>
```

### Links: `<a>`

```html
<p>
  Search 
  <a href="http://www.google.com/">Google</a> or our
  <a href="lectures.html">Lecture Notes</a>.
</p>
```

### Block & Inline

- Block Element: elements contain an entire large region of content
	- paragraphs
	- lists
	- table cells

- Inline Element: elements affect a small amount of content
	- bold text
	- code fragments
	- images
	- **must be nested inside a block element**

### Images: `<img>`

**HTML5** also requires an `alt` attribute describing the image

```html
<img src="images/gollum.jpg" alt="Gollum from LOTR" />
```
`title` attribute is an optional tooltip (*on ANY element*)
```html
<a href="http://theonering.net/">
  <img src="images/gandalf.jpg" alt="Gandalf from LOTR"
   title="You shall not pass!" />
</a>
```

### Line break: `<br>`

*Warning: Don't over-use br (guideline: >= 2 in a row is bad)*

```html
<p>Teddy said it was a hat, <br /> So I put it on.</p>
<p>Now Daddy's sayin', <br /> Where the
heck's the toilet plunger gone?</p>
```

### Phrase elements: `<em>, <strong>`

```html
<p>
  HTML is <em>really</em>,
  <strong>REALLY</strong> fun!
</p>
```

### Comments: `<!-- -->`

```html
<!-- My web page, by Suzy Student
     CSE3026, 2nd Semester 2025    -->
<p>CSE courses are <!-- NOT --> a lot of fun!</p>
```

### Unordered list: `<ul>, <li>`

```html
<ul>
  <li>No shoes</li>
  <li>No shirt</li>
  <li>No problem!</li>
</ul>
<!-- More List -->
<ul>
  <li>Simpsons:
    <ul>
      <li>Homer</li>
      <li>Marge</li>
    </ul>
  </li>
  <li>Family Guy:
    <ul>
      <li>Peter</li>
      <li>Lois</li>
    </ul>
  </li>
</ul>
```

### Ordered list: `<ol>`

```html
<p>RIAA business model:</p>
<ol>
  <li>Sue customers</li>
  <li>???</li>
  <li>Profit!</li>
</ol>
```

### Definition list: `<dl>, <dt>, <dd>`

```html
<dl>
  <dt>newbie</dt> <dd>one who does not have mad skills</dd>
  <dt>own</dt> <dd>to soundly defeat
    (e.g. I owned that newbie!)</dd>
  <dt>frag</dt> <dd>a kill in a shooting game</dd>
</dl>
```

### Quotations: `<blockquote>`

```html
<p>As Lincoln said in his famous Gettysburg Address:</p>
<blockquote>
  <p>Fourscore and seven years ago, our fathers brought forth
    on this continent a new nation, conceived in liberty, and
    dedicated to the proposition that all men are created equal.</p>
</blockquote>
```

### Inline quotations: `<q>`

```html
<p>Quoth the Raven, <q>Nevermore.</q></p>
```

### HTML Character Entities

```
< >	&lt; &gt;
é è ñ	&eacute; &egrave; &ntilde;
™ ©	&trade; &copy;
π δ Δ	&pi; &delta; &Delta;
И	&#1048;
" &	&quot; &amp;
```

### HTML-encoding text

```html
&lt;p&gt;
  &lt;a href=&quot;http://google.com/search?q=marty&amp;ie=utf-8&quot;&gt;
    Search Google for Marty
  &lt;/a&gt;
&lt;/p&gt;
```

### Deletions and insertions: `<del>, <ins>`

```html
<p>
  <del>Final Exam</del> <ins>Midterm</ins> is on 
  <del>Dec 10-15</del> <ins>Oct 10-11</ins>.
</p>
```

### Abbreviations: `<abbr>`

```html
<p>
  Safe divers always remember to check their
  <abbr title="Self-Contained Underwater Breathing Apparatus">SCUBA</abbr> gear.
</p>
```

### Computer code: `<code>`

```html
<p>
  The <code>ul</code> and <code>ol</code>
  tags make lists.
</p>
```

### Preformatted text: `<pre>`

```html
<pre>
     Steve Jobs speaks loudly
        reality distortion
       Apple fans bow down
</pre>
```

### Web page metadata: `<meta>`

```html
<meta charset="utf-8" />
<meta name="description"
    content="Authors' web site for Building Java Programs." />
<meta name="keywords" content="java, textbook" />
<meta http-equiv="refresh" content="10, www.naver.com">
<meta http-equiv="content-language" content="ko" />
```

### Favorites icon: `favicon`

```html
<link href="yahoo.gif" type="image/gif" rel="shortcut icon" />
```

### HTML tables: `<table>, <tr>, <td>`

```html
<table>
  <tr><td>1,1</td><td>1,2 okay</td></tr>
  <tr><td>2,1 real wide</td><td>2,2</td></tr>
</table>
```

### Table headers, captions: `<th>, <caption>`

```html
<table>
  <caption>My important data</caption>
  <tr><th>Column 1</th><th>Column 2</th></tr>
  <tr><td>1,1</td><td>1,2 okay</td></tr>
  <tr><td>2,1 real wide</td><td>2,2</td></tr>
</table>
```

### Linking to multimedia files

```html
<a href="video.avi">My video</a>
```
> MPG, MOV, WMV, RM, SWF, WAV, MID
> 

### HTML 5 embedding a video

```html
<video src="video.ogv" width="425" height="350"></video>
```

### Embedded objects: `<object>`

```html
<object data="video.avi" type="video/avi"></object>
```
> attributes: archive, classid, codebase, codetype, data, declare, height, name, standby, type, usemap, width
> 

### Parameters: `<param>`

```html
<object data="duckhunt.mp4" width="100" height="50">
  <param name="autoplay" value="true" />
</object>
```

### Embedding a Youtube video

```html
<iframe width="width" height="height" src="videoURL">
</iframe>
```

## 3. CSS for Styling

### Cascading Style Sheets (CSS): `<link>`

```html
<link href="style.css" type="text/css" rel="stylesheet" />
```

### CSS properties for colors

```css
p {
  color: red;
  background-color: yellow;
}
```

### Specifying colors

```css
p { color: red; }
h2 { color: rgb(128, 0, 196); }
h4 { color: #FF8800; }
```

### font-family

```css
p {
  font-family: Georgia;
}
h2 {
  font-family: "Courier New";
}
```

### More about font-family

```css
p {
  font-family: Garamond, "Times New Roman", serif;
}
```

### font-size

```css
p {
  font-size: 14pt;
}
```

### font-weight, font-style

```css
p {
  font-weight: bold;
  font-style: italic;
}
```

### font

```css
p {
  font: italic bold 14px "Arial", cursive;
}
```

### CSS comments: /* ... */

```css
/* This is a comment.
  It can span many lines in the CSS file. */
p {
  color: red;
  background-color: aqua;
}
```

### CSS properties for text

```css
/* left, right, center, or justify */
blockquote { text-align: justify; }
h2 { text-align: center; }
/* overline, line-through, blink, or none */
p {
  text-decoration: underline;
}
/* text-shadow */
p {
  font-weight: bold;
  text-shadow: -2px 5px gray;
}
```

### CSS properties for backgrounds

```css
body {
  background-image: url("images/draft.jpg");
  background-repeat: no-repeat;
  background-position: 370px 20px;
}
```

### The list-style-type property

```css
ol { list-style-type: lower-roman; }
```

### Styling tables

```css
table { border: 2px solid black; caption-side: bottom; }
tr { font-style: italic; }
td { background-color: yellow; text-align: center; width: 30%; }
```

### The border-collapse property

```css
table, td, th { border: 2px solid black; }
table { border-collapse: collapse; }
```

### The rowspan and colspan attributes

```html
<table>
  <tr><th>Column 1</th><th>Column 2</th><th>Column 3</th></tr>
  <tr><td colspan="2">1,1-1,2</td>
    <td rowspan="3">1,3-3,3</td></tr>
  <tr><td>2,1</td><td>2,2</td></tr>
  <tr><td>3,1</td><td>3,2</td></tr>
</table>
```

### Column styles: `<col>, <colgroup>`

```html
<table>
  <col class="urgent" />
  <colgroup class="highlight" span="2"></colgroup>
    
  <tr><th>Column 1</th><th>Column 2</th><th>Column 3</th></tr>
  <tr><td>1,1</td><td>1,2</td><td>1,3</td></tr>
  <tr><td>2,1</td><td>2,2</td><td>2,3</td></tr>
</table>
```

### CSS pseudo-classes

```css
a:link    { color: #FF0000; }      /* unvisited link */
a:visited { color: #00FF00; }      /* visited link */
a:hover   { color: #FF00FF; }      /* mouse over link */
```

## Page Layout

### CSS context selectors

```
selector1 selector2 {
  properties
}
```
- applies the given properties to selector2 only if it is inside a selector1 on the page

```
selector1 > selector2 {
  properties
}
```
- applies the given properties to selector2 only if it is directly inside a selector1 on the page (selector2 tag is immediately inside selector1 with no tags in between)
