<script></script>

<template>
  <header>
    <div class="img-text">
      <img class="logo" src="@/assets/eu.jpeg" />

      <div class="text">Bem vindo!</div>
      <div class="social-medias">
        <a href="https://instagram.com/bitakamori" target="_blank">
          Instagram
        </a>
        <a href="https://www.facebook.com/bianca.takamori/" target="_blank"
          >Facebok</a
        >
        <a
          href="https://www.linkedin.com/in/bianca-helena-takamori-ribeiro-9557a5191/"
          target="_blank"
          >Linkedin</a
        >
        <a href="https://github.com/bitakamori" target="_blank">Github</a>
      </div>
    </div>
  </header>
</template>

<style scoped>
.img-text {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 300px;
  height: 300px;
  padding-top: 15px;
  /* margin: 0 2rem; */
}

.text {
  margin: 1rem 0;
}

.img-text > img {
  width: 75%;
  border-radius: 50%;
  display: flex;
}

.social-medias {
  display: flex;
  margin: 0.5rem auto;
  height: 200px;
  justify-content: space-around;
  width: 50%;
}

.social-medias > a {
  margin: 0 0.5rem;
}
</style>
