<template>
<div id="fs">
  <div id="poli1"></div>
  <h1>About us</h1>
  <div id="mainwrap">
    <div class="ploscica" id="p1">Lorem ipsum dolor sit amet consectetur adipisicing elit. Id fugit quo recusandae suscipit soluta adipisci omnis illum, tempora sed at sequi, rem nobis corporis blanditiis dolores reprehenderit ut? Ullam quaerat mollitia accusantium id. Soluta, enim officia at exercitationem magni cupiditate sunt ullam similique eius nam? Ducimus nihil nulla architecto provident suscipit totam dignissimos tenetur quam, ut, nemo quia recusandae blanditiis dicta, eum aut. Iusto eveniet explicabo tenetur aperiam dicta, ea temporibus praesentium veritatis magni perspiciatis provident numquam illum, deleniti voluptates animi laboriosam laudantium culpa ipsum, veniam iure necessitatibus asperiores molestiae sunt illo? Est illo distinctio ipsam? Tenetur perferendis ut iure.</div>
    <div class="ploscica" id="p2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum optio, at nihil hic reiciendis, aspernatur dolor atque ad totam ipsa corrupti quae laboriosam molestias debitis perferendis possimus eum sint veniam libero eveniet dignissimos dicta corporis! Eaque dolorem enim culpa totam sit debitis nulla dicta nihil saepe! Tenetur magni debitis sapiente itaque reiciendis, delectus quae neque, dolore, repellendus tempore veritatis beatae omnis impedit quis dolor libero molestiae? Dicta dignissimos beatae hic vitae totam assumenda maxime recusandae illum ipsam! Perferendis, est fugiat.</div>
    <div class="ploscica" id="p3">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Perspiciatis, illum! Alias, in dolor amet nesciunt nobis accusantium, porro quidem necessitatibus eligendi similique omnis architecto voluptates id delectus fugiat ea deleniti ex ut aspernatur, quibusdam aliquid? Molestiae asperiores quia numquam. Perferendis voluptatem quo itaque ullam iusto rem! Culpa ab repudiandae fugit tempora esse quaerat illo fugiat porro corporis rem, sapiente consequuntur distinctio tempore atque dolorum molestiae obcaecati repellat dicta, cumque dolore. Impedit sapiente harum veritatis magni quam dolorum voluptates ipsum, fugit consequatur, molestias a. Voluptates dolorum iure similique vitae excepturi, suscipit cupiditate mollitia eos consectetur minima fugit, assumenda aliquam repudiandae maiores doloribus quibusdam blanditiis repellat tempora eius explicabo alias, architecto eaque nam deserunt. Debitis reiciendis eligendi itaque accusamus odit similique, repudiandae nesciunt ipsam, maiores ratione porro doloremque corporis! Dolorem distinctio accusamus optio eligendi sed soluta natus voluptatibus numquam possimus placeat hic nesciunt esse odio eveniet commodi, delectus, nobis explicabo reprehenderit repellat.</div>
    <div  id="s1"></div>
    <div  id="s2"></div>
  </div>
  <div id="poli2"></div>
</div>
</template>

<script>

</script>

<style>
* {
    padding: 0;
    margin: 0;
}
#fs{
  position: relative;
  min-height: calc(100vh - 70px - 45px);
  display: flex;
  flex-direction: column;
}
#mainwrap{
  margin: 0 auto;
  padding: 20px;
  width: clamp(500px, 90vw, 1200px);
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto 1vh auto 1vh auto;
  gap:10px;
}
.ploscica{
  background-color: rgba(255, 255, 255, 0.95);
  border-radius: 3px;
  box-shadow: rgba(0, 0, 0, 0.6) 2px 2px 5px;
  text-align: left;
  margin:auto;
  padding: clamp(2px, 1rem ,20px);
}

#p1{
  grid-column: 1 /  4;
  grid-row: 1/ 2;
}
#p2{
  grid-column: 2 /  5;
  grid-row: 3/ 4;
}
#p3{
  grid-column: 1 /  4;
  grid-row: 5/ 6;
}
#s1{
  grid-column: 4 / 5;
  grid-row: 1/ 2;
  background-image: url("../../Icons/network.png");
  background-size: 50%;
  background-repeat: no-repeat;
  background-position: 30%;
}
#s2{
  grid-column: 4 /  5;
  grid-row: 5/ 6;
    background-image: url("../../Icons/coding.png");
  background-size: 50%;
  background-repeat: no-repeat;
  background-position: 70%;
}
#poli1{
  position: absolute;
  top:-45px;
  left: 0px;
  z-index: -99;
  width: 100%;
  height: 40vh;
  background-color: #5dc1ee;
  clip-path: polygon(0 0, 100% 0, 100% 50%, 0 100%);
}
#poli2{
  position: absolute;
  bottom: 0;
  z-index: -99;
  width: 100%;
  height: 40vh;
  background-color: #f8c025;
  clip-path: polygon(0 70%, 100% 0, 100% 100%, 0 100%);
}

h1{
  padding: 20px;
  text-decoration: underline;
}
/* za telefon */
@media only screen and (max-width: 770px) {
  #mainwrap{
  margin: 0 auto;
  padding: 20px;
  width: 90vw;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto 5rem auto 5rem auto;
  gap:10px;
  overflow: visible;
}
#p1{
  grid-column: 1 /  5;
  grid-row: 1/ 2;
}
#p2{
  grid-column: 1 /  5;
  grid-row: 3/ 4;
}
#p3{
  grid-column: 1 /  5;
  grid-row: 5/ 6;
}
#s1{
  margin: -3rem;
  grid-column: 3 / 4;
  grid-row: 2/ 3;
  background-image: url("../../Icons/network.png");
  background-size: fill;
  background-repeat: no-repeat;
}
#s2{
  margin: -3rem;
  grid-column: 2 /  3;
  grid-row: 4/ 5;
  background-image: url("../../Icons/coding.png");
  background-size: fill;
  background-repeat: no-repeat;
}
}
</style>

