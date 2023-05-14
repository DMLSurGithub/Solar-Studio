<svelte:head>
  <link rel="stylesheet" href="./Discord.css">
</svelte:head>

<discord>
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
</discord>