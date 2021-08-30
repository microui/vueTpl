<template>
  <div>
    <hello-world></hello-world>
  </div>
</template>

<script>
import Ajax from '@/assets/js/api/ajax.js';
import HelloWorld from '@/components/HelloWorld';

export default {
  name: 'Home',
  data () {
    return {};
  },
  components: {
    HelloWorld
  },
  mounted () {
    Ajax(`/tui/commission`, {
      'id': 222
    }).then(res => {
      console.log(res);
      console.log('1111111111');
      console.log('222222');
    });
  }
};
</script>

<style>

</style>
