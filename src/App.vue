<template class="dark">
  <div>
    <PagePrinc/>
    <h1 @click="dark"><img :src="iconImg" alt="img sol/lua"></h1>
  </div>
</template>

<script>
import PagePrinc from './components/PagePrinc.vue'
export default {
  name: 'App',
  components: {
    PagePrinc
  },
  data:()=>({
            viewIcon:true,
            iconImg:'img/sol.png'
  }),
  methods:{
    dark(){
       var element = document.body;
       element.classList.toggle("dark");
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Lexend+Deca&display=swap');

html{
    --bg:#2F3136;
}
.dark{
  background-color: var(--bg);
  color: white;
}

    img,svg{cursor: pointer;}

    h1{
        cursor: text;
        text-align:start;
        font-size: 20pt;
        color: #313131;
        font-family: 500;
        font-family: 'Lexend Deca', sans-serif;
    }
      p{
        cursor: text;
        font-size: 12pt;
        padding: 10px;
        text-align: justify;
        color:#B6B6B6;
        font-weight: 100;
        font-family: 'Inter', sans-serif;
    }
    
    h2{
        color: #ffffff;
        font-family: 500;
        font-family: 'Lexend Deca', sans-serif;
    }
  body{
    color: #FFFF;
    width: 100%;
    height: 100%;
    padding:0;
    margin:0;
    background-color: #F3F5F7;
  }


</style>
