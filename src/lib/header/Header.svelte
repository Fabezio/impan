<script>
  import Links from "./Links.svelte";

  import logo from "./svelte-logo.svg";
</script>

<template lang="pug">
  header
    .corner
      h3 impan
      //a(href='https://kit.svelte.dev')
        img(src='{logo}' alt='SvelteKit')
    nav
      svg(viewBox='0 0 2 3' aria-hidden='true')
        path(d='M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z')
      ul
        Links
        
      svg(viewBox='0 0 2 3' aria-hidden='true')
        path(d='M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z')
    .corner
      // TODO put something else here? github link?


</template>

<!-- <h -->
<style lang="scss">
  @import "../../main.scss";
  $background: rgba(255, 255, 255, 0.7);
  $size: 8px;
  header {
    display: flex;
    justify-content: space-between;
  }

  .corner {
    width: 3em;
    height: 3em;
    h3 {
      margin: 0.5em;
      color: $ruby;
      letter-spacing: 1px;
    }
    a {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 100%;
      height: 100%;
    }
    img {
      width: 2em;
      height: 2em;
      object-fit: contain;
    }
  }

  nav {
    display: flex;
    justify-content: center;
    a {
      display: flex;
      height: 100%;
      align-items: center;
      padding: 0 1em;
      color: $heading-color;
      font-weight: 700;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      text-decoration: none;
      transition: color 0.2s linear;
    }
  }

  a:hover {
    color: $accent-color;
  }

  svg {
    width: 2em;
    height: 3em;
    display: block;
  }

  path {
    fill: $background;
  }

  ul {
    position: relative;
    padding: 0;
    margin: 0;
    height: 3em;
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    background: $background;
    background-size: contain;
  }
</style>
