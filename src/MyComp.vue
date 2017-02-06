<template>
  <div>
    {{ functionProp('value') }}
  </div>
</template>

<script>
export default {
  props: {
    functionProp: {
      type: Function,
      default (x) {
        return 'Default function result: ' + x
      }
    }
  },
  created () {
    console.log(this.functionProp)
  }
}
</script>
