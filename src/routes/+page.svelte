<script>
	import Header from '../lib/components/header/Header.svelte';
	import Presentation from '../lib/components/home/presentation/Presentation.svelte';
	import Team from '../lib/components/home/team/Team.svelte';
	import Partenaires from '../lib/components/home/partenaires/Partenaires.svelte';
	import Reviews from '../lib/components/home/reviews/Reviews.svelte';
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

<Team />

<Partenaires />

<Reviews />

<Footer />

<style>
	@import '../styles.css';
</style>