<template>
  <div></div>
</template>

<script>
export default {
  props: {
    a: {
      type: Object,
      // `{ val: 1 }`
      default: function () {
        return {
          val: 1
        }
      }
    },
    b: {
      type: Object,
      // `{ val: 1, a: 2 }`
      default: () => ({ val: 1, a: 2 })
    },
    c: {
      type: Object,
      // `{ val: 1}`
      default(){
        return { val: 1 }
      }
    }
  }
}
</script>
