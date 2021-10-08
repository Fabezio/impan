<script>
  export let pageTitle
</script>

<template lang="pug">
	svelte:head
		title impan | {pageTitle}
	//- </svelte:head>
	h1 {pageTitle}
	
</template>