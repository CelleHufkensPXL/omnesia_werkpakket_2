<script setup>
export default{
  data(){
    return{
      description: 'Welkom op de officiële webshop van Omnesia!'
    }
  }
}

import Navbar from './components/Navbar.vue';

export default {
  name: 'App',
  components: {
    Navbar, 
  },
};
</script>

<template>
  <body>
    <Navbar />

    <header class="header" >
        <div class="header__container">
            <div class="header__logo"><img src="assets/img/logo-lg-2.png" alt="Logo Omnesia"></div>
            <h1>{{ description }}</h1>
            <a href="producten.html"><h3 class="header__button">bekijk producten</h3></a>
        </div>
    </header>

    <div class="cite__container">
      <cite>
        <p>Purple People</p>
      </cite>
      
      <pre class="poem">
    <ins class="pilcrow">&#182;</ins>Ur so fucking perfect don't u think<ins>, </ins>  baby?<br>
    Looking down on others<span class="backspace">k at</span><ins class="red">, yeah</ins> <span class="comet">  to save yourself</span><ins>, </ins>  maybe
    But i know that you're insecure and afraid of being a failure
    <del class="desertion">The desertion of nurseries, the desertion of dead men</del>
    Dig a deeper grave<ins>,</ins> <ins class="the">to</ins><del class="of">so </del>put me down <ins>under.</ins>
      </pre>
    </div>

    <div class="about__container">
      <p class="about__tekst">Welkom op de officiële merchandise-webshop van Omnesia! Ontdek een wereld vol met  ontwerpen, geïnspireerd door de krachtige muziek en het unieke erfgoed van de ons. <br>
        Van t-shirts tot must-have verzamelitems, hier vind je alles om je liefde voor de Omnesia levendig te houden.</p>
    </div>

    <div class="image-container">
      <h1>Populaire Items</h1><br>
      <div class="image">
        <img src="assets/img/tshirt_1.png" alt="Tee Omnesia">
        <div class="overlay">
          <h1>Omnesia Tee</h1>
          <a href="details.html"><p>Bekijk</p></a>
        </div>
      </div>
      <div class="image">
        <img src="assets/img/totebag.png" alt="Totebag Omnesia">
        <div class="overlay">
          <h1>Omnesia Totebag</h1>
          <a href="producten.html"><p>Bekijk</p></a>
        </div>
      </div>
      <div class="image">
        <img src="assets/img/sticker1.png" alt="Sticker Omnesia">
        <div class="overlay">
          <h1>Omnesia Sticker</h1>
          <a href="producten.html"><p>Bekijk</p></a>
        </div>
      </div>
    </div>

    <footer>
      <div class="footer-content">
          <div class="footer-logo">
              <a href="#"><img src="assets/img/logo-lg-bw.png" alt="Omnesia Logo"></a>
          </div>
          <div class="social-media">
              <a href="https://www.facebook.com/profile.php?id=100078037556890"><img src="assets/img/fb.png" alt="Facebook"></a>
              <a href="https://www.instagram.com/omnesiaband/"><img src="assets/img/insta.png" alt="Instagram"></a>
              <a href="https://vi.be/platform/Omnesia"><img id="img__vibe" src="assets/img/vibe-logo-white.png" alt="Vibe Platform"></a>
          </div>
          <div class="footer-tekst">
            <p>&#169; Omnesia 2023 | omnesia.management@gmail.com</p>
          </div>
      </div>
  </footer>
</body>
</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  font-family: "Special Elite", "Inconsolata", "Courier New", mono;
  margin: 0;
  padding: 0;
  background-color: #E2E2E2;
}

/*HOME PAGINA*/
.nav {
  background-color: #1C1C1C;
  width: 100%;
  position: inherit;
}
.nav .navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 10px;
}
.nav .navbar .logo {
  margin-left: 30px;
}
.nav .navbar .logo img {
  width: 60px;
  height: auto;
}
.nav .navbar .logo img:hover {
  opacity: 0.8;
  transition: 0.2s;
}
.nav .navbar .nav-links {
  list-style: none;
  display: flex;
  align-items: center;
}
.nav .navbar .nav-links li {
  margin-right: 50px;
}
.nav .navbar .nav-links li:hover {
  transform: translateY(-20%);
  transition: transform 0.2s ease-in-out;
}
.nav .navbar .nav-links li a {
  text-decoration: none;
  font-size: large;
  color: #E2E2E2;
  background-color: #EF3030;
  padding: 8px;
  border-radius: 5px;
}
.nav .navbar .nav-links li a:hover {
  text-decoration: none;
}

/*HEADER*/
.header {
  background-image: url("../assets/img/Band b&w.jpg");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

.header__container {
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}
.header__container .header__logo {
  opacity: 0.8;
  width: 500px;
}
.header__container .header__logo:hover {
  opacity: 1;
  transition: 0.3s;
}
.header__container .header__title {
  color: #E2E2E2;
  font-variant: small-caps;
  align-self: center;
  vertical-align: center;
  font-style: italic;
  text-align: center;
  font-size: 3rem;
}
.header__container .header__button {
  color: #E2E2E2;
  align-self: center;
  vertical-align: center;
  text-align: center;
  background-color: #EF3030;
  padding: 10px;
  border-radius: 5px;
  margin-top: 50px;
}
.header__container .header__button:hover {
  transform: translateY(-20%);
  transition: transform 0.2s ease-in-out;
}

/*Poem section, bron: codepen.io*/
.cite__container {
  padding-left: 50px;
}

cite {
  display: flex;
  margin-bottom: 1rem;
  font-size: 14px;
  text-transform: uppercase;
  letter-spacing: 2.5px;
}

a {
  text-decoration: none;
  color: inherit;
}
a:hover {
  color: #EF3030;
}

.poem {
  position: relative;
  font-family: "Special Elite", "Inconsolata", "Courier New", mono;
  font-size: 1.75rem;
  line-height: 1.5;
  margin-top: 70px;
}

del {
  position: relative;
  text-decoration: none;
}
del:after {
  position: absolute;
  left: 0;
  width: 100%;
  height: 40px;
  content: "";
  background-image: url(data:image/svg+xml;base64,PHN2ZyBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2aWV3Qm94PSIwIDAgMzA1LjkgOCI+PHN0eWxlPi5zdDB7ZmlsbDojZGQyNjI2fTwvc3R5bGU+PHBhdGggY2xhc3M9InN0MCIgZD0iTTMwNS45IDQuN2MuMS0uMS4xLS4zLS4zLS4ybC0uMy4zLjYtLjF6TTMwMy4zIDQuMWMtLjQuMi0xIC40LS43LjcuNC0uMy41LS4yIDEtLjYuNCAwIC43LjEuNi4yLjEtLjEuNi4xLjgtLjEtLjUtLjMtMS4xLS4zLTEuOC0uMWwuMS0uMXpNMjY2LjYgMy41aC4yYzAgLjEtLjEgMC0uMiAwek0yNDMuOCAzLjRjLjIgMCAuMiAwIC4zLS4xLS4yIDAtLjMgMC0uMy4xek0yNDAgM2guMi0uMnpNMjY2LjYgMy41bC0uNi0uMWMtLjEuMS4zLjEuNi4xek0yOTguMyA0LjljLjEgMCAuMiAwIC4zLS4xLS4xIDAtLjIgMC0uMy4xIDAtLjEgMC0uMSAwIDB6TTI3Ni42IDMuM2guMmMuMSAwIC4xLS4xLjItLjFsLS40LjF6TTI4NC4zIDMuMmMtLjIgMC0uMi4zLS4zLjQuMS0uMS4yLS4yLjQtLjIgMCAwIDAtLjEtLjEtLjJ6TTI5Ni41IDMuN2gwek0yNzEuMSAzLjJzMC0uMS0uMS0uMWwuMS4xek01NS44IDUuM2MtLjEgMC0uMSAwIDAgMHpNNDYuOSAzLjloLjFjMC0uMS40LjUuNC41bC0uNS0uNXpNMjMxLjkgMy4zYy4yIDAgLjEgMCAwIDB6TTE2Ny45IDMuNWMuNy4zLTEuMi4zLS4xLjYtLjEtLjEgMS4xLS41LjEtLjZ6TTI5OC4xIDQuOGgtLjMuM3pNMTY3LjkgNC4xaC4xLS4xek0yMTUuNSAzLjVzLjEuMS4yLjFjMCAwIDAtLjEtLjItLjF6TTIyNy43IDMuOWgtLjMuM3pNMjA5LjIgMy45Yy0uMiAwLS4yLS4xLS40IDBoLjFzLjEtLjEuMyAwek0yMDMuOSAzLjhzLjEgMCAuMS4xaC4ybC0uMy0uMXpNNzUuOCA1LjJsLS4zLS4zYy4xLjItLjguMy4zLjN6TTI5OC4zIDQuN2MwIC4xLS4xLjEtLjIuMWguMnYtLjF6TTIwOS45IDUuNGgtMSAxek0xMjMuMSA1LjFoLS4yYy4xLjEuMi4xLjIgMHpNMjA1LjcgNS40Yy0uMi0uMS0uNC0uMi0uNi0uMiAwIDAtLjEgMC0uMS4xbC43LjF6TTc1LjUgNC45eiIvPjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik02OC42IDUuNmMxIDAgLjUtLjQuNy0uNiAxLjItLjEuNi4zIDEgLjUuNy0uMSAxLjMtLjUgMS44LS40IDAgLjEuMS4xIDAgLjIuOC0uMyAyLjMgMCAzLjMtLjQuMSAwIC4xLjEuMS4xLS4xLS4yLS4yLS40LS4xLS41LjQgMCAuOC0uMiAxIDAtLjMgMC0uMy4xLS40LjJsLjUtLjFjLjQuMy0uNi4xLS42LjQuOS0uMSAyLS40IDIuNy0uMy4xLjMtMS42LjEtLjcuNEw3Ni44IDVjLjguNS0uNyAwIC4xLjUgMS40LjEgMS42LS4yIDMtLjEuMi0uMy0uMi0uNC4xLS42IDItLjMgMS42LjkgMy4xLjQuNC0uMi41LS43IDEuNi0uNGwtLjQuNGMxLjQgMCAuOC0uNiAyLjItLjMtLjMuMi0xLjEuMS0uOS4yLjkuMy43LS4yIDEuNC0uMmwuMS4zYzEuNS0uMSAzLjEtLjMgNC43LS40LS4xLjEtLjQuMiAwIC4zIDIuMS0uMiA0LjQgMCA2LjQuMkw5OSA1Yy4yIDAgLjMuMS4xLjIuOC4xIDAtLjIuNC0uMy40IDAgLjYuMi4zLjMgMS40LS4yIDMuOS0uNSA1LjMtLjJsLS4xLjFjMS4xLjEgMS4zLS42IDIuMy0uM2wtLjIuMWMyLjQuMSA1LjEtLjEgNyAuMy40LS40IDIuNC4yIDIuNi0uNCAxLjQuMyAxIC40IDIuOS42LjUgMCAuOC0uNCAxLjQtLjR2LjNsLjktLjMuNS40LjYtLjFjLS4yIDAtLjUtLjEtLjUtLjIuOS0uMSAyLjMuMiAyLjMuNGwyLjItLjNjMCAuMS0uNC4yLS43LjIgMS4yLS4zLjIuMyAxLjMgMC0uMS0uMS4xLS4yLjEtLjIuNS4yIDEuOC4yIDIuNy4xbC0uMi4yYzEuNy4xIDMuNS0uMSA1LjQtLjEtLjctLjEtLjUtLjUgMC0uNWwuMi4zYy40LS4yLS42LS4xLjItLjQuNyAwIC41LjQuMS41bC44LS4xYzAgLjEtLjEuMS0uMi4zLjMtLjIgMS41LjMgMiAwdi4xYzEuOSAwIDIuNy0uMSA0LjItLjEgMC0uMy42LS4yIDEuMS0uNCAxLjEuMSAyLjMuMyAzLjcuMy45LS4xLjMtLjIuNy0uNC4xLjMgMS40LjIuNy40IDEuNiAwIDIuMS0uMSA0LjEtLjMtLjItLjEtLjUtLjItLjMtLjIuNCAwIC44LjEuOC4yaC0uMWMyLjMtLjQgNS4zLjcgNy4xLjJoLS4xbDEuOS0uM2MuOSAwLS41LjIuMS40IDItLjQgMy4yLjEgNC45LS4yIDEuMy44IDQuNi0uMSA2LjQuNGwtLjEtLjJjLjUtLjIuNS4xLjkuMSAwLS4xLS41LS4yLS4yLS4zIDMuOC0uMiA3LjkuMyAxMS44LjQgMS40IDAgLjgtLjkgMi42LS41bC0uNS4zYzIuOS0uNCA1LjkgMCA4LjgtLjMtLjIuMS0uMi4yLS41LjIuNi4yIDIuMiAwIDIuMi0uMi40IDAgLjEuMi40LjMuNi4xIDEuNS0uMyAxLjgtLjEuMSAwLS4yLjEtLjMuMS40LS4xIDEuOCAwIDEuNS0uMiAxLjEuMSAyLS4xIDIuOSAwIC42LS4zIDEuOC4xIDItLjMtLjEuNSAxLjkuNCAyLjUuMi0uMi4xLjYuMS4zLjMuOCAwIDEuNS0uMSAxLjMtLjMgMS40LjUgMi44LS40IDMuNi4zIDIuMy0uMiA0LjQtLjQgNi41LS41LS4xLjUtMi4zIDAtMi4yLjUgMS45LS4yIDMuMS0uNiA1LS41LjUuMS0uMy4yLS41LjMgMS45LS4yIDMuOCAwIDUuNS0uMiAwIDAtLjIuMS0uNC4xLjMgMCAuOC4xLjgtLjFoLS4zYy0uNS0uMyAxLjQtLjYgMS40LS44LS42LjYgMS43LjEuOC45LjIgMCAuNS0uMS41LS4zLjMgMCAuNC4xLjEuMyAxLjItLjEuOC0uMyAxLjktLjMgMCAuMS0uMi4xLS4zLjMuNi0uMiAxLjEtLjQgMi4xLS4zLS4xLjEuMS4xLS4yLjEgMS42IDAgMi43LS41IDQuNS0uMy0uNS40LjYuMS43LjVsLjktLjEtLjQtLjJjLjggMCAxLjYtLjMgMi4zLS4xbC0uNi4yIDEuNi0uMS0uOS0uMWMuOC0uMi0uMS0uNSAxLS40LS4yIDAgLjggMCAxLjMuMi40LS4xLjgtLjIgMS40LS4yLjIuMS0uMS40IDAgLjUuNC0uMyAxLjktLjEgMi41LS40LS4yLjEtLjIuMy0uMS4zbC4zLS4zYy40LjEuNC4xLjQuMyAxLjIgMC0uNC0uNSAxLS4zLS4xIDAtLjEuMS0uMy4xIDEuNC4xIDIuNy0uMiAzLjkgMCAuNC40LTEuMS4xLS43LjQgMS44LS4xIDMuOC0uNSA1LjYtLjRoLS4zYy4yLS41IDEuMy4zIDIuMiAwLS4yIDAtLjMuMy0uMi4yIDEuMi4xIDIuNS0uMSA0LjMtLjNsLS4yLjFjLjcuMSAxLjkuMSAyLjcuMS4yLS4xLjctLjEuNC0uMyAyLjQuOCA0LjUtLjQgNi43LjItLjMgMC0uNi4xLS40LjFsMS44LS4xYy0uMS0uMi0uMi0uMS0uNi0uMy4yLS4xLjctLjIgMS4yLS4yLS44LjIgMCAuNC40LjUtLjEtLjEuMS0uMSAwLS4yLjkuNC4yLS41IDEuNC0uMmwtLjEuMWMuNS0uMS45LS4yIDEuNC0uMi4yLjMtLjUuMS0uNS4zLjcgMCAxLjQtLjUgMi4xLS4yLS4zLjEtLjguMS0xLjEuMS43LjMuOC4yIDEuMy4zaC0uMWwxLjIuMS0uMy0uMWMuOS0uNyAxLjktLjEgMy4xLS42LTEuMi40LS4yLjItLjMuNi4zLjEuOC4yLjcuMy42LS4yIDEgLjIgMS44LS4yIDAgLjEuNiAwIC41LjMuOC0uMS0uMi0uMi0uMS0uMyAxLjItLjMgMi43LjQgNC40LS4xIDEuNC0uMiAxLjctLjUgMy0uNy41LjItLjQuNC0uNC40LjcuMSAxLjMuMSAyIDAtLjEuMSAwIC4yLjIuMy42IDAgLjQtLjQgMS4xLS4yLS4xLjEtLjMuMy0uNS40LjYtLjEgMS4zLS4zIDItLjQuMi4yLS40LjMtLjYuNC44LS4xIDItLjIgMi4yLS40bC0uNS0uMWMuMyAwIC4xLjItLjEuMy0uNi4yLS45LS4xLTEtLjJsLjUtLjFjLS41LS42LTEuOS4xLTIuOS4xbC40LS40LTEgLjNjLS4yLS4xLS40LS4zLjEtLjQtLjctLjItLjYuMS0xLjItLjEtLjEgMCAwLS4xIDAtLjFsLS43LjFjLjEtLjEtLjEtLjMuMy0uMi0xLjItLjItMiAuMy0yLjQgMGguMWMtMS43LjEtLjIuMy0xLjQuN2wtLjgtLjgtLjIuM2MtLjIgMC0uNSAwLS41LS4yLS42LjIuMS4xLS4zLjMtLjgtLjMtMi4zLjEtMi41LS40LS4zLjIuOC4yLS4xLjMtLjMtLjUtMSAuMS0xLjgtLjIuMi0uMyAxLS4xLjItLjQtLjUuNS0xLjUtLjEtMi4xIDAgMCAuNC0xLjQuMi0yLjUuMy4xLS4xLTItLjItMy0uM1YzYy0uMi40LTEuMi4zLTIgLjQgMC0uMi4yLS4zLjYtLjRoLS43Yy0uMi4xLS40LjItLjguMmwuMi0uM2MtLjkgMC0xLjkuMy0zLjEuMS0uMS4zIDEgLjctLjMuOSAwLS4xLS4xLS40LjItLjQtLjEgMC0uNC4xLS42LjFsLjUtLjJjLS42LS4xLS4zLjItLjcuMiAwLS4yLS4zLS4xLS4zLS4zLjEgMCAuNC4xLjYgMC0uNSAwLTEuMS0uMi0xLjMtLjMgMCAuMSAwIC4zLS40LjMtLjkgMC0uMy0uMi0uOS0uMy0uMi4xLS44IDAtLjguMy0uMyAwLS4zLS4xLS40LS4yLS41LjEtMi4zIDAtMS43LjRoMGMtMS42LjMtMy4zLS4yLTQuOSAwdi0uMWMtLjkuMS0yLjEuMS0yLjguMy0uMyAwLS43LS4yLS41LS4zLS43LjEtLjguMi0xLjkgMCAuNy0uMi0uMy0uMi43LS4xLS45LS4xLTEuMi0uMi0yLjIgMCAuMy0uMy0uNy0uMy0xLjItLjJsLjcuMmgtMS40bC4yLS4zYy0xLjktLjQtMy41LjctNC45IDAtLjUuMiAxIC4yLjYuNC0uOSAwLTEuOC0uNS0yLjEtLjUtMS4yLS4yLTEuMS41LTIuNC40LjIuMS4zLjQtLjYuNS0uOSAwLTEuMS0uNS0uNS0uNi4yIDAgLjMgMCAuMy4xLjMgMCAuNy0uMS4zLS4ybC0uMS4xYy0uNC0uMS0xLjctLjEtMS40LS4zLS43LjEtLjMuMi4yLjMtMS4xLS4yLTEuOCAwLTIuOS0uMS4yLjEuNC4yLjIuMi0xLjctLjEtMS43LjktMi44IDEtLjctLjIuMi0uNC0uOS0uMy0uNy0uMS0uMi0uMy4xLS40LTEuMS4yLTItLjItMi42LS4ybC42LS4xYy0uMy4xLS42LjEtLjkuMWwuMy4yYy0uMyAwLS42IDAtLjYtLjEtLjMuMi4zLjQtLjQuNi0uNC0uMS0xLjMuMS0xLjUtLjIgMS40LjEtLjItLjMgMS0uNGgtLjhzMC0uMS4xLS4xYy0xLjMtLjMtLjYuNC0yIC4zLjItLjItLjMtLjMtLjUtLjMuNiAwIC4zLjMtLjIuNC0uOS0uMS0xIC4xLTEuNC4xbC41LjFjLS4yLjItLjYuMi0xLjIuMi0uMy0uMi4zLS4xLjEtLjItLjcuMy0xLjUtLjMtMi41LS4xLS40LS4xIDAtLjMtLjQtLjQtMS4xLjItMS4yLS4yLTIuMy0uMS4zLjIuNC4yLS40LjRsMS44LS4yLTEuMi40Yy42IDAgMS4yLS4xIDEuNS0uMS0uNi4yLS41LjEtLjIuMy0uOC0uNC0xLjUuMi0yLjQgMHYtLjZjLTEuMy0uMy0yLjMuMy00LjEuMmwuNi4xYy0uMi4yLTEuMSAwLTEuNi4xLjEtLjItLjMtLjMtLjUtLjQgMCAuMS0xLjMgMC0xLjQuNGwtLjgtLjNjLTEuNC0uMS0xLjYuNi0yLjkuNS40LS4yLS4yLS40LjctLjUtLjQgMC0uOCAwLS44LjEtLjMtLjEtMS4yLjMtMS42LjEtLjIuMS0uMi4zLS43LjMtLjEgMCAwLS4xIDAtLjEgMCAuMS0uOC4xLS4zLjQtMS40LS42LTIuNSAwLTMuNy0uNS0xIC4xLTIuMS4xLTMgLjEuMS0uMSAwLS4xLjItLjEtMS4yLS4yLS43LjYtMi4xLjQtLjctLjMuNy0uMi4zLS4zLS4yLS42LTEuNy4xLTIuNi0uM2guMmMtLjctLjItMS43LjItMi45LjIgMCAwIC4xLS4xIDAtLjEtLjguMy0yLjMuNC0zLjQuNS4zLS4zLjUtLjEuMy0uNC0uNSAwIC4xLjQtLjkuNS0uMy0uMS0xLS4zLTEuMS0uNWguOWMtLjUtLjQtMS4yIDAtMS43IDBsLjEtLjJjLTEuNC4xLTEuNS40LTMgLjRsLjIuMWMtLjguNC0uNy0uMi0xLjYuMWwtLjMtLjRjLS42LjEtMiAuNC0zIC41LjYtLjMgMS43LS40IDIuNS0uNi0uNiAwLTEuOSAwLTIuMi4yLjIgMCAuNS0uMS43LS4xLS43LjMtMS42LjUtMi43LjUuMi0uOC0yLjktLjItMy43LS44LTIgLjMtMy45LS4xLTYuMi0uMS44LjYtLjcgMC0uNS42aC0uOGwtMS42LS40Yy0uNC0uMi41LS4xLjUtLjMtMS4yIDAtLjUtLjMtMS4zLS40LjIuMi0uNC4zLTEuMS4ybC45LjNjLTEuNi4zLTEuNC0uNS0zLS4ybC41LS4yYy0uOC4xLTMuMSAwLTMuOS41LS4xLS4xLS4zLS4yIDAtLjMtMi0uMS00LjUuNS02IC4ybC4yLS4xYy0uNCAwLS43LjMtMS4xLjEgMC0uMS4yLS4xIDAtLjItLjIuMS0xIC4zLTEuNS4ybC40LS4yYy0yLS4yLTMgLjQtNC42LjUgMC0uNC0xLjUtLjYtMi4zLS43di0uMWMtMi4zLS4xLTMuOS40LTYgLjUtMS4zLS41LTQuNC0uMi02LjUtLjUuMy4xLS4xLjMtLjQuNC0uNS0uMS0xLjQuMy0xLjMtLjFoLjJjLS40LS40LTEuNC0uMy0yLjItLjNsLS4xLjVjLTIuMS0uOC01LjQuMy02LjYtLjQtLjUuMS0xLjEuMS0xLjYuM3YtLjNjLTEuNC0uMS0yLjEtLjEtMy44IDBsLjMtLjJjLTEgMC0xLjIuOC0yLjEuOGwtLjMtLjRjLTEuNyAwLTMuNC0uNC01LjEgMCAwLS4xLjEtLjIuMy0uMi0uOCAwLTMuMS0uMy0yLjguMyAwLS40LTEuNyAwLTIuNi4xbC4xLS4zYy0uOC40LS44LjUtMS45LjYtLjMgMC0uMi0uMi4xLS4yLS44LS4xLS43LjMtMS43LjFsLjQtLjJjLS45IDAtLjguMS0xLjMuMy0uNS4xLTEuNy0uMS0xLjgtLjMtLjEuMi0uNi40LTEuMS4zLS4xLS4xLjEtLjIuMi0uMi0xLjUtLjItMi4yLjMtMy4yLjEgMC0uMS0uMS0uMS0uMi0uMmgyYzAtLjMtLjktLjMtLjItLjctLjguMi0yIC42LTIuOS41IDAgMC0uMSAwLS4xLS4xaC4xLS42Yy0uMyAwLS41LS4xLS44LS4xLS4xLS4yLTEuMS0uMS0xLjUtLjEgMCAuMy0uNi4yIDAgLjVoMS44Yy0uNC4xLS44LjMtMS4zLjEtLjIuMi0uNS40LS43LjUtLjYtLjQtMS45LS42LTItLjgtMS40LjItMy40LjEtNC4zLjYtLjQuMS0uNS0uMi0uNi0uMi4yLS4xLjUgMCAuNi0uMS0uOC4xLTIuNC4xLTIuNi40LTEtLjIuNi0uMy0uOC0uM2wuMi0uMWMtMi42LS41LTQuMyAxLTcuNC4zLjIgMCAuMy4xLjQuMS0zLjUtLjMtNy4yLjMtMTAuNi0uMi0xLS4xLTEuMS4xLTEuNy4zbC0uMi0uMy0xIC4zYy0xLjQuMy0yLjUtLjctNC4zLS4zbC4yLjJjLS43IDAtMi4xLjEtMi0uMS0uMSAwLS4yLjItLjUuMXYtLjJsLTEuNi4zYy0xLjMtLjEuMi0uNi0xLjYtLjctLjcuMS0xLjkuNS0xLjcuNi4zIDAgLjcuMS43LjNsLTEtLjZjLS4xLjUtLjYuOS45IDEuM2wxLjEtLjIuMy4yaC0uOWMuNS4yLjggMCAxLjItLjEuMS4xLjIuMi40LjJsMS0uNGMuMS4yLS41LjQuMi41LjUtLjItLjUtLjQuMy0uNS43LjIuNS4zIDEuMS4yLjEuMSAwIC4yLS4zLjIuNS0uMSAxLjQtLjEgMS43LS4zLjUuMyAxLjgtLjEgMS43LjQuMi0uMS45LS4zIDEuNC0uNC0uOS41IDEuOCAwIDEuNi42LjgtLjUgMi41LS4yIDMuNi0uNS0uMSAwLS4yLjEtLjMuMS43IDAgLjguMiAxLjMuMy4xLS40IDEuMS0uNSAxLjctLjcuOC40LS41LjUtLjIuOCAwLS4zIDEuNC0uMyAxLjEtLjYuNi4yLjUuMS44LjQuMS0uNS42LS4xIDEuMS0uNC45LjMuMi41IDEuMi40LjUuMS0uNC4zLS40LjN6bTIzLjMtLjljMCAuMSAwIC4xIDAgMGgtLjVjLjIuMS4zLjEuNSAwem0yIDBIOTNjLS4xLS4xIDAtLjIuMi0uMi0uMS4xLjQuMi43LjJ6bS0zLjgtMS4zYy4zIDAgLjQgMCAuNS4xaC0uNWMtLjEgMCAwIDAgMC0uMXoiLz48cGF0aCBjbGFzcz0ic3QwIiBkPSJNODkuNiAzLjhoLS4xYzAgLjEuMS4xLjEgMCAuMS4xLjEgMCAuMiAwaC0uMnpNMjY2LjkgMy42ek0xMjEgNS4zdi0uMWwtLjIuMXpNMjc3LjcgNC41bC4xLjFzLS4xIDAtLjEtLjF6TTI4Mi4zIDQuNmwuNy4xYy0uMyAwLS41LS4xLS43LS4xek0yODUuOSA0LjdsLjEtLjEtLjEuMXpNMjI4LjkgNS4xaDB6TTI0NS45IDQuNGMtLjIuMS0uNC4xLS41LjEuMi4xLjUuMS41LS4xek0yMTAgNS40aC0uMS4xek0yNDQuNSA0LjZjLjMuMS42IDAgLjggMC0uMi0uMS0uNS0uMS0uOCAwek0zMDEuNSA0LjloLjItLjJ6TTMwMS43IDQuOGguMi0uMnpNMzAyLjIgNC43bC0uNC4xYy4yIDAgLjQgMCAuNC0uMXpNMjk2LjcgNC43bC0uMS4xYy4xIDAgLjEgMCAuMS0uMXpNMjk1LjMgNC44Yy4zIDAgLjkuMiAxLjMuMnYtLjFjLS4yLjEtMS0uMy0xLjMtLjF6TTI4OS4yIDMuNWwxLjIuMWMtLjItLjEtLjUtLjMuMS0uMy0xLjUtLjMuMy4zLTEuMy4yek0yODUuNSAzLjRjLjYtLjEgMC0uMiAwLS4yLS40IDAtLjUuMSAwIC4yek0yNTguNCAzLjRsLjEtLjNjLS41IDAgMCAuMS0uMS4zek0yNTMuMiA0LjdsLjUuMS4zLS4yek0yNTAuMiAyLjlsLjItLjEtLjguMXpNMjA1LjEgMy42bC4yLjNjLjMtLjEuMy0uNC0uMi0uM3pNMTg1LjQgMy45Yy0uMi0uMi0uOC0uMy0xLjEtLjEuNSAwIC45LjIgMS4xLjF6TTEyNi42IDMuNGwuMy0uMS0uNy4xeiIvPjxnPjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik0xOS44IDQuM2MwIC4xIDAgLjMtLjEuNWwuMS0uMWMuOS40IDIuNS4xIDMuMy40LS4xLS4xIDAtLjEgMC0uMi42IDAgMS4xLjMgMS45LjQuNC0uMi0uMi0uNiAxLS41LjIuMi0uMy42LjcuNiAwIDAtLjktLjItLjQtLjMgMSAuMS4zLS4xIDEuMi0uMy41LjMgMS0uMSAxLjEuNC4zLS4zLjItLjIuOC0uNC0uMy4yIDEuMS4yIDEuMS42LjMtLjQtMS0uNC0uMi0uOC42LjIgMS42LjMgMS43LjcuMy0uMS41LS4zIDEuMi0uMy0uMSAwLS4yLS4xLS4zLS4xIDEuMi4zIDIuOSAwIDMuNi41LS4yLS42IDIuNS0uMSAxLjYtLjYuNSAwIDEuMy4zIDEuNC40LS4xLS40IDEuMi0uMSAxLjctLjQuMy4yIDEuMS4yIDEuNy4zLS4yLS4xLS40LS4xLS4zLS4yLjYuMi40IDAgMS0uMi44LjEtLjEuMy4zLjUuNy0uMS4xLS4zLjItLjVsMSAuNGMuMiAwIC40LS4xLjQtLjIuNS4xLjguMyAxLjMuMWgtLjlsLjMtLjIgMS4xLjJjMS41LS4zIDEuNC0uMiAxLjMtLjZsLS42LS4xYzAtLjIuNC0uMi43LS4zLjMgMC0xLS40LTEuNy0uNS0xLjggMC0uOC0uMS0yIDBsLTEuNi0uM3YuMmMtLjMuMS0yLjguMy0yLjguMy4xLjItMS4zLjEtMiAuMWwuMi0uMmMtMS44LS41LTIuNC43LTMuOC40bC0xLS4zLS4yLjNjLS42LS4yLS43LS40LTEuNy0uMy0zLjQuNS01LjcgMC01LjUgMGwtMy4yLjUtMS4yLS4yLTEuMi40LS44LS40LS40LjMiLz48cGF0aCBjbGFzcz0ic3QwIiBkPSJNMTkuMyAzLjdjLTEuMS0uMS0yLjQuMS0yLjUtLjMtLjYtLjEtMS43LjUtMi4xIDAtLjguMiAwIC4xLjIuNC0uOC4yLTEuNS0uNC0xLjguMi0uOS0uMi4yLS4xLS4xLS4zLS4yLjUtMS43LjEtMi41LjQtLjQtLjIuNC0uMS0uMy0uMy4xLjEtLjMuMS0uNS4ybC0uMS0uNS0uOC43Yy0xLjMtLjMuMi0uNS0xLjQtLjZoLjFjLS41LjMtMS4yLS4yLTIuNCAwIC40LS4xLjIuMS4zLjJsLS43LS4xYy4xIDAgLjEgMCAwIC4xLS42LjItLjUtLjEtMS4yLjEuNSAwIC4zLjMuMS40bC0xLS4zLjQuM2MtMSAwLTEuNS0uNy0yLS4xbC0uNC4xYzAgLjEuNi40LS4xLjItLjIgMC0uMy0uMy0uMS0uM2wtLjQuMWMuMi4zLjUuNCAxLjMuNS0uMi0uMS0uOC0uMi0uNi0uNC43LjEgMS4zLjMgMiAuNC0uMy0uMS0uNS0uMy0uNi0uNC43LS4xLjUuMiAxLjEuMi4yLS4xLjQtLjIuMi0uMy43LjEgMS4yLjEgMiAwIDAgMC0uOC0uMi0uNC0uNCAxLjMuMiAxLjYuNSAzIC43IDEuNy41IDMuMi0uMyA0LjQuMS4xLjEtLjkuMi0uMS4zLS4xLS4yLjUtLjIuNS0uMy44LjQgMS4yLS4xIDEuOC4yLS4xLS4xLjMtLjIuNy0uMy0uMS0uMy45LS4xLS4zLS42IDEuMi41IDIuMSAwIDMgLjdsLS4zLjEgMS4yLS4xaC0uMWMuNSAwIC42IDAgMS4zLS4zLS4zLS4xLS44LS4xLTEuMS0uMSIvPjwvZz48L3N2Zz4=);
  background-repeat: repeat-x;
  background-position: center center;
  background-size: 100% 100%;
}

.backspace {
  position: absolute;
  opacity: 0.15;
}

ins {
  position: absolute;
  margin-left: 2px;
  color: #EF3030;
  font-family: "Homemade Apple", cursive;
  text-decoration: none;
  transform: rotate(-4deg);
}
ins.the {
  margin-top: 27px;
}

.pilcrow {
  margin-left: -24px;
}

.red {
  margin-left: -3px;
  letter-spacing: -3px;
}

del.of:after {
  background-size: 1200% auto;
}

.comet {
  margin-left: 54px;
}

.cite__container {
  display: flex;
  align-items: center;
  margin: 0 auto;
  height: 45vh;
  background-color: #E2E2E2;
}

/*ABOUT SECTION*/
.about__container {
  width: 100%;
  height: 45vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #1C1C1C;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  opacity: 1;
}
.about__container .about__tekst {
  display: flex;
  width: 30vw;
  line-height: 2.5rem;
}
.about__container p {
  color: #E2E2E2;
  font-size: 1.5rem;
}

/*TRENDING PRODUCTS*/
.image-container {
  display: flex;
  width: 100%;
  height: 60vh;
  justify-content: space-evenly;
  align-items: center;
  background-color: #E2E2E2;
}

.image {
  position: relative;
  margin: 10px;
}

img {
  max-width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 400px;
  height: 400px;
  background: rgba(239, 48, 48, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.overlay h1 {
  color: #E2E2E2;
  font-size: 25px;
  text-align: center;
  transform: translateY(-100%);
  transition: transform 0.3s ease-in-out;
}

.overlay p {
  color: #E2E2E2;
  font-size: 20px;
  text-align: center;
  transform: translateY(-100%);
  transition: transform 0.3s ease-in-out;
}

.image:hover .overlay {
  opacity: 1;
}

.image:hover .overlay p {
  transform: translateY(0);
}

/*FOOTER*/
footer {
  background-color: #EF3030;
  color: #E2E2E2;
  height: 31vh;
  width: 100%;
}
footer .footer-content {
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  width: 100%;
}
footer .footer-content .footer-logo a img {
  width: 500px;
}
footer .footer-content .social-media {
  display: flex;
  align-items: center;
  justify-content: center;
}
footer .footer-content .social-media a {
  margin: 0 10px;
}
footer .footer-content .social-media a img {
  width: 30px;
  height: 30px;
  opacity: 0.7;
  transition: opacity 0.3s;
}
footer .footer-content .social-media a img:hover {
  opacity: 1;
}
footer .footer-content .social-media a #img__vibe {
  width: 70px;
  height: 20px;
  opacity: 0.7;
  transition: opacity 0.3s;
  align-items: center;
}
footer .footer-content .social-media a #img__vibe:hover {
  opacity: 1;
}

/*PRODUCTEN PAGINA*/
.title_container {
  background-color: #EF3030;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
}
.title_container h1 {
  color: #1C1C1C;
}

.introduction_container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #E2E2E2;
  padding: 10px;
  padding-left: 50px;
}
.introduction_container .introduction_tekst {
  flex: 1;
}
.introduction_container .filter-options {
  display: flex;
  flex-direction: row;
  gap: 10px;
}
.introduction_container .filter-options label {
  color: #E2E2E2;
  background-color: #EF3030;
  padding: 8px;
  border-radius: 5px;
}
.introduction_container .filter-options #filter1, .introduction_container .filter-options #filter2 {
  background-color: transparent;
  border-radius: 5px;
}

.product_info {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

/*DETAILPAGINA*/
.back_button {
  display: flex;
  margin: 20px;
}

.product-detail {
  display: flex;
  margin: 0 auto;
  margin-top: 100px;
  background-color: #E2E2E2;
  border-radius: 5px;
  padding: 20px;
  width: 1000px;
}

.product-image {
  width: 50%;
}
.product-image img {
  width: 500px;
  height: auto;
}

.product-info {
  width: 50%;
  margin-left: 50px;
}
.product-info h1 {
  font-size: 4rem;
  margin: 0 0 10px;
}
.product-info p {
  font-size: 16px;
}
.product-info .size-quantity {
  display: flex;
  flex-direction: row;
}
.product-info .size-quantity .size-options, .product-info .size-quantity .quantity-options {
  width: 30%;
  margin-top: 20px;
  padding-right: 30px;
}
.product-info .size-quantity .size-options label, .product-info .size-quantity .quantity-options label {
  color: #E2E2E2;
  background-color: #EF3030;
  padding: 8px;
  border-radius: 5px;
}
.product-info .size-quantity .size-options #size, .product-info .size-quantity .quantity-options #size {
  margin-top: 40px;
  background-color: transparent;
  border-radius: 5px;
}
.product-info .size-quantity .size-options #quantity, .product-info .size-quantity .quantity-options #quantity {
  margin-top: 40px;
  background-color: transparent;
  border-radius: 5px;
  width: 50px;
}
.product-info .size-quantity select, .product-info .size-quantity input {
  width: 100%;
  height: 50px;
  font-size: 16px;
}
.product-info .add-to-cart {
  color: #E2E2E2;
  background-color: #EF3030;
  padding: 8px;
  border-radius: 5px;
  font-family: "Special Elite";
  font-size: 1rem;
  cursor: pointer;
}

/*LOGIN PAGINA*/
.login-container {
  display: flex;
  margin: 0 auto;
  margin-top: 150px;
  flex-direction: column;
  background-color: #EF3030;
  border: 1px solid #ccc;
  padding: 40px;
  width: 300px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}
.login-container h2 {
  font-size: 1.5rem;
  margin: 0 0 20px;
}
.login-container .input-container {
  margin: 10px 0;
}
.login-container .input-container label {
  display: block;
  font-weight: bold;
  color: #1C1C1C;
}
.login-container .input-container input {
  width: 100%;
  height: 40px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
  margin-top: 10px;
}
.login-container button {
  width: 100%;
  height: 40px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 3px;
  background-color: #E2E2E2;
  color: #EF3030;
  font-size: large;
  border: none;
  margin-top: 10px;
  cursor: pointer;
  font-family: "Special Elite";
}
.login-container #login-button:hover {
  transform: translateY(-10%);
  transition: transform 0.2s ease-in-out;
}
.login-container #forgot-password {
  color: #E2E2E2;
  font-size: medium;
}
.login-container #forgot-password {
  background-color: transparent;
  border: none;
  text-decoration: underline;
  font-size: small;
}

/* Mediaquery voor kleinere schermen */
@media screen and (max-width: 768px) {
  .nav {
    padding: 10px;
  }
  .nav .navbar {
    flex-direction: column;
    align-items: center;
  }
  .nav .navbar .logo {
    margin: 10px 0;
  }
  .nav .navbar .logo img {
    width: 40px;
  }
  .nav .navbar .nav-links {
    flex-direction: column;
    text-align: center;
    margin-top: 10px;
  }
  .nav .navbar .nav-links li {
    margin: 10px 0;
  }
  /*HEADER*/
  .header {
    background-image: url("../assets/img/Band b&w.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
  .header__container {
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
  }
  .header__container .header__logo {
    opacity: 0.8;
    width: 500px;
  }
  .header__container .header__logo:hover {
    opacity: 1;
    transition: 0.3s;
  }
  .header__container .header__title {
    color: #E2E2E2;
    font-variant: small-caps;
    align-self: center;
    vertical-align: center;
    font-style: italic;
    text-align: center;
    font-size: 3rem;
  }
  .header__container .header__button {
    color: #E2E2E2;
    align-self: center;
    vertical-align: center;
    text-align: center;
    background-color: #EF3030;
    padding: 10px;
    border-radius: 5px;
    margin-top: 50px;
  }
  .header__container .header__button:hover {
    transform: translateY(-20%);
    transition: transform 0.2s ease-in-out;
  }
  .cite__container {
    display: none;
  }
  /*About section*/
  .about__container {
    width: 100%;
    height: 45vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color: #1C1C1C;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    opacity: 1;
  }
  .about__container .about__tekst {
    display: flex;
    width: 35vw;
    line-height: 1.2rem;
  }
  .about__container p {
    color: #E2E2E2;
    font-size: 1.2rem;
  }
  /*trending products*/
  .image-container {
    display: flex;
    width: 100%;
    height: 60vh;
    justify-content: space-evenly;
    flex-direction: row;
    align-items: center;
    background-color: #E2E2E2;
  }
  .image {
    position: relative;
    margin: 10px;
  }
  img {
    max-width: 150px;
    height: auto;
  }
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 150px;
    height: 150px;
    background: rgba(239, 48, 48, 0.5);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.3s ease-in-out;
  }
  .overlay .overlay h1 {
    color: #E2E2E2;
    font-size: 15px;
    text-align: center;
    transform: translateY(-100%);
    transition: transform 0.3s ease-in-out;
  }
  .overlay .overlay p {
    color: #E2E2E2;
    font-size: 10px;
    text-align: center;
    transform: translateY(-100%);
    transition: transform 0.3s ease-in-out;
  }
  .overlay .image:hover .overlay {
    opacity: 1;
  }
  .overlay .image:hover .overlay p {
    transform: translateY(0);
  }
  /*FOOTER*/
  footer {
    background-color: #EF3030;
    color: #E2E2E2;
    height: 20vh;
    width: 100%;
  }
  footer .footer-content {
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
    width: 100%;
  }
  footer .footer-content .footer-logo a img {
    width: 500px;
  }
  footer .footer-content .social-media {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  footer .footer-content .social-media a {
    margin: 0 10px;
  }
  footer .footer-content .social-media a img {
    width: 30px;
    height: 30px;
    opacity: 0.7;
    transition: opacity 0.3s;
  }
  footer .footer-content .social-media a img:hover {
    opacity: 1;
  }
  footer .footer-content .social-media a #img__vibe {
    width: 70px;
    height: 20px;
    opacity: 0.7;
    transition: opacity 0.3s;
    align-items: center;
  }
  footer .footer-content .social-media a #img__vibe:hover {
    opacity: 1;
  }
  .introduction_container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #E2E2E2;
    padding: 10px;
    padding-left: 50px;
  }
  .introduction_container .introduction_tekst {
    flex: 1;
  }
  .introduction_container .filter-options {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .introduction_container .filter-options label {
    text-decoration: none;
    color: #E2E2E2;
    background-color: #EF3030;
    padding: 8px;
    border-radius: 5px;
  }
  .product_info {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}

/*# sourceMappingURL=style.css.map */

</style>
