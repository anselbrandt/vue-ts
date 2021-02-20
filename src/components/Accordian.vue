<template>
  <label> <input type="checkbox" v-model="useScriptSetup" /> Show A </label>
  <label> <input type="checkbox" v-model="useTsPlugin" /> Show B </label>
  <p>
    Dynamic content:
    <template v-if="!useScriptSetup"> Default </template>
    <template v-else> Option A </template>
  </p>
  <p v-if="useTsPlugin">Content B</p>
</template>

<script lang="ts">
import { ref, defineComponent } from "vue";
export default defineComponent({
  name: "Accordian",
  setup: () => {
    const useScriptSetup = ref(false);
    const useTsPlugin = ref(false);
    return { useScriptSetup, useTsPlugin };
  },
});
</script>
