<template>
    <div id="change_color">
        <label for="r1">修改颜色</label>
        <input type="checkbox" v-model="use" id="r1">
        <div :class="{'class1': use}">
            v-bind:class 指令
        </div>
    </div>
</template>

<script>
export default {
    name: 'change_color',
    data () {
        return {
            use: false,
        }
    }

}
</script>

<style>
.class1 {
  background: #444;
  color: #eee;
}
</style>
