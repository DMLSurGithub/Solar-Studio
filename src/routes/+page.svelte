<script>
	import Header from '../lib/components/header/Header.svelte';
	import Presentation from '../lib/components/presentation/Presentation.svelte';
	import Footer from '../lib/components/footer/Footer.svelte';
</script>

<svelte:head>
	<title>Solar Studio - Accueil</title>
	<meta name="description" content="Site officiel de Solar Studio, dessus vous pourrez retrouver des créations Web, Bot Discord et Add-Ons hors normes !" />
	<meta content="#ffbc00" data-react-helmet="true" name="theme-color"/>
	<meta property="og:image" content="https://i.ibb.co/SP6L5ZQ/solar-studio.png" />
</svelte:head>

<Header />

<Presentation />

<Footer />

<style>
	@import '../styles.css';
</style>