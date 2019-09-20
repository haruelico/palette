<template>
  <div
    id="app"
  >
    <SourceCode
      class="source-code"
      language="javascript"
      :style="codeStyle"
    />
    <Color
      class="color"
      :code-style="codeStyle"
      @updateColor="updateColor"
    />
  </div>
</template>

<script>
import SourceCode from "./components/SourceCode.vue";
import Color from "./components/Color.vue";

export default {
  name: "App",
  components: {
    SourceCode,
    Color
  },
  data: function() {
    return {
      codeStyle: {
        "--hljs-background-color": "#fff",
        "--hljs-keyword": "#eee",
        "--hljs-built_in": "#eee",
        "--hljs-type": "#eee",
        "--hljs-literal": "#eee",
        "--hljs-number": "#eee",
        "--hljs-regexp": "#eee",
        "--hljs-string": "#eee",
        "--hljs-subst": "#eee",
        "--hljs-symbol": "#eee",
        "--hljs-class": "#eee",
        "--hljs-function": "#eee",
        "--hljs-title": "#eee",
        "--hljs-params": "#eee",
        "--hljs-comment": "#eee",
        "--hljs-doctag": "#eee",
        "--hljs-meta": "#eee",
        "--hljs-meta-keyword": "#eee",
        "--hljs-meta-string": "#eee",
        "--hljs-section": "#eee",
        "--hljs-tag": "#eee",
        "--hljs-name": "#eee",
        "--hljs-builtin-name": "#eee",
        "--hljs-attr": "#eee",
        "--hljs-attribute": "#eee",
        "--hljs-variable": "#eee",
        "--hljs-bullet": "#eee",
        "--hljs-code": "#eee",
        "--hljs-emphasis": "#eee",
        "--hljs-strong": "#eee",
        "--hljs-formula": "#eee",
        "--hljs-link": "#eee",
        "--hljs-quote": "#eee",
        "--hljs-selector-tag": "#eee",
        "--hljs-selector-id": "#eee",
        "--hljs-selector-class": "#eee",
        "--hljs-selector-attr": "#eee",
        "--hljs-selector-pseudo": "#eee",
        "--hljs-template-tag": "#eee",
        "--hljs-template-variable": "#eee",
        "--hljs-addition": "#eee",
        "--hljs-deletion": "#eee"
      }
    };
  },
  methods: {
    updateColor(data) {
      this.codeStyle[data.key] = data.color;
    }
  }
};
</script>

<style scoped>
#app {
  font-family: "monospace";
  display: flex;
}

.source-code {
  flex-grow: 3;
  margin-right: 20px;
}

.color {
  flex-grow: 1;
}
</style>
