<template>
  <div>
    <LikeHeader header-text="hello">
      <h3>初めまして</h3>
    </LikeHeader>
    <LikeNumber :total-number="number" @my-click="number = $event"></LikeNumber>

    <button @click="currentComponent = 'Home'">Home</button>
    <button @click="currentComponent = 'About'">About</button>
    <component :is="currentComponent"></component>
    <!-- <About v-if="currentComponent === 'About'"></About>
    <Home v-if="currentComponent === 'Home'"></Home> -->
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader";
import About from "./components/About";
import Home from "./components/Home";


export default {
  data() {
    return {
      number: 14,
      currentComponent: "Home"
    }
  },
  components: {
    LikeHeader: LikeHeader,
    About,
    Home,
  }
};
</script>

<style scoped>
  div {
    border: blue 1px solid;
  }
  h1 {
    color: red;
  }
</style>
