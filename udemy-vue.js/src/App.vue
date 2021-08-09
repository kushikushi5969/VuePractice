<template>
  <div>
    <LikeHeader header-text="hello">
      <h2>みなさん</h2>
      <template v-slot:title>
        <h1>こんにちは</h1>
      </template>
      <h3>初めまして</h3>
      <p>よろしくお願いします</p>
      <template v-slot:number>
        <h2>{{number}}</h2>
      </template>
    </LikeHeader>
    <LikeNumber :total-number="number" @my-click="number = $event"></LikeNumber>
    <LikeNumber :total-number="number"></LikeNumber>
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader";

export default {
  data() {
    return {
      number: 14
    }
  },
  components: {
    LikeHeader: LikeHeader
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
