<template>

  <div id="navbar">
      <div class="zavihek">Logo</div>
     <router-link to="/"> Home</router-link>
      <router-link to="/about">About</router-link>
  </div>
<router-view/>
</template>

<script>
export default {
    data(){
        return{
        }
    },
    methods:{
    }
}
</script>

<style>
* {
    padding: 0;
    margin: 0;
}

#navbar{
    z-index: 10;
    width: 100%;
    height: 45px;
    background-color: rgba(255, 255, 255, 0.664);
    display: grid;
    grid-template-columns: 2fr 1fr 1fr 1fr;
    gap: 10px;
    
}
#navbar a{
    margin: auto;
    width: 100px;
    padding-top: 5px;
    text-decoration: none;
    color: rgba(0, 0, 0, 0.815);
    font-size: 1.5rem;
    text-align: center;
    border-radius: 10px;
    font-weight: bold;
    transition: 0.2s;
}
#navbar a:hover{
    margin: auto;
    text-decoration: none;
    font-size: 1.5rem;
    text-align: center;
    color: rgba(48, 48, 48, 0.815);
}
#navbar a.router-link-exact-active {
  color: rgba(56, 56, 56, 0.815);
}
.zavihek{
    width: 100px;
    height: fit-content;
    margin: auto;
    padding: 10px 20px;
    border-radius: 10px;
    color: black;
}

</style>