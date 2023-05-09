<script>
	import './styles.css';
	import img1 from '../lib/images/img1.png'
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
	<h1>Bienvenue sur Wizards Network</h1>
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
		background: linear-gradient(210deg, #7473e8aa, #26249caa);
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
	}
</style>