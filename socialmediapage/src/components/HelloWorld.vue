<template>
  <div class="bgImg">
    <div class="overlay d-flex align-items-center">
      <div class="container-fluid">
        <div class="container my-5">
          <a data-mdb-ripple-init class="btn btn-primary facebookBtn" href="https://www.facebook.com/search/top?q=imperial%20detailing" role="button" target="_blank">
            <i class="fab fa-facebook me-2"></i> Facebook
          </a>
        </div>
        <div class="container my-5">
          <a data-mdb-ripple-init class="btn btn-primary instagramBtn" href="https://www.instagram.com/imperialdetailing.ro/" role="button" target="_blank">
            <i class="fab fa-instagram me-2"></i> Instagram
          </a>
        </div>
        <div class="container">
          <a data-mdb-ripple-init class="btn btn-primary tiktokBtn" href="https://www.tiktok.com/@imperialdetailingoradea" role="button" target="_blank">
            <i class="fab fa-tiktok me-2"></i> TikTok
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.bgImg {
  position: relative; /* Permite overlay-ului să se poziționeze relativ față de background */
  background-image: url('../img/atelierGol.png'); /* Asigură-te că calea este corectă */
  background-size: cover; /* Acoperă întregul spațiu disponibil */
  background-position: center; /* Centrează imaginea */
  min-height: 100vh; /* Asigură-te că fundalul acoperă întreaga înălțime */
  color: white; /* Poate vrei să schimbi culoarea textului pentru a fi vizibil pe fundal */
}

.overlay {
  position: absolute; /* Pozitioneaza overlay-ul peste background */
  top: 0; /* Aliniere sus */
  left: 0; /* Aliniere la stânga */
  right: 0; /* Aliniere la dreapta */
  bottom: 0; /* Aliniere jos */
  background-color: rgba(37, 35, 35, 0.5); /* Gri cu 50% opacitate */
  z-index: 1; /* Overlay-ul va fi sub conținut, dar deasupra fundalului */
}

/* Stiluri pentru butoane */
.facebookBtn,
.instagramBtn,
.tiktokBtn {
  transition: transform 0.3s ease; /* Adaugă tranziție pentru scalare */
  z-index: 2; /* Asigură-te că butoanele sunt deasupra overlay-ului */
}

.facebookBtn:hover,
.instagramBtn:hover,
.tiktokBtn:hover {
  transform: scale(1.1); /* Mărește butonul cu 10% la hover */
  color: white; 
}

.facebookBtn {
  background: #3B5998;
  border: none;
}

.instagramBtn {
  background: linear-gradient(45deg, #E1306C, #F77737);
  border: none;
}

.tiktokBtn {
  background: black;
  border: none;
}

@media (max-width: 768px) {
  .facebookBtn,
  .instagramBtn,
  .tiktokBtn {
    width: 50%; /* Asigură-te că butoanele au lățimea completă pe mobile */
    margin: 10px 0; /* Spatiu între butoane */
  }

  
}
</style>
