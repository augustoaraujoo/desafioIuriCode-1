<template>
    <nav class="container">
        <div class="elementsNav">
            <h2 >Codelândia</h2>
            <h2>blog</h2>

            <div v-if="viewIcon">
                <img :src="iconImg" @click="viewIcons" class="iconBtn">
            </div>

            <div v-else>
                <img :src="iconImg2" @click="viewIcons" class="iconBtn">
            </div>
        </div>

    <div class="inputC"><Input/></div>

    </nav>
    <header>
        <Infos/>
    </header>
</template>
<script>
import Input from './Input.vue'
import Infos from './Infos.vue'
export default {
    data:()=>({
            viewIcon:true,
            iconImg:'img/sol.png'
    }),
    components:{
        Input,
        Infos
    },
    methods:{
        viewIcons(){
            this.viewIcon = !this.viewIcon
            if(!this.viewIcon){
                this.iconImg2 ='img/night.png'
            }
        }
    }
}
</script>
<style>
    .container{
        
            z-index: 1;
            position:sticky;
            top: 0px;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        height: 30vh;
        background-image: linear-gradient(to right,#574AE8,#3EA1DB);
        
    }
    .elementsNav{
        width:100%;
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: space-around;
    }
    .inputC{
        margin: 10px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
    .iconBtn{
        width: auto;
        height: auto;
        border: none;
        background-color: transparent;
    }

     @media only screen and (max-width:768px){
      
     }
</style>