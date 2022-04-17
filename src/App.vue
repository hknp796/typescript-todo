<template>
  <div>{{name}}--{{age}}</div>
  <button @click="changeName('hell')">change name</button>
  <button @click="changeAge(40)">change age</button>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  components: {},
  data(){
    return{
      name:'hari' ,
      age:40 ,
    }
  },methods:{
    changeName(name:string){
      this.name = name
    },
    changeAge(age:number){
      this.age= age
    }
  }
});
</script>

<style>
</style>
