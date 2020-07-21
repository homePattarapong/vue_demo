<template>
  <div>
    <h1>{{title}}</h1>
    <h2>{{count}}</h2>
    <button @click="onClickAdd">Add</button>
  </div>
</template>

<script>
export default {
  name:"app",
  data() {
    return {
      title:"Click & Count ",
      count:0
    }
  },
  methods: {
    onClickAdd(){
      this.count=this.count+1
    }
  },
}
</script>

<style>

</style>