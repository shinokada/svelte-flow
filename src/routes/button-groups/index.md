---
layout: doc
---

<script>
  import {ButtonGroup, ButtonGroupOutline} from 'svelte-flow'
</script>


<h1 class="text-3xl w-full mb-8 text-gray-900 dark:text-white">Button groups</h1>

```svelte
<script>
  import {ButtonGroup, ButtonGroupOutline} from 'svelte-flow'
  let buttons = [
  {
    href: "/",
    name: "Profile",
  },
  {
    href: "/",
    name: "Settings",
  },
  {
    href: "/",
    name: "Messages",
  },
];
</script>
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white">Props</h2>

```svelte
let buttons = [
  {
    href: "/",
    name: "Profile",
  },
  {
    href: "/",
    name: "Settings",
  },
  {
    href: "/",
    name: "Messages",
  },
];
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white">Default</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ButtonGroup {buttons}/>
</div>


```svelte
<ButtonGroup {buttons}/>
```

<h2 class="text-2xl w-full dark:text-white mt-8">Adding links</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Badge name="Default" textSize="text-sm"/>
<Badge name="Gray" color="gray" textSize="text-sm"/>
<Badge name="Red" color="red" textSize="text-sm"/>
<Badge name="Green" color="green" textSize="text-sm"/>
<Badge name="Yellow" color="yellow" textSize="text-sm"/>
<Badge name="Indigo" color="indigo" textSize="text-sm"/>
<Badge name="Purple" color="purple" textSize="text-sm"/>
<Badge name="Pink" color="pink" textSize="text-sm"/>
</div>

```svelte
<Badge name="Default" textSize="text-sm"/>
<Badge name="Gray" color="gray" textSize="text-sm"/>
<Badge name="Red" color="red" textSize="text-sm"/>
<Badge name="Green" color="green" textSize="text-sm"/>
<Badge name="Yellow" color="yellow" textSize="text-sm"/>
<Badge name="Indigo" color="indigo" textSize="text-sm"/>
<Badge name="Purple" color="purple" textSize="text-sm"/>
<Badge name="Pink" color="pink" textSize="text-sm"/>
```

<h2 class="text-2xl w-full dark:text-white mt-8">Size base</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<Badge name="Default" textSize="text-base"/>
<Badge name="Gray" color="gray" textSize="text-base"/>
<Badge name="Red" color="red" textSize="text-base"/>
<Badge name="Green" color="green" textSize="text-base"/>
<Badge name="Yellow" color="yellow" textSize="text-base"/>
<Badge name="Indigo" color="indigo" textSize="text-base"/>
<Badge name="Purple" color="purple" textSize="text-base"/>
<Badge name="Pink" color="pink" textSize="text-base"/>
</div>

```svelte

```