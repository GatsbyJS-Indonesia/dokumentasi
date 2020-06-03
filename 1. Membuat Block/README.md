# Membuat Gatsby Block

Pada bagian ini, akan ditambahkan beberapa Block seperti Style, Image dan lain-lain pada file `src/pages/index.js`

## Buat perubahan pada halaman "Hello World!"

`src/pages/index.js`
```js
import React from "react"

export default function Home() {
  return <div style={{ color: `purple`, fontSize: `72px` }}>Hello Gatsby!</div>
}
``` 
Tampilan akan berubah sesuai `style` di atas

## Menambahkan Padding <p> 

`src/pages/index.js`
```js
import React from "react"

export default function Home() {
  return (
    <div style={{ color: `purple` }}>
      <h1>Hello Gatsby!</h1>
      <p>What a world.</p>
    </div>
  );
}
```

## Menambahkan Image pada

`src/pages/index.js`
```js
import React from "react"

export default function Home() {
  return (
    <div style={{ color: `purple` }}>
      <h1>Hello Gatsby!</h1>
      <p>What a world.</p>
      <img src="https://source.unsplash.com/random/400x200" alt="" />
    </div>
  )
}
```


