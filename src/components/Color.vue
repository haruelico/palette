<template>
  <div id="color">
    <table>
      <color-input
        v-for="(cs, key) in codeStyle"
        :key="key"
        class="code-color-input"
        :color-code="cs"
        :input-id="key"
        :style-name="styleName[key]"
        @updateColor="updateColor"
      />
    </table>
  </div>
</template>

<style scoped>
.code-color-input + .code-color-input {
  margin-top: 5px;
}
</style>

<script>
import ColorInput from './ColorInput.vue'

export default {
  name: "Color",
  components: {
    ColorInput
  },
  props: {
    codeStyle: {
      type: Object,
      required: true
    }
  },
  data: function() {
    return {
      styleName: {
        "--hljs-background-color": "Background color",
        "--hljs-keyword": "Keyword",
        "--hljs-built_in": "Built in",
        "--hljs-type": "Type",
        "--hljs-literal": "Literal",
        "--hljs-number": "Number",
        "--hljs-regexp": "RegExp",
        "--hljs-string": "String",
        "--hljs-subst": "Subst",
        "--hljs-symbol": "Symbol",
        "--hljs-class": "Class",
        "--hljs-function": "Function",
        "--hljs-title": "Title",
        "--hljs-params": "Params",
        "--hljs-comment": "Comment",
        "--hljs-doctag": "Doctag",
        "--hljs-meta": "Meta",
        "--hljs-meta-keyword": "Meta Keyword",
        "--hljs-meta-string": "Meta String",
        "--hljs-section": "Section",
        "--hljs-tag": "Tag",
        "--hljs-name": "Name",
        "--hljs-builtin-name": "Builtin Name",
        "--hljs-attr": "Attr",
        "--hljs-attribute": "Attribute",
        "--hljs-variable": "Variable",
        "--hljs-bullet": "Bullet",
        "--hljs-code": "Code",
        "--hljs-emphasis": "Emphasis",
        "--hljs-strong": "Strong",
        "--hljs-formula": "Formula",
        "--hljs-link": "Link",
        "--hljs-quote": "Quote",
        "--hljs-selector-tag": "Selector Tag",
        "--hljs-selector-id": "Selector Id",
        "--hljs-selector-class": "Selector Class",
        "--hljs-selector-attr": "Selector Attr",
        "--hljs-selector-pseudo": "Selector Pseudo",
        "--hljs-template-tag": "Template Tag",
        "--hljs-template-variable": "Template Variable",
        "--hljs-addition": "Addition",
        "--hljs-deletion": "Deletion"
      }
    }
  },
  methods: {
    updateColor(data){
      this.$emit('updateColor', data)
    }
  }
}
</script>
