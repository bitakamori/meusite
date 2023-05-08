<script>
</script>

<template>
  
  <div class="complexo">
  <main>
    <div class="box1"> 
      <div class="container-img">
      <img  src="@/assets/nn.png" />
    </div>
    <div class="content">
      <div class="center">
        Essa sou eu, Bianca Helena Takamori Ribeiro, nascida no dia 14 de março de 1998 em Campo Mourão, interior do paraná. 
        </div>
     </div>
    </div>

    <div class="box2">
      <div class="content2">
       <div class="center2">
        Esta é minha familia. A melhor mãe do mundo, o irmão mais cool do planeta, e a irmã mais fofa do universo. 
        <div class="img-text">
      <img  src="@/assets/nina.png" />
      <div class="text" > &nbsp;  muito fofa mesmo 😍 </div>
    </div>
        
        </div>
      </div>
      <div class="container-img2">
      <img  src="@/assets/family.png" /> 
      </div>
    </div>  

    <div class="box3"> 
      <div class="container-img3">
      <img  src="@/assets/amor.png" />
    </div>
    <div class="content3">
      <div class="center3">
        Essa é minha outra familia, o homem mais incrivel da via láctea, que faz meus dias mais felizes, que me apoia em tudo e sempre esta la quando eu preciso ❤️
        </div>
     </div>
    </div>

    <div class="box4">
      <div class="text0" > Filhos</div>
      <div class="img-text2">
        <img  src="@/assets/fotos/ox.png" />
        <img  src="@/assets/fotos/ox2.png" />
        <img  src="@/assets/fotos/ox3.png" />
      </div>
      <div class="text2" > Ox, a amante n°1 em tapinha na bundinha</div>

      <div class="img-text2">
        <img  src="@/assets/fotos/t.png" />
        <img  src="@/assets/fotos/t2.png" />
        <img  src="@/assets/fotos/t3.png" />
      </div>
      <div class="text2" > Thor, o apreciador do cochilinhos </div>

      <div class="img-text2">
        <img  src="@/assets/fotos/tl.png" />
        <img  src="@/assets/fotos/tl2.png" />
        <img  src="@/assets/fotos/tl3.png" />
      </div>
      <div class="text2" > Tesla, o caçula mimado que adora passear</div>
   
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



  /* footer{
  background: purple;
  height: 200px;
  flex-grow: 1;
 } */

</style>
