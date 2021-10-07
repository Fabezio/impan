
<script>
	import Article from '$lib/contents/Article.svelte'

</script>

<template lang="pug">
	svelte:head
		title Conseils
	//- </svelte:head>
	h1 Conseils
	Article(title='<q>Et mon coming-out, alors?</q>')
		p
			| Sujet épineux: comme pour toute orientation exotique, (entendez par là: non hétéro), c'est à vous de voir à qui vous pouvez ou voulez vous dévoiler.
		ul
			li
				h3 Les parents
				p
					| C'est le plus délicat: Comment expliquer à maman et papa qu'on aime aussi les gens du même sexe? Doit-on absolument le faire? Si l'un d'eux est ouvertement homophobe, ce n'est même pas la peine d'essayer, vous vous exposeriez à la moins informelle des évictions, et le plus souvent en silence.
					br
					| Si votre parent est mystérieux, ce n'est pas plus simple. Mais méfiez-vous du classique [q Tu es mon enfant, tant que tu es heureux/heureuse...] : c'est la déclaration la plus hypocrite du monde. Si un tel propos vous parvient, évitez de présenter votre conjoint, la situation pourrait devenir explosive.
			li
				h3 Les amis
				p
					| C'est justement là que vous allez pouvoir faire le tri. Ce sont vos amis, n'hésitez pas! Cependant, si l'un d'eux change d'attitude (même subtilement) alors même qu'il vous a affirmé que cela ne changeait rien, c'est qu'il n'est pas honnête. Il se peut qu'il ait besoin d'être rassuré, aussi parlez-en à coeur ouvert. Si la démarche s'avère infructueuse, pas la peine de le mettre en tête de liste de vos confidents, il pourrait se crisper.


</template>


<style lang='scss'> 
  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 1;
  }

  h1 {
    width: 100%;
  }

  .welcome {
    position: relative;
    width: 100%;
    height: 0;
    padding: 0 0 calc(100% * 495 / 2048) 0;
	img {
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  top: 0;
	  display: block;
	}
  }

</style>
