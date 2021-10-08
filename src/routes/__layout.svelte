<script>
  import Header from "$lib/header/Header.svelte";
  import "../app.css";
</script>

<template lang="pug">
	.layout
		Header
		main
			slot
		footer
			p impan.netlify.app &copy; 2021


	//- <div class="layout">
	//-   <Header />
	
	//-   <main>
	//- 	<slot />
	//-   </main>
	
	//-   <footer>
	//- 	<p>
	//- 	  visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit
	//- 	</p>
	//-   </footer>
	//- </div>
</template>

<style lang="scss" globals>
  @import "../main.scss";
  .layout {
    background: $diamond;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  main {
    flex: 1;
    display: flex;
    flex-direction: column;
    padding: 2rem 1rem;
    width: 100%;
    max-width: 1024px;
    margin: 0 auto;
    box-sizing: border-box;
  }

  footer {
    border-top: 1px solid skyblue;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: $diamond;
    opacity: 0.75;
    // color: $pure-white;

    // padding: 40px;
  }

  footer a {
    font-weight: bold;
  }

  @media (min-width: 480px) {
    footer {
      //   padding: 40px 0;
    }
  }
</style>
