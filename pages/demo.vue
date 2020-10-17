<template>
  <div>
    <p>我是demo1页面</p>
    <Hello />
    <Vbind />
    <Other />
  </div>
</template>

<script>
import Hello from '../components/Hello';
import Vbind from '../components/Vbind';
import Other from '../components/Other';

export default {
  name: 'demo',
  components: {
    Hello,
    Vbind,
    Other,
  }
}
</script>
