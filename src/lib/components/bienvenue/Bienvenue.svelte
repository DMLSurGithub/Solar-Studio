<script>
	import trailer from '/static/images/trailer.mp4';
</script>

<svelte:head>
  <link rel="stylesheet" href="./Bienvenue.css">
</svelte:head>

<bienvenue>
  <h1>Bienvenue sur <span class="wizards">Wizards</span> <span class="network">Network</span></h1>
	<div style="display:flex; flex-direction:row; align-items: center;">
		<div style="flex:1;">
			<video src={trailer} width="640" height="390" controls>
				<track kind="captions">
			</video>	  
		</div>
		<div class="presentation" style="flex:1;">
			<p>Bonjour et bienvenue sur le serveur Minecraft Bedrock édition de Wizards Network, je suis Luna, et je suis ravie de te présenter notre univers de jeu passionnant !<br><br>Wizards Network, comme son nom l'indique, est un lieu où la magie opère et où les joueurs peuvent s'affronter dans des modes de jeux passionnants. Nous avons actuellement deux modes de jeux : PvP Faction et Practice, où tu peux mettre tes compétences à l'épreuve en affrontant d'autres joueurs pour la suprématie de ta faction.<br><br>Mais ce n'est pas tout, nous sommes également en train de préparer l'arrivée prochaine du mode de jeu SkyBlock, où tu pourras construire ta propre île dans le ciel et explorer de nouveaux horizons.<br><br>Sur notre serveur, nous avons également une boutique où tu peux acheter des objets à un prix abordable pour t'aider à progresser plus rapidement et à te démarquer des autres joueurs. N'hésite pas à <a href="https://wizards-network-boutique.tebex.io/" target="_blank">y faire un tour</a> et à soutenir notre serveur en faisant des achats !<br><br>Enfin, notre communauté est chaleureuse et accueillante, et nous avons des membres du personnel compétents pour t'aider en cas de besoin. Nous organisons également des événements réguliers pour que tu puisses t'amuser avec les autres joueurs.<br><br>Alors, <a href="https://discord.gg/wizardsmc" target="_blank">rejoins-nous</a> dès maintenant sur Wizards Network et découvre un monde magique et passionnant qui t'attend !</p>
		</div>
	</div>
</bienvenue>