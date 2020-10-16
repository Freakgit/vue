<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>你要不要点一点这里<a href="http://www.baidu.com" target="_blank" rel="noopener">地址</a>.
    </p>
    <h3>第一页</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">首页</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">我的</a></li>
    </ul>
    <h3>第二页</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">大是大非</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">汞基甲酚</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">的规范化</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">观复嘟嘟</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">创始人发</a></li>
    </ul>
    <h3>第三页</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">你好</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">你好1</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">你好2</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">你好3</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">你好4</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
