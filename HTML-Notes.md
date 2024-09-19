# HTML-Notes
---
```markdown
# HTML - HyperText Markup Language

HTML (HyperText Markup Language) is the standard markup language used to create web pages. It defines the structure and content of a web document. HTML uses elements and tags to represent the content and its structure.
```

## Flow of HTML

The general structure of an HTML document follows a standard flow:

```
<!DOCTYPE html>    <!-- Declaration of the document type -->
<html lang="en">    <!-- Root element, setting language as English -->

  <head>           <!-- Meta information about the document -->
    <title>Page Title</title>  <!-- Title displayed in the browser tab -->
  </head>

  <body>           <!-- Content visible on the web page -->
    <!-- Your content here -->
  </body>

</html>
```

### Example of HTML Document Flow:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Sample Page</title>
  </head>
  <body>
    <h1>Welcome to HTML</h1>
    <p>This is a paragraph explaining HTML structure.</p>
  </body>
</html>
```



## Common HTML Tags

### Headings
HTML provides six levels of headings, from `<h1>` (largest) to `<h6>` (smallest).
```html
<h1>This is an H1 heading</h1>
<h2>This is an H2 heading</h2>
<h3>This is an H3 heading</h3>
<h4>This is an H4 heading</h4>
<h5>This is an H5 heading</h5>
<h6>This is an H6 heading</h6>
```

### The Paragraph Tag `<p>`
The `<p>` tag is used for paragraphs.
```html
<p>This is a paragraph of text in HTML.</p>
```

### The Horizontal Line Tag `<hr>`
The `<hr>` tag is used to create a thematic break or horizontal line.
```html
<hr>
```

### The Line Break Tag `<br>`
The tag is used to insert a line break.
```html
<p>This is a paragraph with a line break.<br>This is the next line.</p>
```





### The Comment Tag `<!--   -->`
HTML comments are used to add notes or explanations within the code, which are not displayed in the browser.
```html
<!-- This is a comment and won't be visible on the webpage -->
```

## Text Styling  

### `<strong>` Tag
Defines text with strong importance, typically displayed in **bold**.

**Syntax:**
```html
<strong>This is important text (bold)</strong>
```

---

### `<em>` Tag
Defines emphasized text, typically displayed in *italic*.

**Syntax:**
```html
<em>This is emphasized text (italic)</em>
```

---

### `<u>` Tag
Underlines the text.

**Syntax:**
```html
<u>This text is underlined</u>
```

---

### `<s>` Tag
Strikes through the text, indicating something no longer accurate or relevant.

**Syntax:**
```html
<s>This text is struck through</s>
```

---

### `<sub>` Tag
Creates subscript text (lowered text, often used in scientific notation).

**Syntax:**
```html
H<sub>2</sub>O (subscript for chemical formula)
```

---

### `<sup>` Tag
Creates superscript text (raised text, often used for exponents or footnotes).

**Syntax:**
```html
X<sup>2</sup> (superscript for exponent)
```

---

### `<pre>` Tag
Preserves white spaces and displays text in a fixed-width font.

**Syntax:**
```html
<pre>
This is preformatted text.
    Spaces and
line breaks are preserved.
</pre>
```

---

### `<kbd>` Tag
Represents keyboard input.

**Syntax:**
```html
<kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text.
```

---

### `<abbr>` Tag
Defines an abbreviation or acronym, with an optional `title` attribute for expanded meaning.

**Syntax:**
```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

---

### `<mark>` Tag
Highlights the text, often used to indicate important content.

**Syntax:**
```html
<mark>This text is highlighted</mark>
```

---

### `<small>` Tag
Renders text in a smaller font size.

**Syntax:**
```html
<small>This text is smaller</small>
```

---

### `<del>` Tag
Displays text that has been deleted or is no longer relevant, typically shown with a strikethrough.

**Syntax:**
```html
<del>This text is deleted</del>
```

---
### The Anchor Tag `<a>`


The `<a>` tag is used to create hyperlinks in HTML, allowing users to navigate from one page to another. It can link to internal pages, external websites, or even specific sections within a page.

### Basic Syntax
```html
<a href="URL">Link Text</a>
```

### Example:
```html
<a href="https://www.example.com">Visit Example Website</a>
```

---

### Common Attributes of the `<a>` Tag

#### 1. `href` (Hypertext Reference)
The `href` attribute specifies the URL of the page or resource the link points to.
```html
<a href="https://www.example.com">Example</a>
```

#### 2. `target`
The `target` attribute defines where the linked document will open. The most common values are:
- `_self` (default): Opens in the same tab.
- `_blank`: Opens in a new tab or window.
- `_parent`: Opens in the parent frame.
- `_top`: Opens in the full body of the window.

```html
<a href="https://www.example.com" target="_blank">Open in New Tab</a>
```

#### 3. `download`
The `download` attribute allows users to download the linked file rather than navigate to it. It can specify a custom filename for the download.

```html
<a href="file.pdf" download="custom_filename.pdf">Download PDF</a>
```

#### 4. `rel`
The `rel` attribute specifies the relationship between the current page and the linked resource. It is often used to define behaviors or improve security:
- `noopener`: Prevents the new page from controlling the opening page.
- `noreferrer`: Removes the referrer information when navigating to the link.
- `nofollow`: Tells search engines not to follow the link.

```html
<a href="https://www.example.com" target="_blank" rel="noopener noreferrer">Secure External Link</a>
```

#### 5. `title`
The `title` attribute provides additional information about the link. When the user hovers over the link, the title text appears as a tooltip.

```html
<a href="https://www.example.com" title="Click to visit Example">Example with Tooltip</a>
```

---

#### Additional Attributes

##### `type`
The `type` attribute can specify the MIME type of the resource being linked to. This helps browsers understand how to handle the linked content.
```html
<a href="https://www.example.com" type="text/html">HTML Link</a>
```

#### `hreflang`
The `hreflang` attribute specifies the language of the linked resource. This can help with SEO and accessibility.
```html
<a href="https://www.example.com" hreflang="en">Link to English Page</a>
```
#### Complete Example:
```html
<a href="https://www.example.com" target="_blank" rel="noopener noreferrer" title="Example Website">Visit Example</a>
```

---

### The Embed Tag `<embed>`
The `<embed>` tag is used to embed external content, like PDFs, videos, or audio files.

**Syntax:**
```html
<embed src="file.pdf" type="application/pdf" width="600" height="400">
```

---

### The link Tag `<link>`
The `<link>` tag defines the relationship between the current document and an external resource, often used for stylesheets.

**Syntax:**
```html
<link rel="stylesheet" href="styles.css">
```

---

### The Source Tag `<source>`
The `<source>` tag specifies multiple media resources for media elements like `<video>` or `<audio>`.

**Syntax (for video):**
```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

---

### The Track Tag `<track>`
The `<track>` tag is used to specify text tracks for media elements like `<video>` and `<audio>` (such as subtitles or captions).

**Syntax:**
```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <track src="subtitles_en.vtt" kind="subtitles" srclang="en" label="English">
</video>
```

---

### The Wordbreak Tag `<wbr>`
The `<wbr>` tag defines a possible line break point. It can suggest places for the browser to break the text without hyphenating words.

**Syntax:**
```html
<p>This is a very long text, but I can insert a<wbr>line break here.</p>
```

---


### The Input Tag `<input>`
The `<input>` tag is used to create input fields in forms. It can be of different types, such as `text`, `password`, `checkbox`, `radio`, `submit`, etc.

**Syntax:**
```html
<input type="text" name="username" placeholder="Enter your username">
```

---

### The Column Tag `<col>`
The `<col>` tag defines attributes for columns within a `<table>` element.

**Syntax:**
```html
<table>
  <colgroup>
    <col span="1" style="background-color:yellow">
    <col span="1" style="background-color:lightblue">
  </colgroup>
  <tr>
    <td>Column 1</td>
    <td>Column 2</td>
  </tr>
</table>
```
---
###  The Picture Tag `<picture>`
The `<picture>` tag is used for responsive images. It allows you to specify multiple image sources for different screen sizes or media types, offering more control over which image is displayed.

**Syntax:**
```html
<picture>
  <source srcset="image-small.jpg" media="(max-width: 600px)" type="image/webp">
  <source srcset="image-large.jpg" media="(min-width: 601px)"type="image/jpeg">
  <img src="fallback-image.jpg" alt="A descriptive alternative text">
</picture>
```

- **`srcset`**: Specifies the image to use based on the device's resolution or media query.
- **`media`**: Defines the conditions (like screen width) under which a specific image should be loaded.
- **`type`**: Specifies the image format (e.g., `image/jpeg`, `image/webp`).
---

### The Figure `<figure>` and The Figure caption`<figcaption>` Tags
The `<figure>` tag is used to group media elements (like images, videos, or diagrams) with their captions. The `<figcaption>` tag is used to define the caption for the media content.

**Syntax:**
```html
<figure>
  <img src="image.jpg" alt="A descriptive alternative text">
  <figcaption>This is the caption describing the image.</figcaption>
</figure>
```

- **`<figure>`**: Groups media content and its caption.
- **`<figcaption>`**: Provides a description or caption for the media content.

---

##### Complete Example:
```html
<figure>
  <img src="sunset.jpg" alt="A beautiful sunset over the mountains">
  <figcaption>The sun setting behind the mountains on a summer evening.</figcaption>
</figure>
```

## HTML Lists

### `<ol>` (Ordered List)
The `<ol>` tag is used to create an ordered list, where the list items are automatically numbered. You can control the type of numbering using the `list-style-type` CSS property.

**Syntax:**
```html
<ol style="list-style-type: decimal;">
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

---

### List Style Types for `<ol>`
You can use the following values for the `list-style-type` in ordered lists:

- **decimal**: Default numbering (1, 2, 3, ...)
- **lower-alpha**: Lowercase letters (a, b, c, ...)
- **upper-alpha**: Uppercase letters (A, B, C, ...)
- **lower-roman**: Lowercase Roman numerals (i, ii, iii, ...)
- **upper-roman**: Uppercase Roman numerals (I, II, III, ...)

**Examples:**
```html
<ol style="list-style-type: lower-alpha;">
  <li>Item a</li>
  <li>Item b</li>
  <li>Item c</li>
</ol>

<ol style="list-style-type: upper-roman;">
  <li>Item I</li>
  <li>Item II</li>
  <li>Item III</li>
</ol>
```

---

### `<ul>` (Unordered List)
The `<ul>` tag is used to create unordered lists, where the list items are marked with bullets by default. You can control the type of bullets using the `list-style-type` CSS property.

**Syntax:**
```html
<ul style="list-style-type: disc;">
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ul>
```

---

### List Style Types for `<ul>`
You can use the following values for the `list-style-type` in unordered lists:

- **disc**: Default bullet (•)
- **circle**: Hollow circle (○)
- **square**: Square bullet (■)
- **none**: No bullet

**Examples:**
```html
<ul style="list-style-type: circle;">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<ul style="list-style-type: square;">
  <li>Square bullet item 1</li>
  <li>Square bullet item 2</li>
</ul>
```

---

### Nested Lists
You can create nested lists by placing one list inside another. Both ordered and unordered lists can be nested.

**Syntax/ Nested List Example::**
```html
<ol>
  <li>Item 1
    <ul style="list-style-type: square;">
      <li>Nested item 1.1</li>
      <li>Nested item 1.2</li>
    </ul>
  </li>
  <li>Item 2
    <ol style="list-style-type: lower-roman;">
      <li>Nested item ii</li>
      <li>Nested item iii</li>
    </ol>
  </li>
</ol>
```

This structure allows for combining ordered and unordered lists within one another, creating a hierarchical list.

### List Attributes

#### `start`
The `start` attribute specifies the starting number for the first list item in an ordered list. By default, the list starts with 1.

**Syntax:**
```html
<ol start="5">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>

```

## HTML Table Tags

### The Table Tag `<table>`
The `<table>` tag is used to create a table in HTML.

**Syntax:**
```html
<table>
  <!-- Table content goes here -->
</table>
```

---

### `<thead>`, `<tbody>`, and `<tfoot>` Tags
- **`<thead>`**: Defines the table header.
- **`<tbody>`**: Defines the body content of the table.
- **`<tfoot>`**: Defines the table footer (optional).

**Syntax:**
```html
<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Cell 1</td>
      <td>Row 1, Cell 2</td>
    </tr>
    <tr>
      <td>Row 2, Cell 1</td>
      <td>Row 2, Cell 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer 1</td>
      <td>Footer 2</td>
    </tr>
  </tfoot>
</table>
```

---

### The Table Head Tag `<th>`
The `<th>` tag defines a header cell in a table, which is typically displayed in bold and centered.

**Syntax:**
```html
<th>Header Cell</th>
```

---

### The Table Data Tag `<td>`
The `<td>` tag defines a standard cell in a table (data cell).

**Syntax:**
```html
<td>Table Cell</td>
```

---

### The Table Row Tag `<tr>`
The `<tr>` tag defines a table row. It can contain `<th>` (header) or `<td>` (data) cells.

**Syntax:**
```html
<tr>
  <td>Cell 1</td>
  <td>Cell 2</td>
</tr>
```

---

### `colspan` Attribute
The `colspan` attribute allows a cell to span across multiple columns.

**Syntax:**
```html
<td colspan="2">This cell spans 2 columns</td>
```

**Example:**
```html
<table>
  <tr>
    <td colspan="2">Spanning two columns</td>
  </tr>
  <tr>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
</table>
```

---

### `rowspan` Attribute
The `rowspan` attribute allows a cell to span across multiple rows.

**Syntax:**
```html
<td rowspan="2">This cell spans 2 rows</td>
```

**Example:**
```html
<table>
  <tr>
    <td rowspan="2">Spanning two rows</td>
    <td>Cell 1</td>
  </tr>
  <tr>
    <td>Cell 2</td>
  </tr>
</table>
```

---

### Complete Table Example:
```html
<table border="1">
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2">Rowspan Cell</td>
      <td>Row 1, Cell 2</td>
    </tr>
    <tr>
      <td>Row 2, Cell 2</td>
    </tr>
    <tr>
      <td colspan="2">Colspan Cell</td>
    </tr>
  </tbody>
</table>
```

## HTML Media Tags


### The Image Tag `<img>`
The `<img>` tag is used to embed images in an HTML page.

- `src`: Specifies the image source URL.
- `alt`: Provides alternative text for the image if it cannot be displayed.

**Syntax:**
```html
<img src="image.jpg" alt="Description of the image">
```

---

### Link Inside `<img>` Tag
You can wrap an image in an `<a>` tag to make it a clickable link.

**Syntax:**
```html
<a href="https://www.example.com">
  <img src="image.jpg" alt="Clickable Image">
</a>
```

---

### `<iframe>` Tag
The `<iframe>` tag is used to embed another HTML page or content inside the current page.

- **`src`**: Specifies the URL of the page to embed.
- **`title`**: Provides a brief description of the embedded content for accessibility.

**Syntax:**
```html
<iframe src="https://www.example.com" title="Embedded Example"></iframe>
```

---

### The Audio Tag `<audio>`
The `<audio>` tag is used to embed audio files. It can include multiple `<source>` elements to specify different audio formats.

**Attributes:**
- **`controls`**: Displays audio controls like play, pause, and volume.
- **`autoplay`**: Automatically starts playing the audio.
- **`loop`**: Repeats the audio once it ends.
- **`preload`**: Specifies whether the audio file should be loaded when the page loads. Values: `auto`, `metadata`, or `none`.
- **`muted`**: Mutes the audio by default.

**Syntax:**
```html
<audio controls autoplay loop preload="auto" muted>
  <source src="audio-file.mp3" type="audio/mpeg">
  <source src="audio-file.ogg" type="audio/ogg">
  Your browser does not support the audio tag.
</audio>
```

---

### The Video Tag `<video>`
The `<video>` tag is used to embed video files, similar to the `<audio>` tag. It can contain multiple `<source>` elements for different video formats.

**Attributes:**
- **`controls`**: Displays video controls like play, pause, and volume.
- **`autoplay`**: Automatically starts playing the video.
- **`loop`**: Repeats the video once it ends.
- **`preload`**: Specifies if the video should be loaded when the page loads. Values: `auto`, `metadata`, or `none`.
- **`poster`**: Specifies an image to show while the video is downloading or until the user hits play.
- **`muted`**: Mutes the video by default.

**Syntax:**
```html
<video controls autoplay loop preload="auto" poster="thumbnail.jpg" muted>
  <source src="video-file.mp4" type="video/mp4">
  <source src="video-file.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

---



### The Form Tag `<form>`
The `<form>` tag is used to create an HTML form for user input. Forms can contain various input elements such as text fields, checkboxes, radio buttons, submit buttons, etc.

**Syntax:**
```html
<form action="submit.php" method="POST">
  <!-- Form elements go here -->
</form>
```

---

### Form Input Elements

#### `<input>` Tag
The `<input>` tag is one of the most commonly used form elements. It can represent various types of inputs based on the `type` attribute.

1. **Text Input**:
    ```html
    <label for="username">Enter Username:</label>
    <input type="text" id="username" name="username" placeholder="Username" required />
    ```

2. **Password Input**:
    ```html
    <label for="password">Password:</label>
    <input type="password" id="password" name="password" required />
    ```

3. **Email Input**:
    ```html
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required />
    ```

4. **Number Input**:
    ```html
    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="18" max="100" value="25" />
    ```

5. **Radio Button**:
    ```html
    <label for="gender">Gender:</label>
    <input type="radio" id="male" name="gender" value="Male"> Male
    <input type="radio" id="female" name="gender" value="Female"> Female
    ```

6. **Checkbox**:
    ```html
    <label for="subscribe">Subscribe:</label>
    <input type="checkbox" id="subscribe" name="subscribe" value="Yes" />
    ```

7. **File Upload**:
    ```html
    <label for="fileUpload">Select file:</label>
    <input type="file" id="fileUpload" name="fileUpload" />
    ```

8. **Date Input**:
    ```html
    <label for="birthdate">Birthdate:</label>
    <input type="date" id="birthdate" name="birthdate" />
    ```

9. **Time Input**:
    ```html
    <label for="appointmentTime">Appointment Time:</label>
    <input type="time" id="appointmentTime" name="appointmentTime" />
    ```

10. **Color Picker**:
    ```html
    <label for="favouriteColor">Favorite Color:</label>
    <input type="color" id="favouriteColor" name="favouriteColor" />
    ```

11. **URL Input**:
    ```html
    <label for="website">Website:</label>
    <input type="url" id="website" name="website" placeholder="https://example.com" />
    ```

12. **Search Input**:
    ```html
    <label for="searchquery">Search:</label>
    <input type="search" id="searchquery" name="searchquery" placeholder="Search..." />
    ```

13. **Range Input**:
    ```html
    <label for="range">Range:</label>
    <input type="range" id="range" name="range" min="0" max="100" value="50" />
    ```

14. **Month Input**:
    ```html
    <label for="expiryDate">Month & Year:</label>
    <input type="month" id="expiryDate" name="expiryDate" />
    ```

---

### Text Area

- The `<textarea>` tag is used to create multi-line input fields.
    ```html
    <label for="message">Message:</label>
    <textarea id="message" name="message" rows="4" cols="50" placeholder="Write your message..."></textarea>
    ```

---

### Dropdown List and `<select>`

- The `<select>` element is used to create a drop-down list, and `<option>` specifies the items in the list.
    ```html
    <label for="country">Favorite Country:</label>
    <select id="country" name="country">
      <option value="USA">USA</option>
      <option value="Canada">Canada</option>
      <option value="UK">UK</option>
    </select>
    ```

---

### Submit Buttons

1. **Standard Submit Button**:
    ```html
    <input type="submit" value="Submit" />
    ```

2. **Button Element**:
    ```html
    <button type="submit">Submit</button>
    ```

---

### `<datalist>` Tag

- The `<datalist>` tag is used to provide an autocomplete feature for an `<input>` element.

**Example:**
```html
<label for="browsers">Choose a browser:</label>
<input list="browsers" name="browser" id="browsers" />
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Safari">
  <option value="Edge">
</datalist>
```

---

### Common Input Attributes

1. **`type`**: Specifies the type of `<input>` (e.g., `text`, `email`, `number`, `submit`, etc.).
2. **`placeholder`**: Provides a hint for the expected input value.
3. **`name`**: Assigns a name to the form element (important for form submission).
4. **`required`**: Marks the input as required, preventing form submission if left empty.
5. **`autocomplete`**: Suggests previous entries, values can be `on` or `off`.
6. **`size`**: Specifies the visible width of the input field.
7. **`value`**: Pre-fills the input with a default value.
8. **`readonly`**: Makes the input field uneditable, while still submitting the value.
9. **`disabled`**: Disables the input field, preventing user interaction.
10. **`pattern`**: Specifies a regular expression that the input value must match.
11. **`id` and `class`**: Used for uniquely identifying and styling form elements.


---
### `action` Attribute
The `action` attribute specifies the URL where the form data should be sent when the form is submitted. This URL is the server-side script or endpoint that will process the submitted data.

**Syntax:**
```html
<form action="https://www.example.com/submit-form">
  <!-- Form elements go here -->
</form>
```

*If the `action` attribute is omitted, the form will submit to the same URL as the page that contains the form.*

---

### `method` Attribute
The `method` attribute specifies the HTTP method the browser uses to submit the form data to the server. The two most commonly used methods are `GET` and `POST`.

- **`GET`**: Sends the form data appended to the URL as query parameters. This method is used for retrieving data and should not be used for sensitive data.

    **Syntax:**
    ```html
    <form action="https://www.example.com/submit-form" method="GET">
      <!-- Form elements go here -->
    </form>
    ```

    *In the URL, the form data will appear after the `?` symbol, like `https://www.example.com/submit-form?name=value`.*

- **`POST`**: Sends the form data in the body of the HTTP request. This method is used for sending data to the server, especially for sensitive information or when submitting large amounts of data.

    **Syntax:**
    ```html
    <form action="https://www.example.com/submit-form" method="POST">
      <!-- Form elements go here -->
    </form>
    ```

    *The form data will not be visible in the URL and is sent securely in the request body.*

---

### `enctype` Attribute
The `enctype` attribute specifies how the form data should be encoded when submitted to the server. This attribute is important for forms that include file uploads.

- **`application/x-www-form-urlencoded`**: This is the default encoding type. It encodes form data as key-value pairs, with spaces replaced by `+` and special characters encoded using percent-encoding.

    **Syntax:**
    ```html
    <form action="https://www.example.com/submit-form" method="POST" enctype="application/x-www-form-urlencoded">
      <!-- Form elements go here -->
    </form>
    ```

- **`multipart/form-data`**: This encoding type is used when the form includes file uploads. It allows files to be sent as part of the form data, with each part encoded separately.

    **Syntax:**
    ```html
    <form action="https://www.example.com/submit-form" method="POST" enctype="multipart/form-data">
      <!-- Form elements, including file inputs, go here -->
      <input type="file" name="fileUpload" />
    </form>
    ```

- **`text/plain`**: This encoding type sends form data as plain text, with form fields and values separated by newline characters. It is not commonly used and may not be suitable for forms requiring special encoding.

    **Syntax:**
    ```html
    <form action="https://www.example.com/submit-form" method="POST" enctype="text/plain">
      <!-- Form elements go here -->
    </form>
    ```

---

### Summary of Form Attributes:

- **`action`**: URL to send form data.
- **`method`**: HTTP method (`GET` or `POST`).
- **`enctype`**: Encoding type (`application/x-www-form-urlencoded`, `multipart/form-data`, `text/plain`).
!
```



Here’s the explanation of HTML form semantic elements and HTML5 semantic elements:

```markdown
## HTML Form Semantic Elements

### `<label>`
The `<label>` element is used to define a label for an input element in a form. It provides a clickable area that focuses the corresponding input, improving accessibility.

**Syntax:**
```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

- The `for` attribute links the label to the input with the matching `id` value. When the user clicks the label, the focus is moved to the associated input field.

---

### `<fieldset>`
The `<fieldset>` element is used to group related form elements together. It draws a box around the elements and is often used with the `<legend>` element.

**Syntax:**
```html
<fieldset>
  <legend>Personal Information</legend>
  <label for="fname">First Name:</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name:</label>
  <input type="text" id="lname" name="lname">
</fieldset>
```

- It visually groups form controls, helping users to understand the relationship between them.

---

### `<legend>`
The `<legend>` element provides a title or description for the contents of a `<fieldset>`. It is typically the first element inside a `<fieldset>`.

**Syntax:**
```html
<fieldset>
  <legend>Shipping Address</legend>
  <label for="address">Address:</label>
  <input type="text" id="address" name="address">
</fieldset>
```

- The `<legend>` element describes the context of the form controls grouped within the `<fieldset>`, enhancing clarity.

---

## HTML5 Semantic Elements

HTML5 introduced semantic elements to give more meaning to the structure of web pages, making it easier for browsers and developers to understand the content.

### `<header>`
The `<header>` element represents the introductory content or a group of navigational links for a section or page. It usually contains headings, logos, or search bars.

**Syntax:**
```html
<header>
  <h1>Website Title</h1>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>
</header>
```

---

### `<nav>`
The `<nav>` element represents a section of navigation links. It is used for menus, tables of contents, or other sets of navigational links.

**Syntax:**
```html
<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Services</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>
```

---

### `<main>`
The `<main>` element represents the main content of the document. There should only be one `<main>` element per page, and it excludes content like sidebars and footers.

**Syntax:**
```html
<main>
  <article>
    <h2>Main Content Title</h2>
    <p>This is the main content of the page.</p>
  </article>
</main>
```

---

### `<article>`
The `<article>` element represents a self-contained piece of content, such as a blog post or news article. It can be distributed or syndicated independently.

**Syntax:**
```html
<article>
  <h2>Article Title</h2>
  <p>This is an article.</p>
</article>
```

---

### `<section>`
The `<section>` element represents a thematic grouping of content, typically with a heading. It divides the content into logical sections.

**Syntax:**
```html
<section>
  <h2>Section Title</h2>
  <p>This is a section of the document.</p>
</section>
```

---

### `<aside>`
The `<aside>` element represents content related to the main content, such as sidebars, pull quotes, or related links. It can appear in sidebars or elsewhere.

**Syntax:**
```html
<aside>
  <h2>Related Information</h2>
  <p>This is content related to the main article.</p>
</aside>
```

---

### `<footer>`
The `<footer>` element represents the footer for a section or page. It typically contains information about the author, copyright, or links to related documents.

**Syntax:**
```html
<footer>
  <p>&copy; 2024 Website Name. All rights reserved.</p>
</footer>
```

---

### Summary of HTML5 Semantic Elements (Only One Per Page):
- **`<header>`**: Introductory content or navigational links.
- **`<nav>`**: Navigation section for links.
- **`<main>`**: Main content of the document.
- **`<article>`**: Self-contained piece of content.
- **`<section>`**: Thematic grouping of content.
- **`<aside>`**: Related or tangential content.
- **`<footer>`**: Footer of a page or section.

These elements help structure the page in a meaningful way, improving accessibility and SEO.

<img src="Semantic pic.jpg" alt="HTML5 Semantics" width="500" height="300">



## Meta Tags in HTML

The `<meta>` tag in HTML provides metadata about the webpage. Metadata is not displayed on the page itself but is used by browsers, search engines, and other services to better understand the content and behavior of the page.

### 1. **Meta Tag for `robots`**
The `robots` meta tag controls how search engines index the page and follow its links. It instructs search engine crawlers (like Googlebot) on whether to index the page and whether to follow links on the page.

**Syntax:**
```html
<meta name="robots" content="index, follow">
```

- **`index`**: Tells search engines to include the page in their search results.
- **`follow`**: Tells search engines to follow the links on the page.
- **`noindex`**: Tells search engines **not** to index the page.
- **`nofollow`**: Tells search engines **not** to follow links on the page.

**Example:**
```html
<meta name="robots" content="noindex, nofollow">
```
This example tells search engines not to index the page and not to follow the links.

---

### 2. **Meta Tag for `description`**
The `description` meta tag provides a brief summary of the webpage. This description often appears in search engine results below the page title, helping users understand what the page is about before clicking.

**Syntax:**
```html
<meta name="description" content="This is a brief description of the page.">
```

- **Purpose**: Helps improve search engine rankings and click-through rates by providing an informative snippet of the page’s content.

**Example:**
```html
<meta name="description" content="Learn HTML meta tags, including robots, description, and more.">
```

---

### 3. **Meta Tag for `keywords`**
The `keywords` meta tag allows you to define keywords relevant to the page content. These keywords can help search engines understand the page's focus, though many modern search engines (like Google) don't prioritize this meta tag as much anymore.

**Syntax:**
```html
<meta name="keywords" content="HTML, meta tags, SEO, web development">
```

- **Purpose**: It was historically used to improve search engine optimization (SEO) by providing search engines with important keywords related to the content.

**Example:**
```html
<meta name="keywords" content="HTML, SEO, meta tags, robots, description">
```

---

### 4. **Meta Tag for `author`**
The `author` meta tag defines the author of the webpage. It can be useful for indicating who wrote or owns the content.

**Syntax:**
```html
<meta name="author" content="John Doe">
```

- **Purpose**: Helps identify the content creator and may be used by search engines or social platforms.

**Example:**
```html
<meta name="author" content="Jane Smith">
```

---

### Summary of Meta Tags:
- **`<meta name="robots" content="index, follow">`**: Tells search engines how to index the page and whether to follow links.
- **`<meta name="description" content="...">`**: Provides a short description of the page, often used in search results.
- **`<meta name="keywords" content="...">`**: Defines keywords relevant to the page (not as widely used for SEO today).
- **`<meta name="author" content="...">`**: Specifies the author of the webpage.

---

### Example of Meta Tags in a Document:
```html
<head>
  <meta name="robots" content="index, follow">
  <meta name="description" content="A comprehensive guide on HTML meta tags and their uses.">
  <meta name="keywords" content="HTML, meta tags, SEO, web development">
  <meta name="author" content="John Doe">
</head>
```

---
---

### What's Next?

There are still a few important topics to be added:
- Difference between HTML and HTML5
- Inline vs Block Elements
- Adding Email and WhatsApp links
- Making only a part of an image clickable
- List of Void & Block Elements
- `<span>` vs `<div>` tags
- Ensuring `id` and `for` attributes match
---
---