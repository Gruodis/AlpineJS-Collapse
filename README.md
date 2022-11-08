<h1 align=center>AlpineJS & Collapse How To</h1>
<p align=center>How to include AlpineJS &amp; Collapse</p>

<hr />

# Use Alpine in project via npm

```bash
npm install alpinejs
```

- import Alpine into your bundle and initialize it like so:
  ```js
  import Alpine from 'alpinejs'

  window.Alpine = Alpine

  Alpine.start()
  ```

```bash
npm install @alpinejs/collapse
```
- import Alpine into your bundle and initialize it like so:
  ```js
  import Alpine from 'alpinejs'
  import collapse from '@alpinejs/collapse'

  Alpine.plugin(collapse)
  ```

### Combine include AlpineJS and Collapse in main/app.js file (Apline scripts order matters)
```js
import Alpine from 'alpinejs';
import collapse from '@alpinejs/collapse'
window.Alpine = Alpine
Alpine.plugin(collapse)
Alpine.start()
```
