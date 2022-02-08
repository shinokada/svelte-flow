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
  ];
</script>

<h1 class="text-3xl w-full dark:text-white">Dropdown Navbar Setup</h1>

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
  ];
```



<DropdownNavbar textsize="lg" {menus} />

<h2 class="text-lg mt-8 dark:text-white">Text Sizes</h2>

<p class="dark:text-white">
  You can change `textsize` prop to `xs`, `sm`, `base`, `lg` or `xl`.
</p>
