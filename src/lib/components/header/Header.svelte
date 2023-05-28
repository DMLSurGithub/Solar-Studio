<script>
	import { page } from '$app/stores';
	import Icone from '../../images/icon.png';
  import { onMount } from 'svelte';

  onMount(() => {
    const menuItems = document.querySelectorAll('nav ul li');

    menuItems.forEach((item) => {
      item.addEventListener('mouseenter', () => {
        item.classList.add('active');
      });

      item.addEventListener('mouseleave', () => {
        item.classList.remove('active');
      });
    });
  });
</script>

<header>
  <nav class="container">
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