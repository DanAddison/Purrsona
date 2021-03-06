<div align="center">
  <a href="">
    <img alt="" src="src/assets/images/Purrsona_screenshot.png" width="700" />
  </a>
</div>

# Purrsona

A simple Eleventy Starter Kit, my base for all new 11ty projects.

I've simply added a little bit more flesh on the bones of [Eleventastic](https://github.com/maxboeck/eleventastic) by Max Boeck.

## Features

-   CSS Pipeline (Sass, CleanCSS)
-   JS Bundling (Webpack)
-   SVG Icon Sprite Generation
-   Critical CSS
-   HTML Minification
-   No external builds, everything runs through 11ty

## Getting Started

To install the necessary packages, run this command in the root folder of the site:

```sh
npm install
```

### Commands

-   Run `npm start` for a development server and live reloading
-   Run `npm run build` to generate a production build

## CSS

Styling works with Sass. The main index file is in `src/assets/styles/main.scss`. Import any SCSS code you want in there; it will be processed and optimized. The output is in `dist/assets/styles/main.css`

## JS

Javascript can be written in ES6 syntax. The main index file is in `src/assets/scripts/main.js`. It will be transpiled to ES5 with babel, bundled together with webpack, and minified in production. The output is in `dist/assets/scripts/main.js`

## SVG Icons

All SVG files added to `src/assets/icons` will be bundled into a `symbol` sprite file. The SVG filename will then be used as the symbol identifier and the icon can be used as a shortcode.

For example, if you have a `github.svg` file in that folder, you can display it anywhere by using `{% icon "github" %}` in your templates.

## Critical CSS

Currently, critical CSS will only be inlined in the head of the homepage. This is done by using the [critical](https://github.com/addyosmani/critical) package in an automatic transform.

## Deployment
[![Netlify Status](https://api.netlify.com/api/v1/badges/6004f385-4fb2-46b5-a11b-eba408c8f646/deploy-status)](https://app.netlify.com/sites/purrsona/deploys)

## Credits

This is basically [Eleventastic](https://github.com/maxboeck/eleventastic) by Max Boeck.

I've just added a little more flesh on its bones to make things even quicker to get up and running.

Max in turn credits the following for influencing Eleventastic:

-   Phil Hawksworth: [EleventyOne](https://github.com/philhawksworth/eleventyone)
-   Mike Riethmuller: [Supermaya](https://github.com/MadeByMike/supermaya)
-   Zach Leatherman: [zachleat.com](https://github.com/zachleat/zachleat.com)
