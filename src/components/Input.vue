<template class=".dark">
<div class="inputContainer">
        <input type="search" id="input" placeholder="Pesquisar no blog">
</div>
</template>

<script>
export default {
    data:()=>({

    }),
    methods:{

     }
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

