# CRips

A static HTML/SCSS storefront template for a cryptocurrency mining hardware shop, built with [Swiper](https://swiperjs.com/) carousels.

## Project structure

```
index.html          Home page (hero, crypto/brand/algorithm sliders, testimonials, footer)
products.html        Product listing page
faqs.html            FAQ accordion page
assets/
  css/style.css      Compiled CSS (generated from scss, do not edit directly)
  scss/style.scss    Source styles
  img/               Images used across the site
```

## Development

Styles are written in `assets/scss/style.scss` and compiled to `assets/css/style.css`. Install the Dart Sass CLI and compile with:

```
sass assets/scss/style.scss assets/css/style.css --style=expanded --source-map
```

Add `--watch` to recompile on save while editing:

```
sass --watch assets/scss/style.scss:assets/css/style.css --source-map
```

There is no build step for the HTML/JS — open `index.html` directly in a browser, or serve the folder with any static file server.

## Features

- Responsive layout (breakpoints for tablet/mobile on grids and Swiper sliders)
- Dark mode toggle (persisted in `localStorage`, driven by CSS custom properties in `style.scss`)
- Login/Register modals
- FAQ accordion and product filter chips
