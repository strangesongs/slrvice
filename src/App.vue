<template>
  <div class="taped_photograph">
    <img alt="tape" class="tape" src="./assets/ancient_removed_tape.gif" />
    <img alt="back of old photograph" width="400" src="./assets/paper_old_back_of_photograph.png" />
  </div>
  
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
.taped_photograph {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.tape {
  margin-bottom: -2.5em;
  z-index: 1;
}
</style>
