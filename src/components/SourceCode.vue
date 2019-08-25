<template>
  <div id="source-code">
    <pre
      v-highlightjs="code"
    >
      <code :class="language" />
    </pre>
    <textarea
      v-model="code"
      rows="20"
    />
  </div>
</template>

<script>
export default {
  name: "SourceCode",
  props: {
    language:{
      type: String,
      required: true
    }
  },
  data: function() {
    return {
      code: `import Foo from 'bar'

// sample class definition
class Sample {
  constructor(arg) {
    this.greet = \`Hello $\{arg}!\`;
    this.counter = 0;
    this.pattern = /\\w+/;
  }

  greet(argument) {
    console.log(this.greet);
  }
}
`
    };
  }
};
</script>

<style scoped>
textarea {
  width: 100%;
}

pre {
  text-align: left;
  font-size: 1.4em;
}
</style>

<style>
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

</style>