---
layout: doc
---

<script>
  import { List } from "svelte-flow";
  import {UserCircleIconSolid, CloudDownloadIconSolid, AdjustmentsIconSolid, InboxIconSolid } from '@codewithshin/svelte-heroicons'

  let lists = [
    {
      title: "Home",
      link: "/",
    },
    {
      title: "Alerts",
      link: "/alert",
    },
    {
      title: "Cards",
      link: "/cards",
    },
    {
      title: "List Group",
      link: "/list-group/list",
    },
    {
      title: "Modals",
      link: "/modals",
    },
    {
      title: "Tabs",
      link: "/tabs",
    },
  ];
  let list2 = [
    {
      title: "Profile",
      icons:"UsericonCircleSolid",
      link: "/",
    },
    {
      title: "Settings",
      icons:"AdjustmentsIconSolid",
      link: "/",
    },
    {
      title: "Messages",
      icons:"InboxIconSolid",
      link: "/",
    },
    {
      title: "Download",
      icons:"CloudDownloadIconSolid",
      link: "/",
    },
   
  ];
</script>

<h1 class="text-3xl w-full dark:text-white">List group</h1>

<div
  class="container flex flex-wrap space-x-8 justify-center rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6"
>
 <List {lists} />
</div>


```svelte
<script>
  import { List } from "svelte-flow";

  let lists = [
    {
      title: "Home",
      link: "/",
    },
    {
      title: "Alerts",
      link: "/alert",
    },
    {
      title: "Cards",
      link: "/cards",
    },
    {
      title: "List Group",
      link: "/list-group/list",
    },
    {
      title: "Modals",
      link: "/modals",
    },
    {
      title: "Tabs",
      link: "/tabs",
    },
  ];
</script>
````

<div
  class="container flex flex-wrap space-x-8 justify-center rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6"
>
  <List />
</div>
