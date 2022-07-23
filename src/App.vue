<template>
  <Shot shot_count=3 />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Shot from './components/Shot.vue';

@Options({
  components: {
    Shot,
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
