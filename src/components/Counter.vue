<template>
  <p>{{ count }}</p>
  <button @click="count++">incr</button>
  <button @click="count--">decr</button>
  <button @click="count = 0">reset</button>
</template>

<script lang="ts">
import { ref, defineComponent } from "vue";
export default defineComponent({
  name: "Counter",
  setup: () => {
    const count = ref(0);
    return { count };
  },
});
</script>
