<script>
	import { page } from '$app/stores';
	import serveurIcone from '../lib/images/icon.png';

</script>
  
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

  <style>
	
  nav.container {
    display: flex;
	justify-content: center;
    align-items: center;
    background-color: black;
    padding-top: 10px;
  }
  
  nav ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
  }
  
  nav ul li {
    margin: 0px 30px;
    font-size: 15px;
	margin-bottom: 3px;
  }

  .wiki{
	margin-right: 60px !important; 
  }

  .vote{
	margin-left: 60px !important; 
  }

  nav ul li {
    margin: 0px 30px;
    font-size: 15px;
	margin-bottom: 3px;
  }

  nav ul li:hover {
  border-bottom: 2px solid #f1bc2c;
  margin-bottom: -3px;
}
  
  nav a {
    text-decoration: none;
    color: rgb(255, 255, 255);
    font-weight: bold;
  }
  
  nav img {
    width: 40px;
    margin-bottom: 8px;
  }
		
	.right {
	  position: absolute;
	  right: 0;
	  background: linear-gradient(45deg, #f1bc2c, #f18f2c);
      font-size: 15px;
    margin-bottom: 10px;
      border-radius: 20px;
      padding: 10px 20px;
	  margin-right: 10px;
      color: rgb(255, 255, 255);
      font-weight: bold;
      cursor: pointer;
	}
  </style>