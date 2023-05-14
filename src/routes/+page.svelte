<script>
	import Header from '../lib/components/header/Header.svelte';
	import Image from '../lib/components/image/Image.svelte';
	import Bienvenue from '../lib/components/bienvenue/Bienvenue.svelte';
	import Discord from '../lib/components/discord/Discord.svelte';
	import Footer from '../lib/components/footer/Footer.svelte';
</script>

<svelte:head>
	<title>Wizards Network - Accueil</title>
	<meta name="description" content="Site officiel du serveur Minecraft Bedrock, Wizards Network, celui-ci est sur le thème High Fantasy et comporte deux modes de jeux, un PvP Faction et un Practice" />
	<meta content="#5553d7" data-react-helmet="true" name="theme-color"/>
	<meta content="/lib/images/img1.png" property="og:image"/>
</svelte:head>

<Header />

<Image />

<Bienvenue />

<Discord />

<Footer />

<style>
	@import '../styles.css';
</style>