<script>
	import serveurIcone from '../lib/images/icon.png';
	import discordIcone from '../lib/images/discord.png'
</script>

<svelte:head>
  <link rel="stylesheet" href="./Footer.css">
</svelte:head>

<footer style="display: flex; justify-content: space-between; align-items: center;">
  <div style="display: flex; align-items: center;">
    <img src={serveurIcone} alt="Serveur" />
  </div>
  <div style="display: flex; align-items: center;">
    <p class="bydml" style="text-align: center;">By <a href="https://github.com/DMLSurGithub" target="_blank">DML</a> for Wizards Network</p>
  </div>
  <div style="display: flex; align-items: center;">
    <a href="https://discord.gg/wizardsmc" target="_blank">
      <img src={discordIcone} alt="Discord"/>
		</a>
  </div>
</footer>