<script context="module">
  export const prerender = true;
</script>

<script>
	import Article from '$lib/contents/Article.svelte'

</script>

<template lang="pug">
	svelte:head
		title Accueil
	//- </svelte:head>
	h1 Être pansexuel
	Article(title='Non, je ne suis ni hétéro ni homo. Voici pourquoi.')
		p
			| D'abord, une orientation sexuelle est unique: on n'est pas gay à temps partiel; pour ma part j'ai des phases transitoires. Bien que cela ne se voie absolument pas, j'ai une personnalité mixte: à la fois féminine et masculine. J'aime les deux sexes primaires ainsi que les représentants du troisième genre.
		p.parag2
			| Imaginez avoir des rapports avec deux personnes de sexes différents: quelle orientation décrirait alors vos ébats? absolument aucune; ça tombe sous le sens. Bien entendu, je ne dis pas que j'ai des rapports mixtes, ce n'est qu'une illustration.
	Article(title="J'assume pleinement")
		p
			| Comment je m'habille, quelles sont mes préférences, [b est-ce que j'assume mon côté féminin]? Oui, pleinement; sans toutefois me déguiser: je n'en éprouve pas le besoin. Je suis la plupart du temps en jean-baskets, je ne porte pas de dessous affriolants, encore moins féminins. Pourtant, je suis naturel sans que cela interpelle. Je croise les bras dans la rue la moitié du temps. Au niveau de l'élocution, j'ai une voix fluette et des inflexions qu'on pourrait qualifier d'empruntées. Je n'ai cependant rien d'[em efféminé].
	Article(title='Quid de mes rapports?')
		p J'ai une attirance naturelle pour les femmes, et bien que j'aime les poitrines généreuses, je préfère que ma partenaire soit sensuelle avec de petits bonnets plutôt que l'inverse.
		p
			| J'ai également besoin d'une présence masculine, mon corps le réclame: il me faut une épaule pour me reposer, des mains pour me caresser, j'ai aussi besoin de passer mes bras autour de son cou, le prendre en main, le recevoir (avec douceur: je m'en fous qu'il assure et soit capable de tenir une heure; moi aussi j'ai besoin de plaisir, de me laisser aller, de perdre le contrôle.)
	Article(title='Je ne suis pas <em>devenu</em> pansexuel')
		p
			| Pour que les choses soient bien claires: je n'ai pas choisi cette orientation: je l'ai découverte. On ne [q se fait] pas gay, c'est une erreur répandue, un amalgame dû à la méconnaissance du milieu. Encore une fois, l'homosexualité est une orientation indépendante de la nôtre.

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
