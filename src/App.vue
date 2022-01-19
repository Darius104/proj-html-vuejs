<template>
  <div id="app">
    <Header :element="headerArray"/>
    <Main :element="sottoHeaderArray" :playlist="playlistArray" :subscribe="subscribeArray" :buy="buyArray"/>
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
          image: require('./assets/drink.jpg'),
          title: "Crossfit",
          subtitle: "Push your limits"
        },
        {
          image: require('./assets/box1-2x.jpg'),
          title: 'New gym apparel',
          subtitle: 'Look good, feel good'
        },
        {
          image: require('./assets/box3-2x.jpg'),
          title: 'Team training',
          subtitle: 'Find a partner'
        }
      ],

      playlistArray: [
        {
          image: require('./assets/video2-2x.jpg'),
          title: "Thighs & glute workout",
          subtitle: "Increase your mobility"
        },
        {
          image: require('./assets/video7-2x.jpg'),
          title: "Lift, firm & perk up",
          subtitle: "Feel young again"
        },
        {
          image: require('./assets/video9-2x.jpg'),
          title: "Slim & tirm your waist",
          subtitle: "Shed those extra pounds"
        }
      ],

      subscribeArray: [
        {
          title: "Team training",
          subtitle: "Find a parner",
          desc: "Vesribulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senecrus eget sed duis vehicula. Tristique.",
          span: "Find a partner >"
        },
        {
          title: "Crossfit workout",
          subtitle: "Push your limits",
          desc: "Vesribulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senecrus eget sed duis vehicula. Tristique.",
          span: "Learn about Crossfit >"
        },
        {
          title: "Weight loss plan",
          subtitle: "Shed those pounds",
          desc: "Vesribulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senecrus eget sed duis vehicula. Tristique.",
          span: "Schedule a workout >"
        }
      ],

      buyArray: [
        {
          image: require('./assets/blog4-2x-400x258.jpg'),
          title: "The best protein shake",
          subtitle: "By admin | November 26th, 2019 | Gym"
        },
        {
          image: require('./assets/blog1-2x-400x258.jpg'),
          title: "Ultimate cardio workout",
          subtitle: "By admin | November 26th, 2019 | Gym"
        },
        {
          image: require('./assets/blog3-2x-400x258.jpg'),
          title: "New juices available now",
          subtitle: "By admin | November 26th, 2019 | Gym"
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