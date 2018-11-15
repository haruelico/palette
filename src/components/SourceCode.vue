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
      code: `console.log('hello world')
// hogehoge
import Vue from './instance/index'
import { initGlobalAPI } from './global-api/index'
import { isServerRendering } from 'core/util/env'
import { FunctionalRenderContext } from 'core/vdom/create-functional-component'

initGlobalAPI(Vue)

Object.defineProperty(Vue.prototype, '$isServer', {
  get: isServerRendering
})`,
      color: "#ff0000",
      style: {
        "--background-color": "#002b36"
      }
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
