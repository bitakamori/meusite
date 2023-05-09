<script>
import face from "@/icons/face.png";
import git from "@/icons/git.png";
import i from "@/icons/i.svg";
import lkd from "@/icons/lkd.png";

export default {
  data() {
    return {
      face,
      git,
      i,
      lkd,
    };
  },
};
</script>

<template>
  <header>
    <div class="img-text">
      <img class="logo" src="@/assets/eu.jpeg" />

      <div class="text">Bem vindo!</div>
      <div class="social-medias">
        <a href="https://instagram.com/bitakamori" target="_blank">
          <img :src="i" alt="" />
        </a>

        <a href="https://www.facebook.com/bianca.takamori/" target="_blank">
          <img :src="face" alt="" />
        </a>

        <a href="https://www.linkedin.com/in/bianca-helena-takamori-ribeiro-9557a5191/" target="_blank">
          <img :src="lkd" alt="" />
        </a>

        <a href="https://github.com/bitakamori" target="_blank">
          <img :src="git" alt="" />
        </a>
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


.img-text a img{
  height: 25px;
  transition: 0.2s;
}

.img-text a img:hover{
  opacity: 0.7;
}


.text {
  margin: 1rem 0;
}

.img-text>img {
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

.social-medias>a {
  margin: 0 0.5rem;
}
</style>
