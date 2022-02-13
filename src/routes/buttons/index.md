---
layout: doc
---

<script>
  import { Button } from "svelte-flow";
</script>

<h1 class="text-3xl w-full dark:text-white">Buttons: Setup</h1>

<p class="dark:text-white">Import Button in the script tag.</p>

```svelte
<script>
  import { Button } from "svelte-flow";
</script>
```

<h1 class="text-3xl w-full dark:text-white">Size xs Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button xs" size="xs" />
  <Button name="Button xs" size="xs" type="dark" />
  <Button name="Button xs" size="xs" type="light" />
  <Button name="Button xs" size="xs" type="green" />
  <Button name="Button xs" size="xs" type="red" />
  <Button name="Button xs" size="xs" type="yellow" />
  <Button name="Button xs" size="xs" type="purple" />
</div>

```svelte
<Button name="Button xs" size="xs" />
<Button name="Button xs" size="xs" type="dark" />
<Button name="Button xs" size="xs" type="light" />
<Button name="Button xs" size="xs" type="green" />
<Button name="Button xs" size="xs" type="red" />
<Button name="Button xs" size="xs" type="yellow" />
<Button name="Button xs" size="xs" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white">Size xs Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button xs" size="xs" rounded="true" />
  <Button name="Button xs" size="xs" type="dark" rounded="true" />
  <Button name="Button xs" size="xs" type="light" rounded="true" />
  <Button name="Button xs" size="xs" type="green" rounded="true" />
  <Button name="Button xs" size="xs" type="red" rounded="true" />
  <Button name="Button xs" size="xs" type="yellow" rounded="true" />
  <Button name="Button xs" size="xs" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button xs" size="xs" rounded="true" />
<Button name="Button xs" size="xs" type="dark" rounded="true" />
<Button name="Button xs" size="xs" type="light" rounded="true" />
<Button name="Button xs" size="xs" type="green" rounded="true" />
<Button name="Button xs" size="xs" type="red" rounded="true" />
<Button name="Button xs" size="xs" type="yellow" rounded="true" />
<Button name="Button xs" size="xs" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white">Size xs Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button xs" size="xs" type="blue-outline" />
  <Button name="Button xs" size="xs" type="dark-outline" />
  <Button name="Button xs" size="xs" type="green-outline" />
  <Button name="Button xs" size="xs" type="red-outline" />
  <Button name="Button xs" size="xs" type="red-outline" />
  <Button name="Button xs" size="xs" type="purple-outline" />
</div>

```svelte
<Button name="Button xs" size="xs" type="blue-outline" />
<Button name="Button xs" size="xs" type="dark-outline" />
<Button name="Button xs" size="xs" type="green-outline" />
<Button name="Button xs" size="xs" type="red-outline" />
<Button name="Button xs" size="xs" type="red-outline" />
<Button name="Button xs" size="xs" type="purple-outline" />
```


<h1 class="text-3xl w-full dark:text-white">Size sm Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" size="sm" />
  <Button name="Button" size="sm" type="dark" />
  <Button name="Button" size="sm" type="light" />
  <Button name="Button" size="sm" type="red" />
  <Button name="Button" size="sm" type="green" />
  <Button name="Button" size="sm" type="yellow" />
  <Button name="Button" size="sm" type="purple" />
</div>

```svelte
<Button name="Button" size="sm" />
<Button name="Button" size="sm" type="dark" />
<Button name="Button" size="sm" type="light" />
<Button name="Button" size="sm" type="red" />
<Button name="Button" size="sm" type="green" />
<Button name="Button" size="sm" type="yellow" />
<Button name="Button" size="sm" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white">Size sm Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" size="sm" rounded="true" />
  <Button name="Button" size="sm" type="dark" rounded="true" />
  <Button name="Button" size="sm" type="light" rounded="true" />
  <Button name="Button" size="sm" type="green" rounded="true" />
  <Button name="Button" size="sm" type="red" rounded="true" />
  <Button name="Button" size="sm" type="yellow" rounded="true" />
  <Button name="Button" size="sm" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button" size="sm" rounded="true" />
<Button name="Button" size="sm" type="dark" rounded="true" />
<Button name="Button" size="sm" type="light" rounded="true" />
<Button name="Button" size="sm" type="green" rounded="true" />
<Button name="Button" size="sm" type="red" rounded="true" />
<Button name="Button" size="sm" type="yellow" rounded="true" />
<Button name="Button" size="sm" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white">Size sm Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" size="sm" type="blue-outline" />
  <Button name="Button" size="sm" type="dark-outline" />
  <Button name="Button" size="sm" type="green-outline" />
  <Button name="Button" size="sm" type="red-outline" />
  <Button name="Button" size="sm" type="red-outline" />
  <Button name="Button" size="sm" type="purple-outline" />
</div>

```svelte
<Button name="Button" size="sm" type="blue-outline" />
<Button name="Button" size="sm" type="dark-outline" />
<Button name="Button" size="sm" type="green-outline" />
<Button name="Button" size="sm" type="red-outline" />
<Button name="Button" size="sm" type="red-outline" />
<Button name="Button" size="sm" type="purple-outline" />
```

<h1 class="text-3xl w-full dark:text-white">Size base Default Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" size="base" />
  <Button name="Button" size="base" type="dark" />
  <Button name="Button" size="base" type="light" />
  <Button name="Button" size="base" type="red" />
  <Button name="Button" size="base" type="green" />
  <Button name="Button" size="base" type="yellow" />
  <Button name="Button" size="base" type="purple" />
</div>

```svelte
<Button name="Button" size="base" />
<Button name="Button" size="base" type="dark" />
<Button name="Button" size="base" type="light" />
<Button name="Button" size="base" type="red" />
<Button name="Button" size="base" type="green" />
<Button name="Button" size="base" type="yellow" />
<Button name="Button" size="base" type="purple" />
```

<h1 class="text-3xl w-full dark:text-white">Size base Rounded Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <Button name="Button" size="base" rounded="true" />
  <Button name="Button" size="base" type="dark" rounded="true" />
  <Button name="Button" size="base" type="light" rounded="true" />
  <Button name="Button" size="base" type="green" rounded="true" />
  <Button name="Button" size="base" type="red" rounded="true" />
  <Button name="Button" size="base" type="yellow" rounded="true" />
  <Button name="Button" size="base" type="purple" rounded="true" />
</div>

```svelte
<Button name="Button" size="base" rounded="true" />
<Button name="Button" size="base" type="dark" rounded="true" />
<Button name="Button" size="base" type="light" rounded="true" />
<Button name="Button" size="base" type="green" rounded="true" />
<Button name="Button" size="base" type="red" rounded="true" />
<Button name="Button" size="base" type="yellow" rounded="true" />
<Button name="Button" size="base" type="purple" rounded="true" />
```

<h1 class="text-3xl w-full dark:text-white">Size sm Outlined Buttons</h1>

<div class="rounded-xl w-full my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Button name="Button" size="base" type="blue-outline" />
<Button name="Button" size="base" type="dark-outline" />
<Button name="Button" size="base" type="green-outline" />
<Button name="Button" size="base" type="red-outline" />
<Button name="Button" size="base" type="red-outline" />
<Button name="Button" size="base" type="purple-outline" />
</div>

```svelte
<Button name="Button" size="base" type="blue-outline" />
<Button name="Button" size="base" type="dark-outline" />
<Button name="Button" size="base" type="green-outline" />
<Button name="Button" size="base" type="red-outline" />
<Button name="Button" size="base" type="red-outline" />
<Button name="Button" size="base" type="purple-outline" />
```
