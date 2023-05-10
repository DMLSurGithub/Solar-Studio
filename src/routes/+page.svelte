<script>
	import './styles.css';
	import img1 from '../lib/images/img1.png'
	import trailer from '../lib/images/trailer.mp4'
</script>

<svelte:head>
	<title>Wizards Network - Accueil</title>
	<meta name="description" content="Site officiel de Wizards Network" />
</svelte:head>

<section>
	<div class="img-container">
		<img class="img1" src={img1} alt="img1"/>
		<div class="box box-left">
			<h2>DISCORD</h2>
			<p>250 Membres</p>
		</div>
		<div class="box box-right">
			<h2>PLAY.WIZARDS-NETWORK.FR</h2>
			<p>250 Membres</p>
		</div>
	</div>	  
	<h1>Bienvenue sur <span class="wizards">Wizards</span> <span class="network">Network</span></h1>
	<div style="display:flex; flex-direction:row;">
		<div style="flex:1;">
		  <video src={trailer} width="640" height="540" controls></video>
		</div>
		<div class="presentation" style="flex:1;">
			<p>Bonjour et bienvenue sur le serveur Minecraft Bedrock édition de Wizards Network, je suis Luna, et je suis ravie de te présenter notre univers de jeu passionnant !<br><br>
				Wizards Network, comme son nom l'indique, est un lieu où la magie opère et où les joueurs peuvent s'affronter dans des modes de jeux passionnants. Nous avons actuellement deux modes de jeux : PvP Faction et Practice, où tu peux mettre tes compétences à l'épreuve en affrontant d'autres joueurs pour la suprématie de ta faction.<br><br>
				Mais ce n'est pas tout, nous sommes également en train de préparer l'arrivée prochaine du mode de jeu SkyBlock, où tu pourras construire ta propre île dans le ciel et explorer de nouveaux horizons.<br><br>
				Sur notre serveur, nous avons également une boutique où tu peux acheter des objets à un prix abordable pour t'aider à progresser plus rapidement et à te démarquer des autres joueurs. N'hésite pas à <a href="https://wizards-network-boutique.tebex.io/" target="_blank">y faire un tour</a> et à soutenir notre serveur en faisant des achats !<br><br>
				Enfin, notre communauté est chaleureuse et accueillante, et nous avons des membres du personnel compétents pour t'aider en cas de besoin. Nous organisons également des événements réguliers pour que tu puisses t'amuser avec les autres joueurs.<br><br>
				Alors, <a href="https://discord.gg/wizardsmc" target="_blank">rejoins-nous</a> dès maintenant sur Wizards Network et découvre un monde magique et passionnant qui t'attend !</p>
		  </div>
	  </div>	  
</section>

<style>
	section {
  		display: flex;
  		flex-direction: column;
  		justify-content: center;
  		align-items: center;
  		flex: 0.6;
	}

	.img-container {
		position: relative;
  		display: flex;
  		justify-content: center;
	}

	.img1 {
		filter: blur(2px) brightness(75%);
		width: 100vw;
		height: 36vw;
	}

	.box {
		position: absolute;
		bottom: 0;
		width: 240px;
		height: 70px;
		border-radius: 0 0 20px 20px;
	}

	.box-left {
		left: 0;
		margin-left: 40px;
		margin-bottom: 35px;
		padding: 10px;
		background: linear-gradient(210deg, #5453b0aa, #161466aa);
        font-size: 14px;
        border-radius: 20px;
        color: rgb(255, 255, 255);
	}

	.box-right {
		right: 0;
		margin-right: 40px;
		margin-bottom: 35px;
		padding: 10px;
		background: linear-gradient(-210deg, #7473e8aa, #26249caa);
        font-size: 14px;
        border-radius: 20px;
        color: rgb(255, 255, 255);
	}

	h2 {
		font-size: 16px;
	}
	
	h1 {
		font-size: 30px;
		font-family: 'Outfit', 'sans serif';
		font-weight: bold;
	}

	.wizards {
		color: #5553d7;
	}

	.network {
		color: #f0b810;
	}

	.presentation {
		margin-left: 10px;
		margin-top: 5px;
	}

	p {
		font-size: 12px;
	}
</style>