# CSS to Sass conversion

A small, runnable example that converts the supplied traditional CSS rules into organized Sass partials.

## Structure

```text
scss/
  abstracts/   variables and mixins
  base/        global styles
  layout/      container
  components/  button and card
  main.scss    Sass entry point
css/
  styles.css   compiled output
```

The source uses `@use` (the modern Sass module system) rather than the deprecated `@import` syntax. It demonstrates variables, a reusable button mixin, nesting, and separate partials while retaining the original body, container, button, and card styles.

## Compile and preview

With Dart Sass installed, run:

```sh
sass --no-source-map scss/main.scss css/styles.css
```

Open `index.html` in a browser to view the result. The original CSS from the exercise is preserved in `styles-original.css` for comparison.
