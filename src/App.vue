<template>
  <div id="app">
    <!-- <FormValid /> -->
    <!-- <DashBoard /> -->
    <!-- <ClientMakeMapping /> -->
    <ClientVariantMapping />
  </div>
</template>

<script>
//import FormValid from "./components/FormValid.vue";
//import DashBoard from "./components/DashBoard.vue";
//import ClientMakeMapping from "./components/ClientMakeMapping.vue";
import ClientVariantMapping from "./components/ClientVariantMapping.vue";
export default {
  name: "App",
  components: {
    // FormValid,
    //DashBoard,
    //  ClientMakeMapping,
    ClientVariantMapping,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  height: 100vh;
}
</style>
