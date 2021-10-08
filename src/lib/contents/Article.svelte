<script>
  export let title;
  //   export let content;
</script>

<article>
  <header><h2 class="article__title">{@html title}</h2></header>
  <!-- {@html content} -->
  <slot />
</article>

<style lang="scss">
  @import "../../main.scss";
  h2 {
    font-size: 1.75rem;
    font-weight: 300;
  }
</style>
