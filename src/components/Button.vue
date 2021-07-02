<template>
    <div>
            <img :src="foto" :alt="descrição">
    </div>
</template>
<script>
export default {
    data:()=>{
        return{
            foto:'/img/coracaoPreto.png',
            descrição:'foto coraçao normal sem o click'
        }
    }
}
</script>
<style scoped>

</style>