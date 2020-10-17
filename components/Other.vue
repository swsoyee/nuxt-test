<template>
  <div>
      <label>显示文本</label>
      <input type="checkbox" v-model='seen'>
      <p v-if="seen">你看到我了</p>
      <p v-show="!seen">我隐藏起来了</p>
  </div>
</template>

<script>
export default {
    data () {
        return {
            seen: true,
        }
    }
}
</script>
