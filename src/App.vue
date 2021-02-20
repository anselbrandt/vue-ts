<script lang="ts">
import { defineComponent } from "vue";
import Hero from "./components/Hero.vue";
import Title from "./components/Title.vue";
import Accordian from "./components/Accordian.vue";
import Counter from "./components/Counter.vue";
import InputBox from "./components/InputBox.vue";

export default defineComponent({
  name: "App",
  components: {
    Hero,
    Title,
    Accordian,
    Counter,
    InputBox,
  },
});
</script>

<template>
  <Hero />
  <Title msg="string prop from app" />
  <Accordian />
  <Counter />
  <InputBox />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
