<script>
  import "../../app.css";
  import "flowbite/dist/flowbite.css";
  import { DarkMode } from "svelte-flow";
</script>

<main class="container mx-auto px-4 pt-4">
  <DarkMode />
  <div class="mt-8 w-full pb-48">
    <slot />
  </div>
</main>
