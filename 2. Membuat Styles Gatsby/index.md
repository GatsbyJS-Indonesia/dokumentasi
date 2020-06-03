# Membuat Gatsby Block

Membuat Styles di dalam Gatsby sangat mudah

## Buat `css` file di dalam direktori `src/styles` dengan nama `global.css`

> Susunan direktori:
```
├── package.json
├── src
│   └── pages
│       └── index.js
│   └── styles
│       └── global.css
```

> Isi file:
src/styles/global.css
```js
html {
  background-color: lavenderblush;
}
```

## Buat file `gatsby-browser.js` pada direktori utama

> Susunan direktori 
```
├── package.json
├── src
│   └── pages
│       └── index.js
│   └── styles
│       └── global.css
├── gatsby-browser.js
```

> Isi file:
```
import "./src/styles/global.css"
```
