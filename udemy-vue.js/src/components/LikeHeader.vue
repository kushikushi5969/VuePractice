<template>
  <div>
    <slot name="title" :user="user"></slot>
    <slot></slot>
    <hr>
    <p>いいねの数</p>
    <slot name="number"></slot>
    <!-- <p>{{headerText}}</p> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        fisrstName: "Jack",
        lastName: "Daniel"
      }
    }
  }
}
</script>
