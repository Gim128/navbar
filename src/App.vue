<template>
    <v-main>
      <navbar-component />
      <hero-component />
      <feature-component />
      <footer-component />
    </v-main>
         
</template>

<script>
import FooterComponent from './components/FooterComponent.vue';
import HeroComponent from './components/HeroComponent.vue';
import FeatureComponent from './components/FeatureComponent.vue';
import NavbarComponent from './components/NavbarComponent.vue';



export default {
  name: 'App',

  components: {
    NavbarComponent,
    HeroComponent,
    FeatureComponent,
    FooterComponent,
},

  data: () => ({
    //
  }),
};
</script>
