# class 1 HTML intro

abbreviation…uses to define an abbreviation or acronym 

```html
<abbr tittle="hyper text markup language">HTML</abbr>
```

icon…to add icon 

```html
<i>Arrow</i>
```

action….defines the action to be performed when the form is submitted

```html
<form action="/action-page.php"></form>
```

target…..specifies where to display the response that is received after submitting the form

```html
<form action="/action_page.php" target="_blank">
```

post message….used to post a message back to the html page 

```jsx
function timedCount() {
  i = i + 1;
  postMessage(i);
  setTimeout("timedCount()",500);
}
```

iframe….to brink contents from other resources 

```html
<iframe src="url" title="description"></iframe>
```

aside…..defines content aside form the content

```html
<aside>school</aside>
```

blockquote….defines a section that is quoted from another source 

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. 
As the world's leading conservation organization, WWF works in nearly 100 countries.
 At every level, we collaborate with people around the world to develop and deliver 
innovative solutions that protect communities, wildlife, and the places in which they 
live.
</blockquote>
```

[forms](class%201%20HTML%20intro%2004f5a6e088ef441f95adc78af8f23b8b/forms%20d5159a48da6241fcba1a20034fa3c48b.md)

`<picture>` element allows you to define different images for different browser window sizes.

```html
<picture>
<source srcset="img_smallflower.jpg" media="(max-width: 600px)">
</picture>
```

`<cite>` tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.)

```jsx
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

`<bdo>` tag is used to override the current text direction:

```jsx
<bdo dir="rtl">This text will be written from right to left</bdo>
```

"_blank" to open the linked document in a new browser window or tab:

```html
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```

Use `mailto:` inside the `href` attribute to create a link that opens the user's email program (to let them send a new email):

```html
<a href="mailto:someone@example.com">Send email</a>
```

The `<fieldset>` tag is used to group related elements in a form.

```html
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label>
    <input type="text" id="fname" name="fname"><br><br>
    <label for="lname">Last name:</label>
    <input type="text" id="lname" name="lname"><br><br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br><br>
    <label for="birthday">Birthday:</label>
    <input type="date" id="birthday" name="birthday"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

The `<canvas>` tag is used to draw graphics, on the fly, via scripting (usually JavaScript).

```html
<canvas id="myCanvas">
Your browser does not support the canvas tag.
</canvas>
```

 **`<address>` (Semantic Address Tag):**

- **Purpose:** Defines contact information for the author or owner of the document.
- **Example:** `<address>John Doe, 123 Main Street, Anytown, CA 12345, john.doe@example.com</address>`
- **Note:** Replaced by `<p>` with `class="address"` in modern HTML, but still valid.

**`<abbr>` (Abbreviation Tag):**

- **Purpose:** Defines an abbreviation and provides its full form as a tooltip.
- **Example:** `<abbr title="HyperText Markup Language">HTML</abbr>`
- **Note:** Less commonly used than `<title>` attribute with `<span>`.

**`<cite>` (Citation Tag):**

- **Purpose:** Defines a title of a creative work (book, article, song).
- **Example:** `<cite>The Lord of the Rings</cite> by J.R.R. Tolkien`
- **Note:** Can be replaced by `<blockquote>` with attribution.

**`<dfn>` (Definition Tag):**

- **Purpose:** Defines a term within the document text.
- **Example:** `<dfn>Algorithm</dfn>: A set of instructions for solving a problem.`
- **Note:** Often used with the `<glossary>` tag for a list of definitions.

**`<del>` (Deleted Text Tag):**

- **Purpose:** Indicates text that has been removed from the document.
- **Example:** `<del>This text is no longer relevant.</del>`
- **Note:** Replaced by `<strike>` in modern HTML, but still valid.

**`<ins>` (Inserted Text Tag):**

- **Purpose:** Indicates text that has been added to the document.
- **Example:** `<ins>This text has been added for clarification.</ins>`
- **Note:** Replaced by `<span>` with `class="inserted"` in modern HTML, but still valid.

**`<q>` (Inline Quote Tag):**

- **Purpose:** Indicates a short inline quotation.
- **Example:** `<q>The early bird gets the worm.</q>`
- **Note:** Often replaced by double quotes (`"`) or the `<blockquote>` tag.

 **`<rp>` (Replacement Character Tag):**

- **Purpose:** Indicates a character that has been replaced.
- **Example:** `<rp>The original text was "hello", but it has been replaced with "goodbye".</rp>`
- **Note:** Rarely used and often replaced with other methods like footnotes or annotations.

 **`<rt>` (Ruby Text Tag):**

- **Purpose:** Displays text above the current line, often used for phonetic pronunciation or annotations.
- **Example:** `<rt>café</rt>` (pronounced "kah-fay")
- **Note:** Rarely used and browser support varies; consider using other methods like superscript (`<sup>`).

**`<samp>` (Sample Output Tag):**

- **Purpose:** Displays sample computer output.
- **Example:** `<samp>$ ls -l</samp>`
- **Note:** Replaced by `<pre>` with `class="sample"` in modern HTML, but still valid.