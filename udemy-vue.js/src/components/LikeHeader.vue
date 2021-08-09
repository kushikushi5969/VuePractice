<template>
  <div>
    <slot name="title"></slot>
    <slot></slot>
    <hr>
    <p>いいねの数</p>
    <slot name="number"></slot>
    <p>{{headerText}}</p>
  </div>
</template>

<script>
export default {
  props: ['headerText']
}
</script>
