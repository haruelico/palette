<template>
  <div id="source-code">
    <pre v-highlightjs="code"><code v-bind:class="language"></code></pre>
    <textarea rows="20" v-model="code"></textarea>
  </div>
</template>

<script>
export default {
  name: "SourceCode",
  props: {
    language: String
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

<style>
textarea {
  width: 100%;
}

pre {
  text-align: left;
  font-size: 1.4em;
}
</style>
