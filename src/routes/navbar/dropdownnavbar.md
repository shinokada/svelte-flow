---
layout: doc
---

<script>
  import { DropdownNavbar } from "svelte-flow";
</script>

<h1 class="text-3xl w-full dark:text-white">Dropdown Navbar Setup</h1>


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
      name: "Component 1",
      link: "/",
      rel: "external",
      child: [
        {
          name: "Modals",
          link: "/modals",
          rel: "external",
        },
        {
          name: "Navbar",
          link: "/navbar",
          rel: "external",
        },
        {
          name: "Tabs",
          link: "/tabs",
          rel: "external",
        },
      ],
    },
    {
      name: "Component 2",
      link: "/",
      rel: "external",
      child: [
        {
          name: "Modals",
          link: "/modals",
          rel: "external",
        },
        {
          name: "Navbar",
          link: "/navbar",
          rel: "external",
        },
        {
          name: "Tabs",
          link: "/tabs",
          rel: "external",
        },
      ],
    },
    {
      name: "List Group",
      link: "/list-group",
      rel: "external",
    },
  ];
</script>
```

<h2 class="text-lg mt-8 dark:text-white">Text Sizes</h2>

You can change `textsize` prop to `xs`, `sm`, `base`, `lg` or `xl`.

```svelte
DropdownNavbar textsize="lg" />
```

<DrowdownNavbar textsize="lg" />


