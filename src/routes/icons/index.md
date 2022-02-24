---
layout: doc
---

<script>
  import {
    TicketIconOutline,
    CameraIconOutline,
    BellIconSolid,
    ChevronLeftIconSolid,
  } from "@codewithshin/svelte-heroicons";
</script>

<h1 class="text-3xl w-full dark:text-white mb-4">HeroIcons</h1>

<p class=" dark:text-white">Svelte-flow uses <a class="text-blue-600 hover:underline dark:text-blue-500" href="https://github.com/shinokada/svelte-heroicons" target="_blank">svelte-heroicons</a>.
You can find all the icon names from the <a class="text-blue-600 hover:underline dark:text-blue-500" href="https://github.com/shinokada/svelte-heroicons/blob/main/icon-names.md">repo</a>.</p>

<p class=" dark:text-white">Svelte-heroicons allow you to change icon color and size by using TailwindCSS/Flowbite.</p>

<h2 class="text-2xl w-full dark:text-white mt-8">Examples</h2>

<div class="container flex flex-wrap justify-center rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">

<TicketIconOutline className="h-10 w-10 text-blue-500 dark:text-yellow-300" />

<CameraIconOutline className="h-10 w-10 text-red-500 dark:text-white" />

<BellIconSolid className="h-10 w-10 text-gray-500 dark:text-blue-500" />

<ChevronLeftIconSolid
  className="h-10 w-10 text-yellow-300 dark:text-white"
/>
</div>

```svelte
<script>
import {
  TicketIconOutline,
  CameraIconOutline,
  BellIconSolid,
  ChevronLeftIconSolid,
} from "@codewithshin/svelte-heroicons";
</script>

<TicketIconOutline className="h-10 w-10 text-blue-500 dark:text-yellow-300" />

<CameraIconOutline className="h-10 w-10 text-red-500 dark:text-white" />

<BellIconSolid className="h-10 w-10 text-gray-500 dark:text-blue-500" />

<ChevronLeftIconSolid
  className="h-10 w-10 text-yellow-300 dark:text-white"
/>
```

<h1 class="text-3xl w-full dark:text-white pb-8">References</h1>

<p class="w-full dark:text-white text-base"><a href="https://github.com/shinokada/svelte-heroicons" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">- Svelte-heroicons</a></p>

<p class="w-full dark:text-white text-base"><a href="https://heroicons.com/" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">- Heroicons</a></p>

