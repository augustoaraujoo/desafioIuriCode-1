<template>
    <header>
        <div class="Box" v-if="verLista">
            <button @click="ClickLista"></button>
            
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Agora é ofical : o Windows 11 está vindo</h1>
                <p>{{lorem}}</p>
            </div>
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Como estudar melhor</h1>
                <p>{{lorem}}</p>
            </div> 
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>  
                <h1>Quando e como utilizar um Framework</h1>
                <p>{{lorem}}</p>
            </div> 
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Aprenda a programar em JavaScript</h1>
                <p>{{lorem}}</p>
            </div>
        </div>
        <div v-else id="else">
           <button  @click="ClickLista">retorne</button>
            <div>
                <input type="text" placeholder="digite o Título" v-model="inputTask">
                <input type="text" placeholder="digite o texto" v-model="texto">
                
                    <h1  v-for="inputV in inputValue"
                     :key="inputV">{{inputV}}
                    </h1>
                    <p v-for="txt in textValue" :key="txt">
                        {{txt}}
                    </p>
                    <button @click="newText">confirmar</button>
            </div>
            
        </div>
    </header>
</template>

<script>
import Button from './Button.vue'
export default {
    data:()=>({
        time:new Date().getDate(),
        ano: new Date().getFullYear(),
        mes: new Date().getMonth(),
        lorem:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga.Lorem ipsum dolor sit amet consectetur ae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga.',

        verLista: true,
        inputValue:[""],
        inputTask:'',

        textValue:[""],
        texto:''
    }),
    components:{
        Button
    },
    methods:{
        ClickLista(){
            this.verLista = !this.verLista
        },
        newText(){
            if(this.inputTask === '' || this.texto ===''){
                return false
            }else{
                this.inputValue.push(this.inputTask)
                this.textValue.push(this.texto)
            }
        }
    }
}

</script>

<style scoped>
    li{
        color: rgb(243, 240, 240);
    }
    ul{
        display: flex;
        justify-content: center;
        height: 30vh;
        background: #181818;
    }
    .iconsAll{
        display: flex;
        width: 100%;
        position: relative;
        top: 5px;
        flex-direction: row;
        justify-content: space-between;
    }
    header{
        display: flex;
        justify-content: center;
        margin: 5px;
    }
    .Box{
        width: 75vw;
        height: 100%;
        margin: 10px 10px;
    }
    span{
        position: relative;
        top: -10px;
        font-family: 'Lexend Deca';
        text-align: center;
        font-size: 11pt;
        color: gray;
    }
    .elementsBox{
        display: flex;
        flex-wrap:wrap;
        box-shadow: 1px 1px 5px 1px #31313159;
        background-color: whitesmoke;
        padding:20px;
        margin:25px 25px;
        width:auto;
        height:auto;
        border-radius: 2px;
        
    }
    @media only screen and (max-width:768px){
        .Box{
             width: 100%;
             background-color: red;
        }

        .elementsBox{
            background-color: green;
            height: 50%;
        }
    }
</style>