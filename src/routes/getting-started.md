---
layout: doc
---

<h1 class="text-2xl w-full dark:text-white">Getting Started</h1>
<h2 class="text-xl w-full mt-8 dark:text-white">Installation</h2>
<p class="dark:text-white">Install SvelteKit.</p>

```sh
npm init svelte@next sveltekit-demo $ cd sveltekit-demo
npm install 
```

<p class="dark:text-white">Install Tailwind CSS and Flowbite.</p>

```sh
npx svelte-add@latest tailwindcss
npm i flowbite 
```

<p class="dark:text-white">Install svelte-flow.</p>

```sh
npm i -D svelte-flow 
```

<p class="dark:text-white">Add the following in the script tag in the __layout.svelte :</p>

```html
<script>
  import "../app.css";
  import "flowbite/dist/flowbite.css";
</script>

<slot />
```



