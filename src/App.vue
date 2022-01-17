<template>
  <div id="app">
    <Header :element="headerArray"/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
  data: function(){
    return{
      headerArray: [
        {
          name: "Home",
          active: true,
        },
        {
          name: "Services",
          active: false,
        },
        {
          name: "About",
          active: false,
        },
        {
          name: "Blog",
          active: false,
        },
        {
          name: "Store",
          active: false,
        }
      ]
    }
  }
};
</script>

<style lang="scss">
@import './style/reset.scss';
@import '../node_modules/bootstrap';


</style>