<h1 align=center>AlpineJS</h1>
<p align=center>How to include AlpineJS &amp; Collapse in your project</p>

AlpineJS lessons: [here](https://laracasts.com/series/alpine-essentials/episodes/1)

AlpineJS, create modal: [here](https://w3collective.com/modal-dialog-alpine-js/)

Use AlpineJS and Laravel-Mix [here](https://dev.to/martin_betz/how-to-use-alpinejs-with-laravel-mix-50cc)

<hr />

### Essentials

  - Hide Elements Until Alpine Js Loads

  ```css
  [x-cloak] {
      display: none !important;
  }
  ```
  ```html
  <div class="overlay" x-show="isModalOpen" x-cloak></div>
  ```
  
<br />
<br />

### Use Alpine in project via npm

```bash
npm install alpinejs
```

import Alpine into your bundle and initialize it like so:
  ```js
  import Alpine from 'alpinejs'

  window.Alpine = Alpine

  Alpine.start()
  ```
<br />
<br />

### Use Collapse in project via npm

```bash
npm install @alpinejs/collapse
```
import Alpine into your bundle and initialize it like so:
  ```js
  import Alpine from 'alpinejs'
  import collapse from '@alpinejs/collapse'

  Alpine.plugin(collapse)
  ```
  
<br />
<br />

### Combine include AlpineJS and Collapse in main/app.js file (Apline scripts order matters)

```js
import Alpine from 'alpinejs';
import collapse from '@alpinejs/collapse'
window.Alpine = Alpine
Alpine.plugin(collapse)
Alpine.start()
```
