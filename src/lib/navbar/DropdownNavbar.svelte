<script>
  import { page } from "$app/stores";

  let hidden = true;
  let block = false;
  let activeDropdown = undefined;
  const handleDropdown = (dropdown) => {
    console.log("dropdown.id", dropdown.id);
    hidden = !hidden;
    block = !block;
    activeDropdown = dropdown.id;
    console.log("activeDropdown: ", activeDropdown);
  };

  let barHidden = true;
  const handleClickbtn = () => {
    barHidden = !barHidden;
  };

  export let sitename = "Svelte Flow";
  export let logo = "/images/mkdir-logo.png";
  export let alt;
  export let textsize = "text-sm";
  export let menus = [
    {
      id: 1,
      name: "Home",
      link: "/",
      rel: undefined,
    },
    {
      id: 2,
      name: "Alerts compoenents",
      link: "/alerts",
      rel: undefined,
    },
    {
      id: 3,
      name: "Component 1",
      link: "/",
      rel: undefined,
      child: [
        {
          id: 4,
          name: "Modals compoenents",
          link: "/modals",
          rel: undefined,
        },
        {
          id: 5,
          name: "Navbar compoenents",
          link: "/navbar",
          rel: undefined,
        },
        {
          id: 6,
          name: "Tabs",
          link: "/tabs",
          rel: undefined,
        },
      ],
    },
    {
      id: 7,
      name: "Component 2",
      link: "/",
      rel: undefined,
      child: [
        {
          id: 8,
          name: "Modals",
          link: "/modals",
          rel: undefined,
        },
        {
          id: 9,
          name: "Navbar",
          link: "/navbar",
          rel: undefined,
        },
        {
          id: 10,
          name: "Tabs",
          link: "/tabs",
          rel: undefined,
        },
      ],
    },
    {
      id: 11,
      name: "List Group",
      link: "/list-group",
      rel: undefined,
    },
  ];
</script>

<nav
  class="px-2 bg-white border-gray-200 dark:bg-gray-800 dark:border-gray-700"
>
  <div class="container flex flex-wrap justify-between items-center mx-auto">
    <a href="/" class="flex">
      <img src={logo} {alt} />
      <span
        class="self-center text-lg font-semibold text-gray-900 whitespace-nowrap dark:text-white"
        >{sitename}</span
      >
    </a>
    <button
      on:click={handleClickbtn}
      type="button"
      class="inline-flex justify-center items-center ml-3 text-gray-400 rounded-lg md:hidden hover:text-gray-900 focus:outline-none focus:ring-2 focus:ring-blue-300 dark:text-gray-400 dark:hover:text-white dark:focus:ring-gray-500"
      aria-controls="mobile-menu-2"
      aria-expanded="false"
    >
      <span class="sr-only">Open main menu</span>
      <svg
        class="w-6 h-6"
        fill="currentColor"
        viewBox="0 0 20 20"
        xmlns="http://www.w3.org/2000/svg"
        ><path
          fill-rule="evenodd"
          d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
          clip-rule="evenodd"
        /></svg
      >
      <svg
        class="hidden w-6 h-6"
        fill="currentColor"
        viewBox="0 0 20 20"
        xmlns="http://www.w3.org/2000/svg"
        ><path
          fill-rule="evenodd"
          d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
          clip-rule="evenodd"
        /></svg
      >
    </button>
    <div
      class="w-full md:block md:w-auto"
      class:hidden={barHidden}
      id="mobile-menu"
    >
      <ul
        class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium"
      >
        {#each menus as { id, name, link, rel, child }}
          {#if child}
            <li>
              <button
                on:click={handleDropdown({ id })}
                class="flex justify-between items-center py-2 pr-4 pl-3 w-full {textsize} font-medium text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-gray-400 dark:hover:text-white dark:focus:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent"
                >{name}
                <svg
                  class="ml-1 w-4 h-4"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                  ><path
                    fill-rule="evenodd"
                    d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                    clip-rule="evenodd"
                  /></svg
                ></button
              >
              {#if activeDropdown === id}
                <!-- Dropdown menu -->
                <div
                  class:hidden
                  class:block
                  class="z-10 w-44 text-base list-none bg-white rounded divide-y divide-gray-100 shadow dark:bg-gray-700 dark:divide-gray-600"
                  style="position: absolute; margin: 0px;"
                >
                  <ul class="py-1" aria-labelledby="dropdownLargeButton">
                    {#each child as item}
                      <li>
                        <a
                          href={item.link}
                          {rel}
                          class="block py-2 px-4 text-{textsize} text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white"
                          >{item.name}</a
                        >
                      </li>
                    {/each}
                  </ul>
                </div>
              {/if}
            </li>
          {:else}
            <li>
              <a
                class:active={$page.url.pathname === link}
                href={link}
                {rel}
                class="block py-2 pr-4 pl-3  text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-gray-400 dark:hover:text-white dark:border-gray-700 dark:hover:bg-gray-700 md:dark:hover:bg-transparent {textsize}"
                >{name}</a
              >
            </li>
          {/if}
        {/each}
      </ul>
    </div>
  </div>
</nav>

<style>
  #mobile-menu .active {
    color: #fab534;
  }
</style>
