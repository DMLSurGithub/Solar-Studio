<script>
	import { page } from '$app/stores';
	import Icone from '../../images/icon.png';
  import sun from '../../images/sun.svg'
  import moon from '../../images/moon.svg'
  import trad from '../../images/trad.svg'
</script>
<header>
  <nav class="container">
    <a href="/">
      <img class="sun-icon" src={sun} alt="Sun" />
    </a>   
    <ul>
      <li class="services" aria-current={$page.url.pathname === '/services' ? 'page' : undefined}>
        <a href="/services">SERVICES</a>
      </li>
      <li class="portfolio" aria-current={$page.url.pathname === '/portfolio' ? 'page' : undefined}>
        <a href="/portfolio">PORTFOLIO</a>
      </li>
    </ul>
    <a href="/">
      <img class="icon" src={Icone} alt="Icone" />
    </a>
    <ul>
      <li class="infos" aria-current={$page.url.pathname === '/infos' ? 'page' : undefined}>
        <a href="/infos">INFORMATIONS</a>
      </li>
      <li class="contact" aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
        <a href="/contact">CONTACTER</a>
      </li>
    </ul>
    <a href="/">
      <img class="trad-icon" src={trad} alt="Traduction" />
    </a>    
  </nav>
</header>

<style>
	@import './Header.css';
</style>