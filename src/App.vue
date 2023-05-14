<script>
import { RouterLink, RouterView } from "vue-router";
import map from '@/gif/map.gif'

export default {
  methods: {
    log() {
      document.getElementById('closed').classList.add('opacinout')

      setInterval(function () {
        document.getElementById('jura').classList.add('none')
        document.getElementById('closed').classList.add('none')

        document.getElementById('open').classList.remove('none')
        document.getElementById('open').classList.add('opacoutin')

        document.getElementById('banner').classList.remove('none')
        document.getElementById('banner').classList.add('opacoutin')


      }, 4000);

/*       document.getElementById('anim').classList.add('none')
 */    },
    hideAnimation() {
      document.getElementById('anim').classList.add('opacinout')
      setInterval(() => {
        document.getElementById('anim').classList.add('none')
      }, 2000)
    }
  }
}

</script>

<template>
  <header>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/works">Escolaridade</RouterLink>
      <RouterLink to="/tec">Hobbies</RouterLink>
      <RouterLink to="/about">About Me</RouterLink>
    </nav>
  </header>

  <RouterView />

  <div class="startAnimation" id="anim">

    <div class="mapClosed" id="closed">
      <img src="./gif/le.png" alt="">
      <img src="./gif/ld.png" alt="">
    </div>

    <div class="mapOpen none" id="open">
      <img src="./gif/opened.png" alt="">
    </div>

    <div @click="hideAnimation" class="mapOpen none" id="banner">
      <img class="banner" src="./gif/banner.png" alt="">
      <img class="bannerName" src="./gif/bannerName.png" alt="">
    </div>

    <!--     <lottie-player src="https://assets8.lottiefiles.com/packages/lf20_xp4orwk6.json" speed="0.5" autoplay loop>
                    </lottie-player> -->
    <button id="jura" @click="log()">
      <div class="text">Eu juro solenemente não fazer nada de bom.</div>
    </button>
  </div>
</template>

<style scoped>
.startAnimation {
  position: fixed;

  z-index: 1;

  height: 100vh;
  width: 100vw;
  top: 0;
  left: 0;

  /*   background-color: #111B4D;
 */
  background-color: #f8f1d6;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}


.startAnimation button {
  background-color: transparent;
  border: none;
  color: transparent;

  position: absolute;

  top: 75%;
  transition: 2s ease-out;

  margin: auto;

  font-family: 'Dancing Script', cursive;
  font-size: 2rem;
}

.startAnimation button:hover {
  color: #6B5D51;
}


.banner {
  height: 50px;
  position: absolute;

  top: 90%;
  left: 45%;

  transition: 1s ease-in-out;
}

.banner:hover {
  opacity: 0.7;
}

.bannerName {
  position: absolute;
  top: 220px;
  left: 30%;

  width: auto;
  height: 50px;

  animation: moveBannerNave 30s ease-in-out;
}

@keyframes moveBannerNave {
  from {
    top: 250px;
    left: 50%;
  }

  to {
    top: 220px;
    left: 30%;
  }
}

.none {
  display: none;
}

.text {
  font-size: 40px;
  font-weight: 600;
}

/* .startAnimation img {
  height: 100vh;
  width: 100vw;
} */



/* lottie-player {
  width: 50%;
} */


/* ANIMAÇÔES */


@keyframes frente {
  from {
    opacity: 1;
  }

  to {
    opacity: 0;
  }
}

@keyframes verso {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

.opacinout {
  animation: frente 4s forwards;
}

.opacoutin {
  animation: verso 4s forwards;
}



/* BASE CSS */

header {
  line-height: 1.5;

  padding-top: 40px;
  padding-bottom: 20px;
}


nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 0rem;
  font-weight: 200;

  /* border: 1px solid red; */
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
  font-weight: 400;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}
</style>
