<template>
  <div id="app">
    <grid :data="gridData" :columns="gridColumns"></grid>
  </div>
</template>

<script>
import Grid from './components/Grid.vue';

export default {
  name: 'app',
  data() {
  return {
      gridData: [
        { name: 'American alligator', location: 'Southeast United States' },
        { name: 'Chinese alligator', location: 'Eastern China' },
        { name: 'Spectacled caiman', location: 'Central & South America' },
        { name: 'Broad-snouted caiman', location: 'South America' },
        { name: 'Jacaré caiman', location: 'South America' },
        { name: 'Black caiman', location: 'South America' },
                { name: 'Jacaré caiman', location: 'South America' },
        { name: 'Black caiman', location: 'South America' },
                { name: 'Jacaré caiman', location: 'South America' },
        { name: 'Black caiman', location: 'South America' },
                { name: 'Jacaré caiman', location: 'South America' },
        { name: 'Black caiman', location: 'South America' },
                { name: 'Jacaré caiman', location: 'South America' },
        { name: 'Black caiman', location: 'South America' },
      ],
      gridColumns: ['name', 'location'],        
    }
  },
  components: {
    Grid,
  },
};
</script>

<style lang="scss" scoped>
@import "./scss/style.scss"; 

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
// Outer-Most <div> in a 'vue' Component
.wrapper, .container {
  // width: 100%;
  width: 75%;
  padding: 0 1rem;
  margin: 0 auto;
}
</style>
