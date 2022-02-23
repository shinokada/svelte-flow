---
layout: doc
---

<script>
  import {ButtonGroup, ButtonGroupOutline} from 'svelte-flow'
    import {UserCircleIconSolid, AdjustmentsIconSolid, CloudDownloadIconSolid} from "@codewithshin/svelte-heroicons"
  let buttons1 = [
  {
    name: "Profile",
    link:"/",
    icon: UserCircleIconSolid
  },
  {
    name: "Settings",
    link:"/",
    icon: AdjustmentsIconSolid
  },
  {
    name: "Messages",
    link:"/",
    icon: CloudDownloadIconSolid
  },
];
  let buttons2 = [
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


<h1 class="text-3xl w-full mb-8 text-gray-900 dark:text-white">Button groups</h1>

```svelte
<script>
  import {ButtonGroup, ButtonGroupOutline} from 'svelte-flow'

  let buttons1 = [
  {
    name: "Profile",
  },
  {
    name: "Settings",
  },
  {
    name: "Messages",
  },
];
  let buttons2 = [
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
<ButtonGroup buttons={buttons1}/>
</div>


```svelte
<ButtonGroup buttons={buttons1}/>
```

<h2 class="text-2xl w-full text-gray-900 dark:text-white">Default with icon</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ButtonGroup buttons={buttons1}/>
</div>


```svelte
<ButtonGroup buttons={buttons1}/>
```

<h2 class="text-2xl w-full dark:text-white mt-8">Adding links</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">

</div>

```svelte

```

<h2 class="text-2xl w-full dark:text-white mt-8">Outline</h2>

<div
  class="container flex flex-wrap justify-evenly rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
<ButtonGroupOutline buttons={buttons1}/>
</div>

```svelte
<ButtonGroupOutline buttons={buttons1}/>
```