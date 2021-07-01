<template>
<div class="inputContainer">
        <input type="search" id="input" placeholder="Pesquisar no blog" 
         @keyup="viewFilter"
         v-model="getValue.infos"
         >
        <button @click="viewFilter"></button>
</div>
</template>

<script>
export default {
    data:()=>({
        getValue:[
            
        ]
    }),
    methods:{
        viewFilter(){
            
        }
    }
}
</script>

<style scoped>
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
        background: royalblue;
        border:none;
        border-radius: 5px;
        height: 3rem;
        width: 50%;
    }
</style>