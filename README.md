# Most Common HTML Elements

A list of the most common HTML elements used. This is intended as a reference for designers and styleguide creators so that they do not forget components when defining styles.


## Rationale

This project is a barebones version of something like the [React Styleguidist](https://react-styleguidist.js.org/). While the React Styleguidist is a great project, not all projects are built with [React](https://reactjs.org/). It may be time consuming to expect a styleguide to be attached to a development framework. So this project expects only HTML elements with CSS classes.


## How to Use

Once a styleguide has been defined, or is in progress, developers can fork or copy this project to adapt it to the styleguide the way they want it.

The intent is to use a logic that creates a namespace for the CSS classes. by not targetting DOM elements directly in the CSS, this allows to decouple the styling from the semantic values. For example, with such a styling logic, it should be possible to quickly swap DOM elements without affecting styling.

All explanations are aligned with this intent, but you are free to adapt it to your preferences.


### Choose a Namespace

Start with choosing a namespace that will be applied to the parent container (`<body>`, `<div>`, or any other). For this example, we will use `ns`, short for "namespace".


### Agree on a Naming Convention

The namespace should serve as a prefix for defining classes. Here are a few examples:

- Headings: `ns-h1`, `ns-h2`, etc.
- Paragraph: `ns-p`
- Lists: `ns-ul`, `ns-ol`, etc.
- Hyperlinks: `ns-a`
- Buttons: `ns-btn`


### Example

With those rules agreed upon, a basic implementation would look like this:

```html
<html>
  <body class="ns">
    <h1 class="ns-h1">Heading</h1>
    <p class="ns-p">Lorem ipsum dolor sit amet...</p>
  </body>
</html>
```


### Adapting the `index.html`

As stated before, this document is meant as a reference for designers, but it shoudl also serve as a reference for developers. In order to serve that second purpose, make sure to adapt the code examples with the relevant namespace and classes.
