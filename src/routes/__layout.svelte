<script>
  import "../app.css";
  import "flowbite/dist/flowbite.css";
  import { DarkMode } from "svelte-flow";
  import {
    Aside,
    Nav,
    SidebarList,
    Navbar,
  } from "@codewithshin/svelte-sidebar";

  import {
    accordions,
    // alerts,
    buttons,
    cards,
    // darkmode,
    // icons,
    // list_group,
    modals,
    navbar,
    svelteflows,
    tabs,
    topMenus,
  } from "./items.js";

  // Navbar
  let activeChildLi =
    "block py-2 px-4 text-lg text-gray-700 hover:bg-gray-100 dark:text-white";
  let childLi =
    "block py-2 pr-4 pl-3  text-gray-700 border-b border-gray-100 md:border-0 md:p-0 text-lg dark:text-white";
  let headerClass =
    "px-8 bg-white h-16 pt-3 text-gray-600 border-b-2 bg-white dark:bg-gray-800 dark:text-white dark:border-b-1";
  let siteName = "Svelte Flow";
  let navClass =
    "py-0 px-8 bg-white text-lg bg-white dark:bg-gray-800 dark:text-white";
  let navDivClass = "pb-4";
  let navDivClasslast = "pb-24";
  let siteClass = " pt-1.5 pl-12 w-full";
  let siteText = "text-lg";
  let topli =
    "block py-2 pr-4 pl-3 text-gray-700 md:border-0  md:p-0 dark:text-gray-300  dark:hover:bg-gray-700  text-lg z-50 dark:bg-gray-800 dark:border-0";
  let topMenuDiv =
    "container flex flex-wrap justify-end items-center mx-auto dark:bg-gray-800";
  let topul =
    "flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-md md:font-medium pt-1 dark:bg-gray-800";
  // Others
  let asideClass =
    "absolute w-auto bg-white pt-8 shadow-lg z-50 px-4 h-full bg-white dark:bg-gray-800";
  let darkmodebtn =
    "text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-lg p-2.5 fixed left-2 top-20 z-50";
  // activeDropdownDiv, activeChildLi, buttonClass, dropdownLi
</script>

<Navbar
  {activeChildLi}
  {childLi}
  {headerClass}
  {siteClass}
  {siteName}
  {siteText}
  {topMenus}
  {topMenuDiv}
  {topul}
  {topli}
/>
<Aside {asideClass}>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/" rel="">Svelte-Flow</a></h3>
    {#each svelteflows as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/accordions">Accordions</a></h3>
    {#each accordions as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/alerts">Alerts</a></h3>
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/buttons">Buttons</a></h3>
    {#each buttons as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/cards">Cards</a></h3>
    {#each cards as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/darkmode">Dark mode</a></h3>
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/icons">Icons</a></h3>
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/list-group">List group</a></h3>
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/modals">Modals</a></h3>
    {#each modals as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} {navDivClass}>
    <h3 class="text-base pb-4"><a href="/navbars">Navbar</a></h3>
    {#each navbar as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
  <Nav {navClass} navDivClass={navDivClasslast}>
    <h3 class="text-base pb-4"><a href="/tabs">Tabs</a></h3>
    {#each tabs as { url, name, rel }}
      <SidebarList {url} {name} {rel} />
    {/each}
  </Nav>
</Aside>

<main class="container mx-auto px-4 pt-4">
  <DarkMode btnClass={darkmodebtn} />
  <div class="mt-4 w-full">
    <slot />
  </div>
</main>
