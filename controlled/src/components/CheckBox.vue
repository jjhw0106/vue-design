<template>
  <input type="checkbox" :checked="modelValue" @input="toggleCheckBox">
</template>

<script>
export default {
  props:['modelValue'],
  methods: {
    toggleCheckBox() {
      console.log(this.v)
      this.$emit('update:modelValue', !this.modelValue)
    }
  }
}
</script>