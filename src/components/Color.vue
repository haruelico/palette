<template>
  <div id="color" :style="colorCodes">
    <color-input v-model="colorCodes['--hljs-background-color']" label="Background color"/>
    <color-input v-model="colorCodes['--hljs-keyword']" label="Keyword"/>
    <color-input v-model="colorCodes['--hljs-built_in']" label="Built_in"/>
    <color-input v-model="colorCodes['--hljs-type']" label="Type"/>
    <color-input v-model="colorCodes['--hljs-literal']" label="Literal"/>
    <color-input v-model="colorCodes['--hljs-number']" label="Number"/>
    <color-input v-model="colorCodes['--hljs-regexp']" label="Regexp"/>
    <color-input v-model="colorCodes['--hljs-string']" label="String"/>
    <color-input v-model="colorCodes['--hljs-subst']" label="Subst"/>
    <color-input v-model="colorCodes['--hljs-symbol']" label="Symbol"/>
    <color-input v-model="colorCodes['--hljs-class']" label="Class"/>
    <color-input v-model="colorCodes['--hljs-function']" label="Function"/>
    <color-input v-model="colorCodes['--hljs-title']" label="Title"/>
    <color-input v-model="colorCodes['--hljs-params']" label="Params"/>
    <color-input v-model="colorCodes['--hljs-comment']" label="Comment"/>
    <color-input v-model="colorCodes['--hljs-doctag']" label="Doctag"/>
    <color-input v-model="colorCodes['--hljs-meta']" label="Meta"/>
    <color-input v-model="colorCodes['--hljs-meta-keyword']" label="Meta keyword"/>
    <color-input v-model="colorCodes['--hljs-meta-string']" label="Meta string"/>
    <color-input v-model="colorCodes['--hljs-section']" label="Section"/>
    <color-input v-model="colorCodes['--hljs-tag']" label="Tag"/>
    <color-input v-model="colorCodes['--hljs-name']" label="Name"/>
    <color-input v-model="colorCodes['--hljs-builtin-name']" label="Builtin name"/>
    <color-input v-model="colorCodes['--hljs-attr']" label="Attr"/>
    <color-input v-model="colorCodes['--hljs-attribute']" label="Attribute"/>
    <color-input v-model="colorCodes['--hljs-variable']" label="Variable"/>
    <color-input v-model="colorCodes['--hljs-bullet']" label="Bullet"/>
    <color-input v-model="colorCodes['--hljs-code']" label="Code"/>
    <color-input v-model="colorCodes['--hljs-emphasis']" label="Emphasis"/>
    <color-input v-model="colorCodes['--hljs-strong']" label="Strong"/>
    <color-input v-model="colorCodes['--hljs-formula']" label="Formula"/>
    <color-input v-model="colorCodes['--hljs-link']" label="Link"/>
    <color-input v-model="colorCodes['--hljs-quote']" label="Quote"/>
    <color-input v-model="colorCodes['--hljs-selector-tag']" label="Selector tag"/>
    <color-input v-model="colorCodes['--hljs-selector-id']" label="Selector id"/>
    <color-input v-model="colorCodes['--hljs-selector-class']" label="Selector class"/>
    <color-input v-model="colorCodes['--hljs-selector-attr']" label="Selector attr"/>
    <color-input v-model="colorCodes['--hljs-selector-pseudo']" label="Selector pseudo"/>
    <color-input v-model="colorCodes['--hljs-template-tag']" label="Template tag"/>
    <color-input v-model="colorCodes['--hljs-template-variable']" label="Template variable"/>
    <color-input v-model="colorCodes['--hljs-addition']" label="Addition"/>
    <color-input v-model="colorCodes['--hljs-deletion']" label="Deletion"/>
  </div>
</template>

<script>
import ColorInput from "./ColorInput";
export default {
  name: "Color",
  components: {
    ColorInput
  },
  props: {
    colorCodes: {
      type: Object,
      required: true
    }
  }
};
</script>
