# Search Atlas Otto — Pixel Installation

## The Pixel

Paste this snippet into your site's `<head>` tag:

```html
<script
  nowprocket
  nitro-exclude
  type="text/javascript"
  id="sa-dynamic-optimization"
  data-uuid="ceecc072-1841-4469-9969-03ecf7ed37fa"
  src="https://dashboard.searchatlas.com/scripts/dynamic_optimization.js"
></script>
```

Or use the dynamic loader version:

```html
<script>
  var script = document.createElement("script");
  script.setAttribute("nowprocket", "");
  script.setAttribute("nitro-exclude", "");
  script.src = "https://dashboard.searchatlas.com/scripts/dynamic_optimization.js";
  script.dataset.uuid = "ceecc072-1841-4469-9969-03ecf7ed37fa";
  script.id = "sa-dynamic-optimization";
  document.head.appendChild(script);
</script>
```

---

## Framework Installation

### React
Open `public/index.html` and paste the snippet inside the `<head>` tag.

### Next.js
Open `src/app/layout.tsx`. Inside the `RootLayout` method, add the snippet within the `<head>` tag.

### Vue.js
Open `public/index.html` and paste the snippet inside the `<head>` tag.

### Nuxt.js
Open `nuxt.config.ts`. Add the snippet under the `app -> head` property inside `defineNuxtConfig`.

### Angular
Open `src/index.html` and paste the snippet inside the `<head>` tag.

### Astro
Open `src/layouts/layout.astro` and paste the snippet inside the `<head>` tag.

### Svelte
Open `src/app.html` and paste the snippet inside the `<head>` tag.

### Remix
Open `app/root.tsx`. Inside the `Layout` method, add the snippet within the `<head>` tag.

### Qwik
Open `src/root.tsx`. Inside the component method, place the snippet inside the `<Head>` tag.

### PReact / Solid.js
Open `index.html` in the root directory and paste the snippet inside the `<head>` tag.

---

## Verify It's Working

1. Open **DevTools** (F12 or right-click > Inspect)
2. Go to the **Network** tab
3. Reload the page
4. Filter by **JS** or search for `dynamic_optimization`
5. Look for a `200 OK` response on the pixel request

A successful `200 OK` means the pixel is firing correctly.
