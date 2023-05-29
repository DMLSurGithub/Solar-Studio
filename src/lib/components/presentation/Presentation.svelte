<script>
	import { page } from '$app/stores';
  import wallpaper from '../../images/wallpaper.jpg'
</script>

<presentation class="presentation">
  <img src={wallpaper} alt="Wallpaper" class="wallpaper"/>
  <div class="text-zone">
    <p>Texte Ici</p>
  </div>
</presentation>

<style>
	@import './Presentation.css';
</style>