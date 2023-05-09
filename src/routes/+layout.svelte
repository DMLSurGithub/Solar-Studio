<script>
	import Header from './Header.svelte';
	import './styles.css';
	import serveurIcone from '../lib/images/icon.png';
	import discordIcone from '../lib/images/discord.png'
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

<footer style="display: flex; justify-content: space-between; align-items: center;">
  	<div style="display: flex; align-items: center;">
    	<img src={serveurIcone} alt="Serveur" />
  	</div>
  	<div style="display: flex; align-items: center;">
    	<p style="text-align: center;">By <a href="https://github.com/DMLSurGithub" target="_blank">DML</a> for Wizards Network</p>
  	</div>
  	<div style="display: flex; align-items: center;">
    	<a href="https://discord.gg/wizardsmc" target="_blank">
      		<img src={discordIcone} alt="Discord"/>
		</a>
  	</div>
</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding: 12px;
		background-color: rgb(6, 5, 7);
	}

	footer a {
		font-weight: bold;
		align-items: flex-start;
	}

	footer img {
		width: 40px;
		margin: 0px 15px
	}

	@media (min-width: 480px) {
		footer {
			padding: 3px 0;
		}
	}
</style>
