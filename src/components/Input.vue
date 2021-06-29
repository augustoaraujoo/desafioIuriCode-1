<template>
<div class="inputContainer">
        <input type="search" id="input" placeholder="Pesquisar no blog" 
         @keyup.enter="viewFilter"
         v-model="getValue.infos"
         >
        <button @click="viewFilter"></button>
</div>
</template>

<script>
export default {
    data:()=>({
        getValue:[

            {id:1,infos:'windos'},
            {id:2,infos:'qual frame'},
            {id:3,infos:'team fire'},
            {id:4,infos:'js'}
        ]
    }),
    methods:{
        viewFilter(){
            console.log(this.getValue.filter(function(p){
                return p.id >=9
            }))
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