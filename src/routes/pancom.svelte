
<script>
	import Article from '$lib/contents/Article.svelte'

</script>

<template lang="pug">
	svelte:head
		title Conseils
	//- </svelte:head>
	h1 La communanuté pan
	Article(title='Idée reçue: les homos ont plus de facilité que les hétéros avec les bi et pansexuels')
		p
			| Rien n'est plus faux: la panphobie vient des représentants des deux orientations, de même que la biphobie. C'est bien plus répandu qu'on ne le croit chez ceux que j'appelle les monosexuels (personnes à orientation unique). Il y a plusieurs choses à prendre en compte. Notez que je parle à la première personne pour souligner notre naturel commun.
		ul
			li
				| D'abord l'instinct de [em propriété]. Bien que notre conjoint soit une personne à part entière, on agit de manière contre intuitive en la traitant comme si elle nous appartenait, ce qui bien sûr n'est pas le cas; dans toute relation, il doit y avoir communication, confiance et surtout: respect de sa personne et de sa liberté. Bien entendu, cela doit être réciproque.
			li
				| Ensuite, on part du principe que notre moitié, si elle a une aventure, nous humiliera encore plus si elle va voir le sexe [q ennemi] , ce qui est parfaitement irrationnel.
			li
				| Enfin, étant unisexuels, ces derniers ne peuvent simplement pas concevoir que l'on soit également bien avec l'autre sexe sans qu'il ait pour autant une quelconque notion de trahison: c'est un besoin vital pour notre équilibre. De plus ça peut permettre de se retrouver avec une expérience enrichie.
			li
				| Dernier point, celui-ci complétant les précédents: les relations à plusieurs sont courantes dans la plupart des cultures et bien souvent condamnées par les lois occidentales. Si nous avions plus de respect à l'égard de la gent féminine ou simplement de nos partenaires en général, notre nature n'en pâtirait pas.
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
