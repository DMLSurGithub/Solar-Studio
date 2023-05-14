<script>
	import { page } from '$app/stores';
	import serveurIcone from '../lib/images/icon.png';
</script>

<head>
  <link rel="stylesheet" href="./Header.css">
</head>

<header>
  <header>
    <nav class="container">
      <ul>
        <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
          <a href="/">ACCUEIL</a>
        </li>
        <li class="wiki" aria-current={$page.url.pathname === '/wiki' ? 'page' : undefined}>
          <a href="/wiki">WIKI</a>
        </li>
      </ul>
      <a href="/">
        <img src={serveurIcone} alt="Serveur" />
      </a>
      <ul>
        <li class="vote" aria-current={$page.url.pathname === '/vote' ? 'page' : undefined}>
          <a href="/vote">VOTE</a>
        </li>
        <li aria-current={$page.url.pathname === '/boutique' ? 'page' : undefined}>
          <a href="https://wizards-network-boutique.tebex.io/" target="_blank">BOUTIQUE</a>
        </li>
      </ul>
		  <div class="right">
	      <a href="/connexion">CONNEXION</a>
		  </div>
	  </nav>
  </header>
</header>