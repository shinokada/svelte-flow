---
layout: doc
---

<script>
  import { DropdownNavbar } from "svelte-flow";

  let menus = [
    {
      name: "Home",
      link: "/",
      rel: "external",
    },
    {
      name: "Cards",
      link: "/cards",
      rel: "external",
      child: [
        {
          name: "Card",
          link: "/cards/card",
          rel: "external",
        },
        {
          name: "CTA Card",
          link: "/cards/cta",
          rel: "external",
        },
        {
          name: "Ecommerce Card",
          link: "/cards/ecommerce",
          rel: "external",
        },
      ],
    },
    {
      name: "Modals",
      link: "/",
      rel: "external",
      child: [
        {
          name: "Small",
          link: "/modals/small",
          rel: "external",
        },
        {
          name: "Medium",
          link: "/modals/medium",
          rel: "external",
        },
      ],
    },
  ];
</script>



<h1 class="text-3xl w-full dark:text-white pb-8">Dropdown Navbar</h1>

<div class="container w-full rounded-xl my-4 mx-auto bg-gradient-to-r bg-white dark:bg-gray-900 border border-gray-200 dark:border-gray-700 p-2 sm:p-6">
  <DropdownNavbar textsize="text-lg" {menus} />
</div>

<p class="dark:text-white text-lg">
  You can change textsize prop to text-xs, text-sm, text-base, text-lg or text-xl.
</p>

<h1 class="text-3xl w-full dark:text-white py-8">Dropdown Navbar Setup</h1>

```svelte
import { DropdownNavbar } from "svelte-flow";

let menus = [
  {
    name: "Home",
    link: "/",
    rel: "external",
  },
  {
    name: "Alerts",
    link: "/alerts",
    rel: "external",
  },
  {
    name: "Buttons",
    link: "/buttons",
    rel: "external",
    child: [
      {
        name: "Card",
        link: "/cards/card",
        rel: "external",
      },
      {
        name: "CTA Card",
        link: "/cards/cta",
        rel: "external",
      },
      {
        name: "Ecommerce Card",
        link: "/cards/ecommerce",
        rel: "external",
      },
    ],
  },
  {
    name: "Modals",
    link: "/",
    rel: "external",
    child: [
      {
        name: "Small",
        link: "/modals/small",
        rel: "external",
      },
      {
        name: "Medium",
        link: "/modals/medium",
        rel: "external",
      },
    ],
  },
];

<DropdownNavbar textsize="text-lg" {menus} />
```




