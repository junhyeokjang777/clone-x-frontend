<template>
  <div>
    <input
      :type="type"
      :placeholder="placeholder"
      :value="modelValue"
      @input="updateValue"
    >
  </div>
</template>

<script>
export default {
  name: "inputField",

  props: {
    type: String,
    placeholder: String,
    modelValue: String,
  },

  emits: ['update:modelValue'],

  methods: {
    updateValue(event) {
      this.$emit('update:modelValue', event.target.value)
    }
  }
}
</script>

<style>
</style>

