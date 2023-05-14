<script>
	import './styles.css';
	import img1 from '../lib/images/img1.png';
	import serveurIcone from '../lib/images/icon.png';
	import serveurLogo from '../lib/images/logo.png';
	import trailer from '../lib/images/trailer.mp4';
</script>

<svelte:head>
	<title>Wizards Network - Accueil</title>
	<meta name="description" content="Site officiel du serveur Minecraft Bedrock, Wizards Network, celui-ci est sur le thème High Fantasy et comporte deux modes de jeux, un PvP Faction et un Practice" />
	<meta content="#5553d7" data-react-helmet="true" name="theme-color"/>
	<meta content="/lib/images/img1.png" property="og:image"/>
</svelte:head>

<section>
	<div class="img-container">
		<img class="img1" src={img1} alt="img1"/>
		<div class="center-logo">
			<img src={serveurLogo} alt="logo" />
		</div>
	</div>		  
	<h1>Bienvenue sur <span class="wizards">Wizards</span> <span class="network">Network</span></h1>
	<div style="display:flex; flex-direction:row; align-items: center;">
		<div style="flex:1;">
			<video src={trailer} width="640" height="390" controls>
				<track kind="captions">
			</video>	  
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
	  <h1>Connexion</h1>

	  <h1>Discord</h1>
		<div id="discordInvite" style="width: 400px;">
		  <h5 id="introText" class="noselect loadHidden" style="display: block;">Rejoins notre Discord !</h5>
		  <div id="discordData">
			<div id="serverImg" class="discordLink loadHidden" style="background: url(&quot;https://i.ibb.co/LZyHc54/partner1.png&quot;) 50% 50% / 100% 100% repeat scroll padding-box padding-box rgb(54, 57, 63); display: block;">
			</div>
			<div id="discordInfo">
			  <div id="serverNameBox" class="discordLink">
				<span class="noselect" id="serverName">Wizards Network</span>
			  </div>
			  <div id="status" class="loadHidden" style="display: block;">
				<div id="statusIndicators" class="noselect">
				  <i id="onlineInd"></i>
				  <span id="numOnline">76 En ligne</span>
				  <i id="offlineInd"></i>
				  <span id="numTotal">259 Membres</span>
				</div>
			  </div>
			</div>
			<button type="button" class="discordLink" id="callToAction">
			  <div id="buttonText" class="noselect"><a href="https://discord.gg/wizardsmc" target="_blank">Rejoindre</a></div>
			</button>
		  </div>
		</div>

	  <h1>Actualités</h1>
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

	@media only screen and (max-width: 768px) {
	.img1 {
		filter: blur(2px) brightness(75%);
		width: 10vw;
		height: 42vw;
	}
}

@media only screen and (min-width: 769px) and (max-width: 1024px) {
	.img1 {
		filter: blur(2px) brightness(75%);
		width: 200vw;
		height: 42vw;
	}
}

@media only screen and (min-width: 1025px) {
	.img1 {
		filter: blur(2px) brightness(75%);
		width: 100vw;
		height: 42vw;
	}
}

	.center-logo {
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);
}

.center-logo img {
	width: 750px;
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

	#discordData,#discordInfo {
    display: flex;
    height: 50px
}

#discordInvite {
    text-align: left;
    box-sizing: border-box;
    color: #fff;
    background: #2b2d31;
    border-radius: 15px;
    border: 1px solid rgba(47,49,54,.9);
    border-collapse: separate;
    font: normal normal 400 normal 16px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    margin: 0;
    padding: 10px 15px 10px 10px;
    display: inline-block
}

#offlineInd,#onlineInd {
    height: 8px;
    width: 8px;
    border-radius: 50%;
    margin: 0 4px 0 0;
    display: block
}

#introText {
    color: #b9bbbe;
    height: 16px;
    letter-spacing: .5px;
    text-transform: uppercase;
    flex: 1 1 0%;
    font: normal normal 600 normal 12px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    margin: 0 0 8px
}

#serverImg {
    background-position: 50% 50%;
    bottom: 0;
    height: 50px;
    left: 0;
    position: relative;
    right: 0;
    top: 0;
    width: 50px;
    border-radius: 15px;
    flex: 0 0 auto;
    margin: 0 10px 0 0
}

#discordInfo {
    align-items: stretch;
    justify-content: center;
    flex: 1 1 auto;
    flex-flow: column nowrap
}

#callToAction,#statusIndicators {
    align-items: center;
    display: flex
}

#serverNameBox {
    color: #f6f6f7;
    height: 20px;
    font: normal normal 600 normal 16px/20px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    margin: 0 0 4px
}


#onlineInd {
    color: #72767d;
    column-rule-color: #72767d;
    background: #43b581;
    font: italic normal 600 normal 12px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif
}

#numOnline {
    color: #72767d;
    display: block;
    height: 16px;
    font: normal normal 600 normal 12px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    margin: 0 8px 0 0
}

#offlineInd {
    color: #72767d;
    background: #747f8d;
    font: italic normal 600 normal 12px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif
}

#numTotal {
    color: #72767d;
    display: block;
    height: 16px;
    font: normal normal 600 normal 12px/16px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif
}

#callToAction {
    color: #fff;
    cursor: pointer;
    border: 0;
    justify-content: center;
    background: #248046;
    border-radius: 3px;
    font: normal normal 500 normal 14px/20px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    transition: background-color .17s ease 0s
}

#callToAction:hover {
    background-color: #1a6334
}

#buttonText a {
	color: #fff;
	text-decoration: none;
}

#buttonText {
    cursor: pointer;
    display: flex;
    height: 20px;
    text-align: center;
    font: normal normal 500 normal 14px/20px Whitney,"Helvetica Neue",Helvetica,Arial,sans-serif;
    margin: 0 8.83px
}

.loadHidden {
    display: none
}
</style>