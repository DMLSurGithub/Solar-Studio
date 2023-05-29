<script>
	import { page } from '$app/stores';
	import Icone from '../../images/icon.png';
  import sun from '../../images/sun.svg'
  import moon from '../../images/moon.svg'
  import trad from '../../images/trad.svg'

import { writable } from 'svelte/store';

const currentPageTheme = writable('clair');

const toggleTheme = () => {
  if ($currentPageTheme === 'clair') {
    $currentPageTheme = 'sombre';
  } else {
    $currentPageTheme = 'clair';
  }
};
</script>

<header>
  <nav class="container">
    <a href="/">
      <svg class="theme" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
        <use href={($currentPageTheme === 'clair') ? sun + '#sun' : moon + '#moon'} />
      </svg>
    </a>    
    <ul>
      <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
        <a href="/">ACCUEIL</a>
      </li>
      <li class="services" aria-current={$page.url.pathname === '/services' ? 'page' : undefined}>
        <a href="/services">SERVICES</a>
      </li>
    </ul>
    <a href="/">
      <img class="icon" src={Icone} alt="Icone" />
    </a>
    <ul>
      <li class="portfolio" aria-current={$page.url.pathname === '/portfolio' ? 'page' : undefined}>
        <a href="/portfolio">PORTFOLIO</a>
      </li>
      <li class="contact" aria-current={$page.url.pathname === '/contact' ? 'page' : undefined}>
        <a href="/contact">CONTACT US</a>
      </li>
    </ul>
  </nav>
</header>

<style>
	@import './Header.css';
</style>