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

<h1 class="text-3xl w-full dark:text-white">HeroIcons</h1>

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

<p class="dark:text-white text-base"><a href="https://github.com/shinokada/svelte-heroicons" target="_blank" class="text-blue-600 hover:underline dark:text-blue-500">- Svelte-heroicons</a></p>


