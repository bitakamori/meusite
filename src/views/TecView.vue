<script>
/* IMPORT LIVROS */
import hp from "@/assets/fotos/hp.png";
import js from "@/assets/fotos/js.png";
import oimp from "@/assets/fotos/oimp.png";
import ver from "@/assets/fotos/ver.png";

/* IMPORT FILMES */
import spn from "@/assets/fotos/spn.png";
import herd from "@/assets/fotos/herd.png";
import mv from "@/assets/fotos/mv.png";
import hpm from "@/assets/fotos/hpm.png";

/* IMPORT AMI */
import rp from "@/assets/fotos/rp.png";
import uni from "@/assets/fotos/uni.png";
import vd from "@/assets/fotos/vd.png";
import rs from "@/assets/fotos/rs.png";

export default {
  data() {
    return {
      indexLivros: 0,
      indexFilmes: 0,
      indexAmi: 0,

      livros: [
        { phat: hp, title: "Harry Potter" },
        { phat: js, title: "jantar Secreto" },
        { phat: oimp, title: "O impulso" },
        { phat: ver, title: "Verity" },
      ],

      filmes: [
        { phat: spn, title: "Supernatural" },
        { phat: herd, title: "hereditário" },
        { phat: mv, title: "Marvel" },
        { phat: hpm, title: "Harry Potter" },
      ],

      ami: [
        { phat: rp, title: "" },
        { phat: uni, title: "" },
        { phat: vd, title: "" },
        { phat: rs, title: "" },
      ],
    };
  },
  methods: {
    indexLivrosMais() {
      this.indexLivros == 3 ? (this.indexLivros = 0) : this.indexLivros++;
    },
    indexLivrosMenos() {
      this.indexLivros == 0 ? (this.indexLivros = 3) : this.indexLivros--;
    },
    indexFilmesMais() {
      this.indexFilmes == 3 ? (this.indexFilmes = 0) : this.indexFilmes++;
    },
    indexFilmesMenos() {
      this.indexFilmes == 0 ? (this.indexFilmes = 3) : this.indexFilmes--;
    },
    indexAmiMais() {
      this.indexAmi == 3 ? (this.indexAmi = 0) : this.indexAmi++;
    },
    indexAmiMenos() {
      this.indexAmi == 0 ? (this.indexAmi = 3) : this.indexAmi--;
    },
  },
};
</script>

<template>
  <div class="complexo">
    <!-- LIVROS FAVORITOS -->

    <div class="box1">
      <div class="text0">Livros favoritos</div>

      <div class="container-img">
        <div class="arrow" @click="indexLivrosMenos">&lt</div>
        <div class="container-livro">
          <img :src="livros[indexLivros].phat" alt="" />
          <br />
          {{ livros[indexLivros].title }}
        </div>
        <div class="arrow" @click="indexLivrosMais">></div>

        <div class="content">
          Sou apaixonada pela leitura, adoro o poder de imersão que um livro proporciona.
          Meus gerenros preferidos são suspense, serial killer, fantasia, ficção
          científica e livros de psicologia e autoajuda.
        </div>
      </div>
    </div>

    <!-- FILMES FAVORITOS -->

    <div class="box1">
      <div class="text0">Filmes favoritos</div>

      <div class="container-img">
        <div class="content content_direita">
          Adoro ver filmes e séries, e harry potter é meu confort film com gostinho de
          infancia. Meus generos preferidos são terror/suspense ficção científica e
          fantasia, pincipalmente com bons plot twist. E adoro séries de confeitaria e
          competições em geral.
        </div>

        <div class="arrow" @click="indexFilmesMenos">&lt</div>
        <div class="container-livro">
          <img :src="filmes[indexFilmes].phat" alt="" />
          <br />
          {{ filmes[indexFilmes].title }}
        </div>
        <div class="arrow" @click="indexFilmesMais">></div>
      </div>
    </div>

    <!-- Amigurumis -->

    <div class="box1">
      <div class="text0">Alguns amigurumis</div>

      <div class="container-img">
        <div class="arrow" @click="indexAmiMenos">&lt</div>
        <div class="container-livro">
          <img :src="ami[indexAmi].phat" alt="" />
          <br />
          {{ ami[indexAmi].title }}
        </div>
        <div class="arrow" @click="indexAmiMais">></div>

        <div class="content">
          Amo fazer croche, principalmente amigurumis. É uma otima terapia.
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
div.complexo {
  display: flex;
  flex-direction: column;
  height: auto;
  width: auto;

  justify-content: space-around;
  align-items: space-around;
}

div.complexo main {
  height: auto;
  display: flex;
  flex-direction: column;
}

/* LIVROS FAVORITOS */

.box1 {
  display: flex;
  justify-content: space-between;
  height: 400px;
  margin-top: 1rem;

  flex-direction: column;

  align-items: center;
}

div.container-img {
  height: 90%;
  width: 70%;

  display: flex;
  align-items: center;
  text-align: center;
  justify-content: space-evenly;

  flex-direction: row;
}

div.container-livro > img {
  height: auto;
  width: 200px;

  border-radius: 20px;
}

.container-livro {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.content {
  /* background: red; */
  height: 90%;
  width: 50%;

  display: flex;

  justify-content: center;
  align-items: center;
  text-align: left;
}

.content_direita {
  text-align: right;
}

.text0 {
  text-align: center;
  margin: 0 0 2rem 0;
  font-size: x-large;
}

.arrow {
  font-size: 25px;
  transition: 1s ease-out;

  width: 30px;
  height: 30px;
  border-radius: 30px;

  display: flex;
  align-items: center;
  justify-content: center;
}

.arrow:hover {
  background-color: rgb(255, 181, 181);
}
</style>
