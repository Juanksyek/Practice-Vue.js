<template>
  <h1>Hello {{ email }}</h1>
  <h1>Mobile: {{ mobile }}</h1>
  <h1>Name: {{ getName1("Juan") }}</h1>
  <h1>Name 2: {{ getName1("Carlos") }}</h1>
  <h1>Data: {{ getData().phone }}</h1>
  <button v-on:click="fun()">Click here</button>
  <h1 v-on:mousemove="getConsole('')">Home page </h1>
</template>
<script>
export default {
  name: "PAGES",
  data() {
    return {
      email: "abc@gmail.com",
      mobile: "55555",
    };
  },
  methods: {
    getName1(name){
      return name;
    },
    getData(){
      return{
        email: "abc.gmail.com",
        phone: "99999999",
      };
    },
    fun(){
      alert("How are you");
    },
    getConsole(){
      console.error("Function is running");
    },
  },
};
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>
  