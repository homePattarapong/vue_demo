<template>
  <div app="demo2">
      <h1>Event and Method</h1>
      <button v-on:click="clickMe">Click Me</button>
      <button v-on:click="clickMe2('Welcome to VueJS')">Click Me2</button>
      <button @click="clickMe3('Welcome to Website')">Click Me3</button>
      <h3>{{getTimestamp()}}</h3>
  </div>
</template>

<script>
export default {
    name:"Demo2",
    mounted(){
        this.initial()
    },
    methods: {
        initial(){
            console.log("Initailization");
        },
        clickMe(){
            alert("Hi")
        },
        clickMe2(message){
            alert(message);
        },
        clickMe3(message){
            alert(message);
        },
        getTimestamp(){
            return Date();
        }
    },
}
</script>

<style>

</style>