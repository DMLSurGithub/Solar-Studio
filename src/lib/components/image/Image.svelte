<script>
  import img1 from '../lib/images/img1.png';
	import serveurLogo from '../lib/images/logo.png';
</script>

<svelte:head>
  <link rel="stylesheet" href="./Image.css">
</svelte:head>

<image>
  <div class="img-container">
    <img class="img1" src={img1} alt="img1"/>
    <div class="center-logo">
      <img src={serveurLogo} alt="logo" />
    </div>
  </div>
</image>