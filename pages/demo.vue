<template>
  <div>
    <p>我是demo1页面</p>
    <Hello />
    <Vbind />
  </div>
</template>

<script>
import Hello from '../components/Hello';
import Vbind from '../components/Vbind';

export default {
  name: 'demo',
  components: {
    Hello,
    Vbind,
  }
}
</script>
