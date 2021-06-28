<template>
<div class="inputContainer">
        <input type="search" id="input" placeholder="Pesquisar no blog" v-model="getValue">
        <button @click="active">{{}}</button>
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
        background-color: rgba(0, 0, 255, 0.089);
        border: none;
        border-radius: 5px;
        height: 3rem;
        width: 60%;
    }
</style>