<template>
  <div>
      <hr>
      <label>显示文本</label>
      <input type="checkbox" v-model='seen'>
      <p v-if="seen">你看到我了</p>
      <p v-show="!seen">我隐藏起来了</p>
      <br>
      <label>动态更换链接</label>
      <input type="checkbox" v-model='isBaidu'>
      <p>
        <a :href="isBaidu ? 'https://www.baidu.com' : 'https://www.google.com'">搜索引擎：{{ isBaidu ? '百度' : '谷歌' }}</a>
      </p>
      <p>{{ message }}</p>
      <button @click="reverseMessage">反转字符串</button>
      <hr>
  </div>
</template>

<script>
export default {
    data () {
        return {
            seen: true,
            isBaidu: true,
            message: '第一次学习Vue.js',
        }
    },
    methods: {
        reverseMessage: function () {
            this.message = this.message.split('').reverse().join('');
        }
    }
}
</script>
