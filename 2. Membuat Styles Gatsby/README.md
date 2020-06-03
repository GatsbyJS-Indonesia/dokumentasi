# Membuat Gatsby Block

Membuat Styles di dalam Gatsby sangat mudah

## Buat `css` file di dalam direktori `src/styles` dengan nama `global.css`

- Susunan direktori:
```
├── package.json
├── src
│   └── pages
│       └── index.js
│   └── styles
│       └── global.css
```

- Isi file untuk `global.css`:
```
html {
  background-color: lavenderblush;
}
```

## Buat file `gatsby-browser.js` pada direktori utama

- Susunan direktori: 
```
├── package.json
├── src
│   └── pages
│       └── index.js
│   └── styles
│       └── global.css
├── gatsby-browser.js
```

- Isi file untuk `gatsby-browser.js`
```jsx
import "./src/styles/global.css"
```
