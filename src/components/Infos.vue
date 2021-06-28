<template>
    <header>
        <div class="Box">
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Agora é ofical : o Windows 11 está vindo</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga. Harum repellat magni delectus quis similique.</p>
            </div>
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Agora é ofical : o Windows 11 está vindo</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga. Harum repellat magni delectus quis similique.</p>
            </div> 
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>  
                <h1>Agora é ofical : o Windows 11 está vindo</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga. Harum repellat magni delectus quis similique.</p>
            </div> 
            <div class="elementsBox">
                <span class="iconsAll">{{time}} de {{mes}}, {{ano}}
                    <span class="btnS"><Button/></span>
                </span>
                <h1>Agora é ofical : o Windows 11 está vindo</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores labore molestiae odit, blanditiis, officia nihil facere tempora id laudantium velit sequi repellendus nam fuga. Harum repellat magni delectus quis similique.</p>
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
        mes: new Date().getMonth()
    }),
    components:{
        Button
    },
    methods:{
    }
}
</script>

<style scoped>
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
        flex-wrap: wrap;
        box-shadow: 1px 1px 5px 1px #31313159;
        background-color: whitesmoke;
        padding:15px;
        margin:8px 8px;
        width:auto;
        height: auto;
        border-radius: 2px;
    }
    .btnS:active{
        border-radius: 50%;
        background-color: red;
    }
</style>