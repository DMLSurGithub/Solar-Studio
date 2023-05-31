<script>
  import dml from '../../../images/dml.gif';
  import unknown from '../../../images/unknown.png';

  const images = document.querySelectorAll('.circle-image');
const arrowLeft = document.querySelector('.arrow-left');
const arrowRight = document.querySelector('.arrow-right');

let currentImage = 0;

function showImage(index) {
  images.forEach((image, i) => {
    if (i === index) {
      image.classList.add('active');
    } else {
      image.classList.remove('active');
    }
  });
}

function showNextImage() {
  currentImage = (currentImage + 1) % images.length;
  showImage(currentImage);
}

function showPreviousImage() {
  currentImage = (currentImage - 1 + images.length) % images.length;
  showImage(currentImage);
}

arrowLeft.addEventListener('click', showPreviousImage);
arrowRight.addEventListener('click', showNextImage);

showImage(currentImage);
</script>

<equipe class="equipe">
  <h2>EQUIPE :</h2>
  <div class="pp-zone">
    <div class="arrow-left"></div>
    <div class="circle-image active">
      <img src={dml} alt="DML">
      <p>DML</p>
    </div>
    <div class="circle-image">
      <img src={unknown} alt="Unknown">
      <p>Unknown</p>
    </div>
    <div class="circle-image">
      <img src={unknown} alt="Unknown">
      <p>Unknown</p>
    </div>
    <div class="arrow-right"></div>
  </div>
</equipe>

<style>
	@import './Equipe.css';
</style>