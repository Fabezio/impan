<script>
  export let title;
  //   export let content;
</script>

<article>
  <header><h2 class="article__title">{@html title}</h2></header>
  <!-- {@html content} -->
  <slot />
</article>
