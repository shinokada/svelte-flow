---
layout: doc
---

<script>
  import { Button } from "svelte-flow";
</script>

<h1 class="text-3xl w-full mb-8 text-gray-900 dark:text-white">Buttons</h1>

<h2 class="text-2xl w-full text-gray-900 dark:text-white">Button Props</h2>

```js
let rounded = false;
let textSize = "text-sm";
let name = "Read more";
let type = "blue"; // blue| dark | light | green | red | yellow | puple
```

<h2 class="text-2xl w-full dark:text-white mt-8">Size xs</h2>

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

<h2 class="text-2xl w-full dark:text-white mt-8">Size sm</h2>

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

<h2 class="text-2xl w-full dark:text-white mt-8">Size base</h2>

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
