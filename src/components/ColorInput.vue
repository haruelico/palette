<template>
  <div class='input'>
    <input type="color" :id="label" v-model="syncData">
    <label :for="label">{{label}} {{ value }}</label>
  </div>
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: "#eeeeee"
    },
    label: {
      type: String,
      required: true
    }
  },
  computed: {
    syncData: {
      get: function() {
        return this.value;
      },
      set: function(val) {
        this.$emit("input", val);
      }
    }
  }
};
</script>

<style scoped>
input[type="color"] {
  margin-right: 10px;
}

.input {
  margin-bottom: 5px;
}
</style>
