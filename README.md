# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

The main difference between semantic and non-semantic HTML elements lies in how they are described. Semantic elements clearly describe their purpose to both the browser and the developer. For instance, a elements like `<article>`, `<section>`, and `<header>` are considered semantic because they clearly communicate their role in the HTML document to the developer and the browser. On the other hand, elements like `<div>` or `<span>` don't use the same easy to understand format and don't convey purpose of the element, therefore it is considered non-semantic. Since semantic tags use plain language and are easy to understand developers can benefit from this to create structured code that is both maintainable and comprehensible.

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Some ways to make a website more accessible are:

1. Writing descriptive alt text for screen reading technologies to effectively describe images and assist individuals that are blind or visually impaired.
2. Making a structured use of heading and subheading tags helps screen readers and users better understand the structure of the page.
3. Testing websites on a variety of devices ensures that all users have access to a responsive site that adapts to their device's needs.

It is important to create websites that meet accessibility standards not only because the website will be accessible to a broader audience, but also because technology should be inclusive and adapt to support any user's needs.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

Inline styles could be useful to make minor style changes to a single HTML element without affecting other elements. On the other hand, writing styles in a separate CSS file is recommended to create organized and maintainable websites. It is practical for developers to have a single file responsible for the styling portion of the website that is separate from the HTML code. This keeps the HTML clean, reduces repetitive inline styles, and minimizes the risk of unintended styling conflicts.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

Classes can be used to refer to one or more HTML elements. A class works like a nickname you can assign to multiple elements. If several elements share the same nickname you can conveniently use that nickname to select and make changes to all of them at once. It is also possible to have multiple nicknames (classes) for a particular element as long as they are separated by a space.

To assign a class to an HTML element, add the `class` attribute with the class name in the opening tag, like in this example:

```html
<h1 class="title">Hello World</h1>
```

In CSS, to style elements with the `title` class, use the dot (`.`) class selector followed by the class name, as shown here:

```css
.title {
  color: blue;
}
```

IDs in the other hand are an unique identifier of a particular element. Think of IDs as a home address, in this case the home is the element and the address is the ID. Each address is unique to each home so you cannot reach that specific home (element) unless you have the right address (id).

To assign an ID to an HTML element, use the `id` attribute with a unique ID name in the opening tag:

```html
<h1 id="unique-title">Hello World</h1>
```

In CSS, select the element with this ID using the hashtag (`#`) ID selector followed by the ID name:

```css
#unique-title {
  color: blue;
}
```

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

Using only JavaScript and the DOM API to build entire websites is generally not recommended.
HTML and CSS are optimized for static content, allowing the browser to render pages more quickly and efficiently. Relying solely on JavaScript to create the entire website can slow down page load times, especially for users with slower devices or connections, which can negatively affect the user experience.
It is recommended to use HTML and CSS for creating content that does not often change dynamically such as text or images. JavaScript and the DOM API are better suited for the parts of the website that respond to user interaction. This way, only the parts that do use JavaScript will run, which consequentially reduces the load on the client's resources.
