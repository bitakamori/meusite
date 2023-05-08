<script>
</script>

<template>
  
  <div class="complexo">
  <main>
    <div class="box1"> 
      <div class="container-img">
      <img  src="@/assets/adv.jpeg" />
    </div>
    <div class="content">
      <div class="center">
        Estudei a vida toda no colegio Adventista, onde o pastor falava para criancinhas que quem não guardasse o sabado iam para o inferno. &nbsp; &nbsp; 
         &#10024; gratidão &#10024; 
      
        </div>
     </div>
    </div>

    <div class="box2">
      <div class="content2">
       <div class="center2">
       Fiz Radiologia, e quando estava prestes a me formar e praticamente contratada, percebi que nao seria feliz na área e resolvi mudar de caminho. 
        </div>
      </div>
      <div class="container-img2">
        <img  src="@/assets/tcc.png" />
      </div>
    </div>  

    <div class="box3"> 
      <div class="container-img3">
      <img  src="@/assets/vue.png" />
    </div>
    <div class="content3">
      <div class="center3">
        Dias após a decisão de mudar de área, surgiu a vaga para fazer este curso de programação e sou muito grata pela oportunidade. 
        </div>
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
  height: 250px;
  width: auto;
  border-radius: 50%;
  margin-top: 6rem;
  margin-left: 13rem;
  
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
  /* margin: 4rem; */
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
  height: 350px;
  width: auto;
  border-radius: 8px;
  margin: 3rem;
  margin-left: 8rem;
 }

 .content2 {
  /* background: rgb(94, 6, 6); */
  height: 90%;
  width: 50%;
  
}

 .center2{
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  /* background: rgb(51, 36, 36); */
  margin-left: 8rem;
  margin-right: 2rem;
  margin-top: 10rem;
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
  border-radius: 8px;
  margin: 3rem;
  margin-left: 13rem;
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
  margin-top: 14rem;
 }


 



 /* div.complexo > footer{
  background: purple;
  flex-grow: 1;
 } */

</style>

