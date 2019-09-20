<template>
  <tr>
    <td>
      <input
        :id="inputId"
        v-model="color"
        type="color"
      >
    </td>
    <td>
      <label class="style-name">{{ styleName }}</label>
    </td>
    <td>
      <label>{{ colorCode }}</label>
    </td>
  </tr>
</template>

<script>
export default {
  name: 'ColorInput',
  props: {
    colorCode: {
      type: String,
      required: true
    },
    styleName: {
      type: String,
      required: true
    },
    inputId: {
      type: String,
      required: true
    }
  },
  computed: {
    color: {
      get(){
        return this.colorCode
      },
      set(color){
        this.$emit('updateColor', {
          color, 
          key: this.inputId
        })
      }
    }
  }
}
</script>

<style scoped>
.style-name {
  padding-left: 5px;
}
</style>
