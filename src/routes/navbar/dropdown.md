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
        {
          name: "Horizontal Card",
          link: "/cards/horizontal",
          rel: "external",
        },
        {
          name: "Interactive Card",
          link: "/cards/interactive",
          rel: "external",
        },
        {
          name: "List Card",
          link: "/cards/list",
          rel: "external",
        },
      ],
    },
    {
      name: "Darkmode",
      link: "/darkmode",
      rel: "external",
    },
    {
      name: "List Group",
      link: "/list-group",
      rel: "external",
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
        {
          name: "Large",
          link: "/modals/large",
          rel: "external",
        },
        {
          name: "Extra-large",
          link: "/modals/extra-large",
          rel: "external",
        },
        {
          name: "Signin",
          link: "/modals/signin",
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
          name: "Navbar",
          link: "/navbar",
          rel: "external",
        },
        {
          name: "Dropdown Navbar",
          link: "/navbar/dropdown",
          rel: "external",
        },
       
      ],
    },
    {
      name: "Tabs",
      link: "/",
      rel: "external",
      child: [
        {
          name: "Default",
          link: "/tabs/default",
          rel: "external",
        },
        {
          name: "Interactive",
          link: "/tabs/interactive",
          rel: "external",
        },
        {
          name: "Multiple Interactive",
          link: "/tabs/multiple-interactive-tabs",
          rel: "external",
        },
        {
          name: "Pilltabs",
          link: "/tabs/pilltabs",
          rel: "external",
        },
      ],
    },
  ];
</script>

<h1 class="text-3xl w-full dark:text-white">Dropdown Navbar Setup</h1>


<DrowdownNavbar textsize="lg" {menus} />


```svelte
<script>
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
        {
          name: "Horizontal Card",
          link: "/cards/horizontal",
          rel: "external",
        },
        {
          name: "Interactive Card",
          link: "/cards/interactive",
          rel: "external",
        },
        {
          name: "List Card",
          link: "/cards/list",
          rel: "external",
        },
      ],
    },
    {
      name: "Darkmode",
      link: "/darkmode",
      rel: "external",
    },
    {
      name: "List Group",
      link: "/list-group",
      rel: "external",
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
        {
          name: "Large",
          link: "/modals/large",
          rel: "external",
        },
        {
          name: "Extra-large",
          link: "/modals/extra-large",
          rel: "external",
        },
        {
          name: "Signin",
          link: "/modals/signin",
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
          name: "Navbar",
          link: "/navbar",
          rel: "external",
        },
        {
          name: "Dropdown Navbar",
          link: "/navbar/dropdown",
          rel: "external",
        },
       
      ],
    },
    {
      name: "Tabs",
      link: "/",
      rel: "external",
      child: [
        {
          name: "Default",
          link: "/tabs/default",
          rel: "external",
        },
        {
          name: "Interactive",
          link: "/tabs/interactive",
          rel: "external",
        },
        {
          name: "Multiple Interactive",
          link: "/tabs/multiple-interactive-tabs",
          rel: "external",
        },
        {
          name: "Pilltabs",
          link: "/tabs/pilltabs",
          rel: "external",
        },
      ],
    },
  ];
</script>
```

<h2 class="text-lg mt-8 dark:text-white">Text Sizes</h2>

You can change `textsize` prop to `xs`, `sm`, `base`, `lg` or `xl`.





