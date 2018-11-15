<template>
  <div id="app" :style="style">
    <SourceCode language="javascript"/>
    <Color v-on:update-style="updateStyle"/>
  </div>
</template>

<script>
import SourceCode from "./components/SourceCode.vue";
import Color from "./components/Color.vue";

export default {
  name: "app",
  components: {
    SourceCode,
    Color
  },
  data: function() {
    return {
      style: {
        "--hljs-keyword": "#eee",
        "--hljs-built_in": "#eee",
        "--hljs-type": "#eee",
        "--hljs-literal": "#eee",
        "--hljs-number": "#eee",
        "--hljs-regexp": "#eee",
        "--hljs-sring": "#eee",
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
        "--hljs-deletion": "#eee",
        "--hljs-background-color": "#fff"
      }
    };
  },
  methods: {
    updateStyle: function(updatedStyle) {
      this.style = updatedStyle;
    }
  }
};
</script>

<style>
#app {
  font-family: "monospace";
  display: flex;
}

#source-code {
  flex-grow: 3;
  margin-right: 20px;
}

#color {
  flex-grow: 1;
}

.hljs-keyword {
  color: var(--hljs-keyword);
}
.hljs-built_in {
  color: var(--hljs-built_in);
}
.hljs-type {
  color: var(--hljs-type);
}
.hljs-literal {
  color: var(--hljs-literal);
}
.hljs-number {
  color: var(--hljs-number);
}
.hljs-regexp {
  color: var(--hljs-regexp);
}
.hljs-string {
  color: var(--hljs-string);
}
.hljs-subst {
  color: var(--hljs-subst);
}
.hljs-symbol {
  color: var(--hljs-symbol);
}
.hljs-class {
  color: var(--hljs-class);
}
.hljs-function {
  color: var(--hljs-function);
}
.hljs-title {
  color: var(--hljs-title);
}
.hljs-params {
  color: var(--hljs-params);
}
.hljs-comment {
  color: var(--hljs-comment);
}
.hljs-doctag {
  color: var(--hljs-doctag);
}
.hljs-meta {
  color: var(--hljs-meta);
}
.hljs-meta-keyword {
  color: var(--hljs-meta-keyword);
}
.hljs-meta-string {
  color: var(--hljs-meta-string);
}
.hljs-section {
  color: var(--hljs-section);
}
.hljs-tag {
  color: var(--hljs-tag);
}
.hljs-name {
  color: var(--hljs-name);
}
.hljs-builtin-name {
  color: var(--hljs-builtin-name);
}
.hljs-attr {
  color: var(--hljs-attr);
}
.hljs-attribute {
  color: var(--hljs-attribute);
}
.hljs-variable {
  color: var(--hljs--variable);
}
.hljs-bullet {
  color: var(--hljs-bullet);
}
.hljs-code {
  color: var(--hljs-code);
}
.hljs-emphasis {
  font-style: italic;
}
.hljs-strong {
  font-weight: bold;
}
.hljs-formula {
  color: var(--hljs-formula);
}
.hljs-link {
  color: var(--hljs-link);
}
.hljs-quote {
  color: var(--hljs-quote);
}
.hljs-selector-tag {
  color: var(--hljs-selector-tag);
}
.hljs-selector-id {
  color: var(--hljs-selector-id);
}
.hljs-selector-class {
  color: var(--hljs-selector-class);
}
.hljs-selector-attr {
  color: var(--hljs-selector-attr);
}
.hljs-selector-pseudo {
  color: var(--hljs-pseudo);
}
.hljs-template-tag {
  color: var(--hljs-template-tag);
}
.hljs-template-variable {
  color: var(--hljs-template-variable);
}
.hljs-addition {
  color: var(--hljs-addition);
}
.hljs-deletion {
  color: var(--hljs-deletion);
}
.hljs {
  display: block;
  overflow-x: auto;
  padding: 0.5em;
  background-color: var(--hljs-background-color);
}
</style>
