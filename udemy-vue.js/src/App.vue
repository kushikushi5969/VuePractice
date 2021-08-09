<template>
  <div>
    <LikeHeader></LikeHeader>
    <LikeNumber></LikeNumber>
  </div>
</template>

<script>
import LikeHeader from "./components/LikeHeader";

export default {
  components: {
    LikeHeader: LikeHeader
  }
};
</script>

<style scoped>
  div {
    border: blue 1px solid;
  }
</style>
