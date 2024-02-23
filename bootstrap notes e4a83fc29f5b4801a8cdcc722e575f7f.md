# bootstrap notes

## Bootstrap Notes

Bootstrap is a popular front-end framework for building responsive and mobile-first websites. It provides a collection of CSS and JavaScript components that make it easier to design and develop web pages.

Some key features of Bootstrap include:

- Responsive grid system: Bootstrap utilizes a flexible and responsive grid system that allows developers to create layouts that adapt to different screen sizes and devices.
- Pre-styled components: Bootstrap provides a wide range of pre-styled components, such as buttons, forms, navigation bars, and more. These components can be easily customized to match the design of a website.
- JavaScript plugins: Bootstrap includes a set of JavaScript plugins that enhance the functionality of web pages. Examples of these plugins include carousels, modals, and dropdown menus.

Using Bootstrap can significantly speed up the development process and help create modern and visually appealing websites.

It is important to note that while Bootstrap provides a solid foundation for building websites, customization may be required to achieve a unique and tailored design.

<aside>
👉 The following text is preliminary.

</aside>

A CDN (Content Delivery Network) is a network of servers located in different geographic locations that deliver web content to users based on their location. When a user requests a file, such as a CSS or JavaScript file, the CDN serves the file from the server that is closest to the user, ensuring faster delivery and improved performance. CDNs are commonly used to deliver static files, such as libraries or frameworks like Bootstrap, to websites.

navigation bar using Bootsrtap

```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
```

**Breakpoints are customizable widths that determine how your responsive layout behaves across device or viewport sizes in Bootstrap.**

•   **Breakpoints are the building blocks of responsive design.** Use them to control when your layout can be adapted at a particular viewport or device size.

- **Use media queries to architect your CSS by breakpoint.** Media queries are a feature of CSS that allow you to conditionally apply styles based on a set of browser and operating system parameters. We most commonly use `min-width` in our media queries.
- **Mobile first, responsive design is the goal.** Bootstrap’s CSS aims to apply the bare minimum of styles to make a layout work at the smallest breakpoint, and then layers on styles to adjust that design for larger devices. This optimizes your CSS, improves rendering time, and provides a great experience for your visitors.

## **Available breakpoints**

Bootstrap includes six default breakpoints, sometimes referred to as *grid tiers*, for building responsively. These breakpoints can be customized if you’re using our source Sass files.

| Breakpoint | Class infix | Dimensions |
| --- | --- | --- |
| Extra small | None | <576px |
| Small | sm | ≥576px |
| Medium | md | ≥768px |
| Large | lg | ≥992px |
| Extra large | xl | ≥1200px |
| Extra extra large | xxl | ≥1400px |

Containers

Containers are the most basic layout element in Bootstrap and are **required when using our default grid system**. Containers are used to contain, pad, and (sometimes) center the content within them. While containers *can* be nested, most layouts do not require a nested container.

Bootstrap comes with three different containers:

- `.container`, which sets a `max-width` at each responsive breakpoint
- `.container-{breakpoint}`, which is `width: 100%` until the specified breakpoint
- `.container-fluid`, which is `width: 100%` at all breakpoints

The table below illustrates how each container’s `max-width` compares to the original `.container` and `.container-fluid` across each breakpoint.

Responsive containers 

allow you to specify a class that is 100% wide until the specified breakpoint is reached, after which we apply `max-width`s for each of the higher breakpoints. For example, `.container-sm` is 100% wide to start until the `sm` breakpoint is reached, where it will scale up with `md`, `lg`, `xl`, and `xxl`.

```html
<div class="container-sm">100% wide until small breakpoint</div>
<div class="container-md">100% wide until medium breakpoint</div>
<div class="container-lg">100% wide until large breakpoint</div>
<div class="container-xl">100% wide until extra large breakpoint</div>
<div class="container-xxl">100% wide until extra extra large breakpoint</div>
```

responsive breakpoint example

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Bootstrap Containers with Responsive Breakpoints</title>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
    <div class="container-sm border py-3 my-3">100% wide until screen size less than 576px</div>
    <div class="container-md border py-3 my-3">100% wide until screen size less than 768px</div>
    <div class="container-lg border py-3 my-3">100% wide until screen size less than 992px</div>
    <div class="container-xl border py-3 my-3">100% wide until screen size less than 1200px</div>
    <p class="m-3"><strong>Note:</strong> The classes ".border", ".py-3", and ".my-3" are <a href="/twitter-bootstrap-tutorial/bootstrap-helper-classes.php" target="_top">utility classes</a> to add borders, paddings, and margins to the element, respectively.</p>
    <p class="m-3"><strong>Tip:</strong> Open the output in a new blank tab (Click the arrow next to "Show Output" button) and resize the browser window to understand how the Bootstrap responsive grid system works.</p>
</body>
</html>
```

GRID

important points about the grid system 

- **Our grid supports [six responsive breakpoints](https://getbootstrap.com/docs/5.3/layout/breakpoints/).** Breakpoints are based on `min-width` media queries, meaning they affect that breakpoint and all those above it (e.g., `.col-sm-4` applies to `sm`, `md`, `lg`, `xl`, and `xxl`). This means you can control container and column sizing and behavior by each breakpoint.
- **Containers center and horizontally pad your content.** Use `.container` for a responsive pixel width, `.container-fluid` for `width: 100%` across all viewports and devices, or a responsive container (e.g., `.container-md`) for a combination of fluid and pixel widths.
- **Rows are wrappers for columns.** Each column has horizontal `padding` (called a gutter) for controlling the space between them. This `padding` is then counteracted on the rows with negative margins to ensure the content in your columns is visually aligned down the left side. Rows also support modifier classes to [uniformly apply column sizing](https://getbootstrap.com/docs/5.3/layout/grid/#row-columns) and [gutter classes](https://getbootstrap.com/docs/5.3/layout/gutters/) to change the spacing of your content.
- **Columns are incredibly flexible.** There are 12 template columns available per row, allowing you to create different combinations of elements that span any number of columns. Column classes indicate the number of template columns to span (e.g., `col-4` spans four). `width`s are set in percentages so you always have the same relative sizing.
- **Gutters are also responsive and customizable.** [Gutter classes are available](https://getbootstrap.com/docs/5.3/layout/gutters/) across all breakpoints, with all the same sizes as our [margin and padding spacing](https://getbootstrap.com/docs/5.3/utilities/spacing/). Change horizontal gutters with `.gx-*` classes, vertical gutters with `.gy-*`, or all gutters with `.g-*` classes. `.g-0` is also available to remove gutters.
- **Sass variables, maps, and mixins power the grid.** If you don’t want to use the predefined grid classes in Bootstrap, you can use our [grid’s source Sass](https://getbootstrap.com/docs/5.3/layout/grid/#sass-variables) to create your own with more semantic markup. We also include some CSS custom properties to consume these Sass variables for even greater flexibility for you.

grid with breakpoints

Bootstrap’s grid system can adapt across all six default breakpoints, and any breakpoints you customize. The six default grid tiers are as follows:

- Extra small (xs)
- Small (sm)
- Medium (md)
- Large (lg)
- Extra large (xl)
- Extra extra large (xxl)

Row Columns

Use the responsive `.row-cols-*` classes to quickly set the number of columns that best render your content and layout. Whereas normal `.col-*` classes apply to the individual columns (e.g., `.col-md-4`), the row columns classes are set on the parent `.row` as a shortcut. With `.row-cols-auto` you can give the columns their natural width.

```html
<div class="container text-center">
  <div class="row row-cols-2">
    <div class="col">Column</div>
    <div class="col">Column</div>
    <div class="col">Column</div>
    <div class="col">Column</div>
  </div>
</div>
```

Nesting

To nest your content with the default grid, add a new `.row` and set of `.col-sm-*` columns within an existing `.col-sm-*` column. Nested rows should include a set of columns that add up to 12 or fewer (it is not required that you use all 12 available columns).

```html
<div class="container text-center">
  <div class="row">
    <div class="col-sm-3">
      Level 1: .col-sm-3
    </div>
    <div class="col-sm-9">
      <div class="row">
        <div class="col-8 col-sm-6">
          Level 2: .col-8 .col-sm-6
        </div>
        <div class="col-4 col-sm-6">
          Level 2: .col-4 .col-sm-6
        </div>
      </div>
    </div>
  </div>
</div>
```