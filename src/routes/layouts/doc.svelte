<script>
  import Prism from "prismjs";
  import "prismjs/themes/prism.css";
  import "prism-themes/themes/prism-holi-theme.css";
  import Comments from "./Comments.svelte";
</script>

<div class="max-w-3xl mx-auto pb-32">
  <div class="container mt-4 flex flex-wrap mx-auto pt-16">
    <slot />
    <Comments />
  </div>
</div>
