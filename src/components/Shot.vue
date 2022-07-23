<template>
<h1>Shot {{ shot_count }}</h1>
  <div class="paper_body">i am in the shot component</div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    shot_count: Number,
  },
})
export default class Shot extends Vue {
  shot_count!: number;
}
</script>

<style scoped></style>