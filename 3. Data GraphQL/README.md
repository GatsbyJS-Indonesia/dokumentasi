# Query Data di Gatsby dengan GraphQL

## Pertama dengan GraphQL query

Buka file `gatsby-config.js` pada root direktori, sebagai awal konfigurasi seperti di bawah:
```js
/**
 * Configure your Gatsby site with this file.
 *
 * See: https://www.gatsbyjs.org/docs/gatsby-config/
 */

module.exports = {
  /* Your site config here */
  plugins: [],
}
```

Diubah menjadi:
```js
/**
 * Configure your Gatsby site with this file.
 *
 * See: https://www.gatsbyjs.org/docs/gatsby-config/
 */

module.exports = {
  /* Your site config here */
  siteMetadata: {
    title: `Title from siteMetadata`,
  },
  plugins: [],
}
```

💡 Restart development server

## Menggunakan page Query

Buat file `about.js` pada `src/pages/about.js`, dan isi seperti di bawah:
```jsx
import React from "react"
import { graphql } from "gatsby"

export default function About({ data }) {
  return (
    <h1>About {data.site.siteMetadata.title}</h1>
    <p>
      We're the only site running on your computer dedicated to showing the
      best photos and videos of pandas eating lots of food.
    </p>
  )
}

export const query = graphql`
  query {
    site {
      siteMetadata {
        title
      }
    }
  }
`
```

> Tampilan di browser pada halaman `about` akan menampilkan `Title from siteMetadata` yang sudah di-set pada file `gatsby-config.js`, dan ditampilkan pada komponen `<h1>` di dalam file `about.js` 

## ➡️ Apa selanjutnya

Tutorial ini berasal dari dokumentasi [Official Gatsby](https://www.gatsbyjs.org/tutorial/part-four/)