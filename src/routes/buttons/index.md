---
layout: doc
---

<script>
  import { Button } from "svelte-flow";
  const btn1 = ()=>{
    alert('You clicked btn1.')
  }
  const btn2 = ()=>{
    alert ('You clicked btn2.')
  }
</script>

<h1 class="text-3xl w-full dark:text-white mb-8">Buttons: Setup</h1>

<h2 class="text-2xl w-full text-gray-900 dark:text-white">Button Props</h2>

```js
let rounded = false;
let textSize = "text-sm";
let name = "Read more";
let type = "blue";
```

<p class="dark:text-white">Import Button in the script tag.</p>

```svelte
<script>
  import { Button } from "svelte-flow";
</script>
```

<h1 class="text-3xl w-full text-gray-900 dark:text-white">Button handler</h1>

<p class="dark:text-white">You can use handleClick to Button component.</p>

```svelte
<script>
  import { Button } from "svelte-flow";
  const btn1 = ()=>{
    alert('You clicked btn1.')
  }
  const btn2 = ()=>{
    alert ('You clicked btn2.')
  }
</script>

<Button name="Button text-xs" on:handleClick={btn1} textSize="text-xs" />
<Button name="Button text-xs" on:handleClick={btn2} textSize="text-xs" />
```

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Button name="Button text-xs" on:handleClick={btn1} textSize="text-xs" />
<Button name="Button text-xs" on:handleClick={btn2} textSize="text-xs" />
</div>


<h1 class="text-3xl w-full dark:text-white my-8">Size xs Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button text-xs" textSize="text-xs" />
  <Button name="Button text-xs" textSize="text-xs" type="dark" />
  <Button name="Button text-xs" textSize="text-xs" type="light" />
  <Button name="Button text-xs" textSize="text-xs" type="green" />
  <Button name="Button text-xs" textSize="text-xs" type="red" />
  <Button name="Button text-xs" textSize="text-xs" type="yellow" />
  <Button name="Button text-xs" textSize="text-xs" type="purple" />
</div>

```svelte
<Button name="Button text-xs" textSize="text-xs" />
<Button name="Button text-xs" textSize="text-xs" type="dark" />
<Button name="Button text-xs" textSize="text-xs" type="light" />
<Button name="Button text-xs" textSize="text-xs" type="green" />
<Button name="Button text-xs" textSize="text-xs" type="red" />
<Button name="Button text-xs" textSize="text-xs" type="yellow" />
<Button name="Button text-xs" textSize="text-xs" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size xs Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button text-xs" textSize="text-xs" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="dark" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="light" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="green" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="red" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="yellow" rounded="true" />
  <Button name="Button text-xs" textSize="text-xs" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button text-xs" textSize="text-xs" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="dark" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="light" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="green" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="red" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="yellow" rounded="true" />
<Button name="Button text-xs" textSize="text-xs" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size xs Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button text-xs" textSize="text-xs" type="blue-outline" />
  <Button name="Button text-xs" textSize="text-xs" type="dark-outline" />
  <Button name="Button text-xs" textSize="text-xs" type="green-outline" />
  <Button name="Button text-xs" textSize="text-xs" type="red-outline" />
  <Button name="Button text-xs" textSize="text-xs" type="red-outline" />
  <Button name="Button text-xs" textSize="text-xs" type="purple-outline" />
</div>

```svelte
<Button name="Button text-xs" textSize="text-xs" type="blue-outline" />
<Button name="Button text-xs" textSize="text-xs" type="dark-outline" />
<Button name="Button text-xs" textSize="text-xs" type="green-outline" />
<Button name="Button text-xs" textSize="text-xs" type="red-outline" />
<Button name="Button text-xs" textSize="text-xs" type="red-outline" />
<Button name="Button text-xs" textSize="text-xs" type="purple-outline" />
```


<h1 class="text-3xl w-full dark:text-white my-8">Size sm Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" textSize="text-sm" />
  <Button name="Button" textSize="text-sm" type="dark" />
  <Button name="Button" textSize="text-sm" type="light" />
  <Button name="Button" textSize="text-sm" type="red" />
  <Button name="Button" textSize="text-sm" type="green" />
  <Button name="Button" textSize="text-sm" type="yellow" />
  <Button name="Button" textSize="text-sm" type="purple" />
</div>

```svelte
<Button name="Button" textSize="text-sm" />
<Button name="Button" textSize="text-sm" type="dark" />
<Button name="Button" textSize="text-sm" type="light" />
<Button name="Button" textSize="text-sm" type="red" />
<Button name="Button" textSize="text-sm" type="green" />
<Button name="Button" textSize="text-sm" type="yellow" />
<Button name="Button" textSize="text-sm" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size sm Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" textSize="text-sm" rounded="true" />
  <Button name="Button" textSize="text-sm" type="dark" rounded="true" />
  <Button name="Button" textSize="text-sm" type="light" rounded="true" />
  <Button name="Button" textSize="text-sm" type="green" rounded="true" />
  <Button name="Button" textSize="text-sm" type="red" rounded="true" />
  <Button name="Button" textSize="text-sm" type="yellow" rounded="true" />
  <Button name="Button" textSize="text-sm" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button" textSize="text-sm" rounded="true" />
<Button name="Button" textSize="text-sm" type="dark" rounded="true" />
<Button name="Button" textSize="text-sm" type="light" rounded="true" />
<Button name="Button" textSize="text-sm" type="green" rounded="true" />
<Button name="Button" textSize="text-sm" type="red" rounded="true" />
<Button name="Button" textSize="text-sm" type="yellow" rounded="true" />
<Button name="Button" textSize="text-sm" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size sm Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" textSize="text-sm" type="blue-outline" />
  <Button name="Button" textSize="text-sm" type="dark-outline" />
  <Button name="Button" textSize="text-sm" type="green-outline" />
  <Button name="Button" textSize="text-sm" type="red-outline" />
  <Button name="Button" textSize="text-sm" type="red-outline" />
  <Button name="Button" textSize="text-sm" type="purple-outline" />
</div>

```svelte
<Button name="Button" textSize="text-sm" type="blue-outline" />
<Button name="Button" textSize="text-sm" type="dark-outline" />
<Button name="Button" textSize="text-sm" type="green-outline" />
<Button name="Button" textSize="text-sm" type="red-outline" />
<Button name="Button" textSize="text-sm" type="red-outline" />
<Button name="Button" textSize="text-sm" type="purple-outline" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size base Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" textSize="text-base" />
  <Button name="Button" textSize="text-base" type="dark" />
  <Button name="Button" textSize="text-base" type="light" />
  <Button name="Button" textSize="text-base" type="red" />
  <Button name="Button" textSize="text-base" type="green" />
  <Button name="Button" textSize="text-base" type="yellow" />
  <Button name="Button" textSize="text-base" type="purple" />
</div>

```svelte
<Button name="Button" textSize="text-base" />
<Button name="Button" textSize="text-base" type="dark" />
<Button name="Button" textSize="text-base" type="light" />
<Button name="Button" textSize="text-base" type="red" />
<Button name="Button" textSize="text-base" type="green" />
<Button name="Button" textSize="text-base" type="yellow" />
<Button name="Button" textSize="text-base" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size base Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" textSize="text-base" rounded="true" />
  <Button name="Button" textSize="text-base" type="dark" rounded="true" />
  <Button name="Button" textSize="text-base" type="light" rounded="true" />
  <Button name="Button" textSize="text-base" type="green" rounded="true" />
  <Button name="Button" textSize="text-base" type="red" rounded="true" />
  <Button name="Button" textSize="text-base" type="yellow" rounded="true" />
  <Button name="Button" textSize="text-base" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button" textSize="text-base" rounded="true" />
<Button name="Button" textSize="text-base" type="dark" rounded="true" />
<Button name="Button" textSize="text-base" type="light" rounded="true" />
<Button name="Button" textSize="text-base" type="green" rounded="true" />
<Button name="Button" textSize="text-base" type="red" rounded="true" />
<Button name="Button" textSize="text-base" type="yellow" rounded="true" />
<Button name="Button" textSize="text-base" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white my-8">Size sm Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Button name="Button" textSize="text-base" type="blue-outline" />
<Button name="Button" textSize="text-base" type="dark-outline" />
<Button name="Button" textSize="text-base" type="green-outline" />
<Button name="Button" textSize="text-base" type="red-outline" />
<Button name="Button" textSize="text-base" type="red-outline" />
<Button name="Button" textSize="text-base" type="purple-outline" />
</div>

```svelte
<Button name="Button" textSize="text-base" type="blue-outline" />
<Button name="Button" textSize="text-base" type="dark-outline" />
<Button name="Button" textSize="text-base" type="green-outline" />
<Button name="Button" textSize="text-base" type="red-outline" />
<Button name="Button" textSize="text-base" type="red-outline" />
<Button name="Button" textSize="text-base" type="purple-outline" />
```
