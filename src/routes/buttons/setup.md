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



<p class="dark:text-white">Import Button in the script tag.</p>

```svelte
<script>
  import { Button } from "svelte-flow";
</script>
```

<h1 class="text-3xl w-full text-gray-900 dark:text-white">Button handler</h1>

<p class="dark:text-white">You can use handleClick.</p>

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
