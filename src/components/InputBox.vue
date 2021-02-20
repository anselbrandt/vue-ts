<template>
  <div>
    <p>{{ message }}</p>
    <input v-model="message" />
  </div>
</template>

<script lang="ts">
import { ref, defineComponent } from "vue";
export default defineComponent({
  name: "InputBox",
  props: {
    msg: {
      type: String,
      required: true,
    },
  },
  data: () => {
    return {
      message: "two way binding",
    };
  },
});
</script>
