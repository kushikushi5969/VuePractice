<template>
  <div>
    <slot></slot>
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
