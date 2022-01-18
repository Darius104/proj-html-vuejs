<template>
  <div id="app">
    <Header :element="headerArray"/>
    <Main :element="sottoHeaderArray"/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
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
      ],

      sottoHeaderArray: [
        {
          image: './assets/drink.jpg',
          title: "Crossfit",
          subtitle: "Push your limits"
        },
        {
          image: './assets/box1-2x.jpg',
          title: 'New gym apparel',
          subtitle: 'Look good, feel good'
        },
        {
          image: './assets/box3-2x.jpg',
          title: 'Team training',
          subtitle: 'Find a partner'
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