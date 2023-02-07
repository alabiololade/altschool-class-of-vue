<script>
// import {ColorPickerGame} from "./composables/ColorPickerGame.js"
import ColorPickerGame from "./components/ColorPickerGame.vue";
import Recap_01_02_2023 from "./components/Recap_01_02_2023.vue";

// const colors = ColorPickerGame("");

export default {
  components: { ColorPickerGame, Recap_01_02_2023 },
  data() {
    return {
      currentLesson: "color-picker-game",
    };
  },
};
</script>

<template>
  <ColorPickerGame v-if="currentLesson === 'color-picker-game'" />
  <Recap_01_02_2023 v-else />
</template>

<style scoped></style>
