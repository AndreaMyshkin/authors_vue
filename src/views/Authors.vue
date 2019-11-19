
<template>
    <div>
    <h1>All authors</h1>


    <router-link :to="{ name:'authors', params:{id:item}}"
     v-for="(item, index) of authorsArray" :key="index">
<button>{{item}}</button>
    </router-link>
       <Author/>
       <button @click='next'>next</button>
       <button @click='previous'> previous</button>
    </div>
    </template>


<script>

import Author from '../components/Author';

   export default {
       name: 'Authors',
       components:{
           Author
       },
       data(){
           return{
               authorsArray:["Lucretius", "Apuleius", 'Cicero']
           }
       },
       methods:{
           next(){
               this.$router.go(1);
               console.log('jejeje')
           },
           previous(){
               this.$router.go(-1)
           }
       }
   }


</script>