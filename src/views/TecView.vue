<script>
</script>

<template>

  <div class="complexo">
  <main>
    <div class="box1"> 
      <div class="container-img">
      <img  src="@/assets/fotos/hp.png" />
    </div>
    <div class="content">
      <div class="center">
        Sou apaixonada pela leitura, adoro o poder de imersão que um livro proporciona. Meus gerenros preferidos são suspense, serial killer, 
        fantasia, ficção científica e livros de psicologia e autoajuda. 
        </div>
     </div>
    </div>

    <div class="box4">
      <div class="text0" > Livros favoritos</div>
      <div class="img-text2">
        <img  src="@/assets/fotos/js.png" />
        <img  src="@/assets/fotos/oimp.png" />
        <img  src="@/assets/fotos/ver.png" />
      </div>
    </div>

    

    <div class="box2">
      <div class="content2">
       <div class="center2">
        Adoro ver filmes e séries, e harry potter é meu confort film com gostinho de infancia. Meus generos preferidos são terror/suspense
        ficção científica e fantasia, pincipalmente com bons plot twist. E adoro séries de confeitaria e competições em geral. 
        </div>
      </div>
      <div class="container-img2">
      <img  src="@/assets/fotos/hpm.png" /> 
      </div>
    </div>  

    <div class="box4">
      <div class="text0" > Séries/Filmes favoritos</div>
      <div class="img-text2">
        <img  src="@/assets/fotos/spn.png" />
        <img  src="@/assets/fotos/herd.png" />
        <img  src="@/assets/fotos/mv.png" />
      </div>
    </div>

    <div class="box3"> 
      <div class="container-img3">
      <img  src="@/assets/fotos/rp.png" />
    </div>
    <div class="content3">
      <div class="center3">
        Amo fazer croche, principalmente amigurumis. É uma otima terapia. 
        </div>
     </div>
    </div>

    <div class="box4">
      <div class="text0" > Alguns amigurumis</div>
      <div class="img-text2">
        <img  src="@/assets/fotos/uni.png" />
        <img  src="@/assets/fotos/vd.png" />
        <img  src="@/assets/fotos/rs.png" />
      </div>
    </div>

    


  </main>
  
</div>



</template>

<style scoped>

div.complexo{
  display: flex;
  flex-direction: column;
  height: auto;
  width: auto;

  justify-content: space-around;
  align-items: space-around;
}


div.complexo main {
  /* background: palevioletred; */
  height: auto;
  display: flex;
  /* justify-content: space-between; */
  flex-direction: column;
 }
 
 .box1 {
  display: flex;
  justify-content: space-between;
  /* background: orange; */
  height: 500px;
  margin-top: 1rem;
 }

 div.container-img{
  height: 90%;
  width: 50%;
  /* background: yellow; */
  
 }

 div.container-img> img {
  height: 320px;
  width: auto;
  border-radius: 30%;
  margin: 3rem;
  margin-left: 9rem;
  margin-top: 4rem;
  
 }

 .content {
  /* background: red; */
  height: 90%;
  width: 50%;
  
}

 .center{
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  /* background: grey; */
  margin-left: 2rem;
  margin-right: 8rem;
  margin-top: 13rem;
 }

.box2{
  display: flex;
  justify-content: space-between;
  /* background: black; */
  height: 500px;
}  

 div.container-img2{
  height: 90%;
  width: 50%;
  /* background: rgb(58, 58, 2); */
 }

 div.container-img2> img {
  height: 320px;
  width: auto;
  border-radius: 20%;
  margin: 3rem;
  margin-left: 4rem;
 }

 .content2 {
  /* background: rgb(94, 6, 6); */
  height: 50%;
  width: 50%;
  
}

 .center2{
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  text-align: justify;
  /* background: rgb(51, 36, 36); */
  margin-left: 8rem;
  margin-right: 2rem;
  margin-top: 8rem;
 }

 /* .img-text {
  height: 250px;
  width: auto;
  background: black;
  margin-left: 8rem;
  margin-right: 2rem;
  margin-top: 2rem;

 } */

 div.img-text > img{
  height: 150px;
  width: auto;
  display: flex;
  border-radius: 50%;
  margin-top: 1rem;
 }


.box3{
  display: flex;
  justify-content: space-between;
  /* background: rgb(192, 65, 65); */
  height: 500px;
}

div.container-img3{
  height: 90%;
  width: 50%;
  /* background: rgb(58, 58, 2); */
 }

 div.container-img3> img {
  height: 350px;
  width: auto;
  border-radius: 50px;
  margin: 3rem;
  margin-left: 11rem;
  margin-top: 4rem;
 }

 .content3 {
  /* background: rgb(94, 6, 6); */
  height: 90%;
  width: 50%;
  
}

 .center3{
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  /* background: rgb(51, 36, 36); */
  margin-left: 2rem;
  margin-right: 8rem;
  margin-top: 13rem;
 }

 .box4{
  display: flex;
  flex-direction: column;
  /* background: rgb(192, 65, 65); */
  height: 500px;

}

.text0 {
  text-align: center;
  margin: 0 0 2rem 0;
  font-size:x-large;
}

.img-text2 {
  display: flex;
  justify-content: space-evenly;
  margin: 0 8rem 1rem 8rem;

}
div.img-text2 > img{
  height: 200px;
  width: 200px;
  object-fit: cover;
  border-radius: 100px;
  display: flex;
  
 }

 .text2 {
  text-align: center;
  margin: 1rem 0 5rem 0;
 }



 



 /* div.complexo > footer{
  background: purple;
  flex-grow: 1;
 } */

</style>