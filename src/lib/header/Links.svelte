<script>
  import { page } from "$app/stores";

  const links = [
    { url: "/", label: "individuel" },
    { url: "/pancom", label: "la communauté" },
    { url: "/advices", label: "conseils" },
  ];
</script>

{#each links as { url, label }}
  <li class:active={$page.path === url}>
    <a sveltekit:prefetch href={url}>{label}</a>
  </li>
{/each}

<!-- 
<li><div class="item flex-2">Je suis:</div></li>
    <li class:active={$page.path === "/pansex"}>
      <a sveltekit:prefetch href="/pansex">Pansexuel</a>
    </li>
    <li class:active={$page.path === "/panrom"}>
      <a sveltekit:prefetch href="/panrom">Panromantique</a>
    </li>
    <li class:active={$page.path === "/todos"}>
      <a sveltekit:prefetch href="/todos">Atypique</a>
    </li>
<template lang="pug">
  +each('links as {url, label, filename}')
    if path===url
      li.active
        a(href="{url}") {label}    
    else
      li
        a(href="{url}") {label}

</template> -->
<style lang="scss">
  @import "../../main.scss";
  $background: rgba(255, 255, 255, 0.7);
  $size: 8px;

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

  a:hover {
    color: $accent-color;
  }

  li {
    position: relative;
    height: 100%;
  }
  li.active::before {
    content: "";
    width: 0;
    height: 0;
    position: absolute;
    top: 0;
    left: calc(50% - $size);
    border: $size solid transparent;
    border-top: $size solid $accent-color;
  }
</style>
