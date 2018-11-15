<template>
  <div id="color" :style="style">
    <div class='input'>
      <input type="color" id="hljs-background-color" v-model="hljs.background_color">
      <label for="hljs-background-color">Background color {{ hljs.background_color }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-keyword" v-model="hljs.keyword">
      <label for="hljs-keyword">Keyword {{ hljs.keyword }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-built_in" v-model="hljs.built_in">
      <label for="hljs-built_in">Built_in {{ hljs.built_in }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-type" v-model="hljs.type">
      <label for="hljs-type">Type {{ hljs.type }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-literal" v-model="hljs.literal">
      <label for="hljs-literal">Literal {{ hljs.literal }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-number" v-model="hljs.number">
      <label for="hljs-number">Number {{ hljs.number }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-regexp" v-model="hljs.regexp">
      <label for="hljs-regexp">Regexp {{ hljs.regexp }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-sring" v-model="hljs.string">
      <label for="hljs-string">String {{ hljs.string }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-subst" v-model="hljs.subst">
      <label for="hljs-subst">Subst {{ hljs.subst }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-symbol" v-model="hljs.symbol">
      <label for="hljs-symbol">Symbol {{ hljs.symbol }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-class" v-model="hljs.class">
      <label for="hljs-class">Class {{ hljs.class }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-function" v-model="hljs.function">
      <label for="hljs-function">Function {{ hljs.function }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-title" v-model="hljs.title">
      <label for="hljs-title">Title {{ hljs.title }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-params" v-model="hljs.params">
      <label for="hljs-params">Params {{ hljs.params }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-comment-" v-model="hljs.comment">
      <label for="hljs-comment">Comment {{ hljs.comment }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-doctag" v-model="hljs.doctag">
      <label for="hljs-doctag">Doctag {{ hljs.doctag }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-meta" v-model="hljs.meta">
      <label for="hljs-meta">Meta {{ hljs.meta }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-meta-keyword" v-model="hljs.meta_keyword">
      <label for="hljs-meta-keyword">Meta keyword {{ hljs.meta_keyword }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-meta-string" v-model="hljs.meta_string">
      <label for="hljs-meta-string">Meta string {{ hljs.meta_string }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-section" v-model="hljs.section">
      <label for="hljs-section">Section {{ hljs.section }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-tag" v-model="hljs.tag">
      <label for="hljs-tag">Tag {{ hljs.tag }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-name" v-model="hljs.name">
      <label for="hljs-name">Name {{ hljs.name }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-builtin-name" v-model="hljs.builtin_name">
      <label for="hljs-builtin-name">Builtin name {{ hljs.builtin_name }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-attr" v-model="hljs.attr">
      <label for="hljs-attr">Attr {{ hljs.attr }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-attribute" v-model="hljs.attribute">
      <label for="hljs-attribute">Attribute {{ hljs.attribute }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-variable" v-model="hljs.variable">
      <label for="hljs-variable">Variable {{ hljs.variable }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-bullet" v-model="hljs.bullet">
      <label for="hljs-bullet">Bullet {{ hljs.bullet }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-code" v-model="hljs.code">
      <label for="hljs-code">Code {{ hljs.code }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-emphasis" v-model="hljs.emphasis">
      <label for="hljs-emphasis">Emphasis {{ hljs.emphasis }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-strong" v-model="hljs.strong">
      <label for="hljs-strong">Strong {{ hljs.strong }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-formula" v-model="hljs.formula">
      <label for="hljs-formula">Formula {{ hljs.formula }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-link" v-model="hljs.link">
      <label for="hljs-link">Link {{ hljs.link }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-quote" v-model="hljs.quote">
      <label for="hljs-quote">Quote {{ hljs.quote }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-selector-tag" v-model="hljs.selector_tag">
      <label for="hljs-selector-tag=">Selector tag {{ hljs.selector_tag }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-selector-id" v-model="hljs.selector_id">
      <label for="hljs-selector-id">Selector id {{ hljs.selector_id }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-selector-class" v-model="hljs.selector_class">
      <label for="hljs-selector-class">Selector class {{ hljs.selector_class }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-selector-attr" v-model="hljs.selector_attr">
      <label for="hljs-selector-attr">Selector attr {{ hljs.selector_attr }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-selector-pseudo" v-model="hljs.selector_pseudo">
      <label for="hljs-selector-pseudo">Selector pseudo {{ hljs.selector_pseudo }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-template-tag" v-model="hljs.template_tag">
      <label for="hljs-template-tag">Template tag {{ hljs.template_tag }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-template-variable" v-model="hljs.template_variable">
      <label for="hljs-template-variable">Template variable {{ hljs.template_variable }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-addition" v-model="hljs.addition">
      <label for="hljs-addition">Addition {{ hljs.addition }}</label>
    </div>
    <div class='input'>
      <input type="color" id="hljs-deletion" v-model="hljs.deletion">
      <label for="hljs-deletion">Deletion {{ hljs.deletion }}</label>
    </div>
  </div>
</template>

<style>
input[type="color"] {
  margin-right: 10px;
}

.input {
  margin-bottom: 5px;
}
</style>


<script>
export default {
  name: "Color",
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
      },
      hljs: {}
    };
  },
  watch: {
    hljs: {
      handler: function() {
        this.style["--hljs-keyword"] = this.hljs.keyword;
        this.style["--hljs-built_in"] = this.hljs.built_in;
        this.style["--hljs-type"] = this.hljs.type;
        this.style["--hljs-literal"] = this.hljs.literal;
        this.style["--hljs-number"] = this.hljs.number;
        this.style["--hljs-regexp"] = this.hljs.regexp;
        this.style["--hljs-string"] = this.hljs.string;
        this.style["--hljs-subst"] = this.hljs.subst;
        this.style["--hljs-symbol"] = this.hljs.symbol;
        this.style["--hljs-class"] = this.hljs.class;
        this.style["--hljs-function"] = this.hljs.function;
        this.style["--hljs-title"] = this.hljs.title;
        this.style["--hljs-params"] = this.hljs.params;
        this.style["--hljs-comment"] = this.hljs.comment;
        this.style["--hljs-doctag"] = this.hljs.doctag;
        this.style["--hljs-meta"] = this.hljs.meta;
        this.style["--hljs-meta-keyword"] = this.hljs.meta_keyword;
        this.style["--hljs-meta-string"] = this.hljs.meta_string;
        this.style["--hljs-section"] = this.hljs.section;
        this.style["--hljs-tag"] = this.hljs.tag;
        this.style["--hljs-name"] = this.hljs.name;
        this.style["--hljs-builtin_name"] = this.hljs.builtin_name;
        this.style["--hljs-attr"] = this.hljs.attr;
        this.style["--hljs-attribute"] = this.hljs.attribute;
        this.style["--hljs-variable"] = this.hljs.variable;
        this.style["--hljs-bullet"] = this.hljs.bullet;
        this.style["--hljs-code"] = this.hljs.code;
        this.style["--hljs-emphasis"] = this.hljs.emphasis;
        this.style["--hljs-strong"] = this.hljs.strong;
        this.style["--hljs-formula"] = this.hljs.formula;
        this.style["--hljs-link"] = this.hljs.link;
        this.style["--hljs-quote"] = this.hljs.quote;
        this.style["--hljs-selector-tag"] = this.hljs.selector_tag;
        this.style["--hljs-selector-id"] = this.hljs.selector_id;
        this.style["--hljs-selector-class"] = this.hljs.selector_class;
        this.style["--hljs-selector-attr"] = this.hljs.selector_attr;
        this.style["--hljs-selector-pseudo"] = this.hljs.selector_pseudo;
        this.style["--hljs-template-tag"] = this.hljs.template_tag;
        this.style["--hljs-template-variable"] = this.hljs.template_variable;
        this.style["--hljs-addition"] = this.hljs.addition;
        this.style["--hljs-deletion"] = this.hljs.deletion;
        this.style["--hljs-background-color"] = this.hljs.background_color;
        this.$emit("update-style", this.style);
      },
      deep: true
    }
  }
};
</script>
