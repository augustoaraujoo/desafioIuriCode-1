<template>
  <div>
    <PagePrinc/>
  </div>
</template>

<script>
import PagePrinc from './components/PagePrinc.vue'
export default {
  name: 'App',
  components: {
    PagePrinc
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Lexend+Deca&display=swap');
   
    h1{
        text-align:start;
        font-size: 20pt;
        color: #313131;
        font-family: 500;
        font-family: 'Lexend Deca', sans-serif;
    }
      p{
        font-size: 12pt;
        padding: 10px;
        text-align: start;
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
  height: 100vh;
  padding:0;
  margin:0;
  background-color: #F3F5F7;
}
</style>
