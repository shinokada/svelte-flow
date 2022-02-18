---
layout: doc
---

<h1 class="text-2xl w-full dark:text-white">Getting Started</h1>
<h2 class="text-xl w-full mt-8 dark:text-white">Installation</h2>
<p class="dark:text-white">Install SvelteKit:</p>

```sh
npm init svelte@next sveltekit-demo 
cd sveltekit-demo
npm install 
```

<p class="dark:text-white">Install Tailwind CSS:</p>

```sh
npx svelte-add@latest tailwindcss
```

<p class="dark:text-white">Run it:</p>

```sh
npm run dev
```

<p class="dark:text-white">You may need to install svelte-preprocess:</p>

```sh
npm i -D svelte-preprocess   
```

<p class="dark:text-white">Install Flowbite:</p>

```sh
npm i flowbite 
```

<p class="dark:text-white">Install svelte-flow and it's dependencies:</p>

```sh
npm i -D svelte-flow @codewithshin/svelte-heroicons svelte-collapse
```

<p class="dark:text-white">Add the following in the script tag in the __layout.svelte :</p>

```html
<script>
  import "../app.css";
  import "flowbite/dist/flowbite.css";
</script>

<slot />
```

<p class="dark:text-white">Update tailwind.config.cjs:</p>

```js
const config = {
  content: [
    "./src/**/*.{html,js,svelte,ts}",
    "./node_modules/svelte-flow/**/*.{html,js,svelte,ts}",
  ],
  ...
```