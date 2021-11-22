<script>
import Vue from 'vue';
import SimpleShimmer from '@/simple-shimmer.vue';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    SimpleShimmer
  }
});
</script>

<template>
  <div id="app">
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>
    <simple-shimmer :style="{height:'100px', width:'100px', borderRadius:'100%'}"/>
  </div>
</template>
