<template>
    <nav class="container">
        <div class="elementsNav">
            <h2>Codelândia</h2>
            <h2>blog</h2>
        </div>
                <div class="inputC">
                    <Input/>
                </div>
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

    }),
    components:{
        Input,
        Infos
    }
}
</script>
<style>
    .container{
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
    /*
    Titulo
        #313131
    descri 
        #B6B6B6
        
    */
</style>