<template>
  <svg class="icon" :class="className" :width="size" :height="size">
    <use :xlink:href="`${props.icon}`"></use>
  </svg>
</template>

<script setup>
const props = defineProps({
  icon: {
    type: String,
    required: true
  },
  size: {
    type: [String, Number],
    default: '24'
  },
  className: {
    type: String,
    default: ''
  }
})
</script>

<style scoped>
.icon {
  display: inline-block;
  vertical-align: middle;
}
</style>
