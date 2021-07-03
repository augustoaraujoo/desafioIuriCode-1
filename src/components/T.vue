<template>
  
    <div>
        <input type="text" v-model="query">
        <button @click="computedList"></button>
        <ul>
            <li
            v-for="lis in list"
            :key="lis">{{lis.msg}}</li>
        </ul>
    </div>
</template>
<script>
export default {
data:()=>({
    query: '',
    list: [
      { msg: 'Bruce Lee' },
      { msg: 'Jackie Chan' },
      { msg: 'Chuck Norris' },
      { msg: 'Jet Li' },
      { msg: 'Kung Fury' }
    ],
    methods:{
            
        }
})
}
</script>
<style>
    ul,li{
        background-color:black;
    }
</style>