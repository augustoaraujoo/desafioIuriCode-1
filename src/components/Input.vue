<template class=".dark">
<div class="inputContainer">
<<<<<<< HEAD
        <input type="search" id="input" placeholder="Pesquisar no blog">
=======
        <input type="search" id="input" placeholder="Pesquisar no blog" 
         @keyup="viewFilter"
         v-model="getValue.infos"
         >
        <button @click="viewFilter"></button>
>>>>>>> b74252559a9db5ea5181a28a13415871178fc2d8
</div>
</template>

<script>
export default {
    data:()=>({
<<<<<<< HEAD

    }),
    methods:{

     }
=======
        getValue:[
            
        ]
    }),
    methods:{
        viewFilter(){
            
        }
    }
>>>>>>> b74252559a9db5ea5181a28a13415871178fc2d8
}
</script>

<style scoped>
    h1{
        background-color: rebeccapurple;
    }
    input::placeholder{
        color: white;
        font-size: 11pt;
    }
    input{
        color: white;
    }
    .inputContainer{
        display: flex;
        justify-content: center;
        width: 100%;
    }
    #input{
        background: royalblue ;
        border:none;
        border-radius: 5px;
        height: 3rem;
        width: 55%;
    }
</style>

