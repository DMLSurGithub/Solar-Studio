<script>
	import Header from '../../lib/components/header/Header.svelte';
	import Footer from '../../lib/components/footer/Footer.svelte';

	import Competances from '../../lib/components/services/competances/Competances.svelte';
	import Web from '../../lib/components/services/web/Web.svelte';
	import Bot from '../../lib/components/services/bot/Bot.svelte';
	import Addon from '../../lib/components/services/addon/Addon.svelte';
</script>

<svelte:head>
	<title>Solar Studio - Services</title>
	<meta name="description" content="Site officiel de Solar Studio, dessus vous pourrez retrouver des créations Web, Bot Discord et Add-Ons hors normes !" />
	<meta content="#ffbc00" data-react-helmet="true" name="theme-color"/>
</svelte:head>

<Header />

<Competances />

<Web />

<Bot />

<Addon />

<Footer />

<style>
	@import '../../styles.css';
</style>