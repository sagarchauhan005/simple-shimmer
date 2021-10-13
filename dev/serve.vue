<script>
import { defineComponent } from 'vue';
import SimpleShimmer from '@/simple-shimmer.vue';

export default defineComponent({
  name: 'ServeDev',
  components: {
    SimpleShimmer
  }
});
</script>

<template>
  <div id="app" style="margin: 50px;">

    <h3>Simple shimmer block</h3>
    <simple-shimmer :style="{height:'100px', borderRadius:'10px'}"/>

    <h3>Circular shimmer block</h3>
    <simple-shimmer :style="{height:'100px', width:'100px', borderRadius:'100%'}"/>

    <h3>Lines shimmer block</h3>
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>

  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nunito&display=swap');
#app{
  font-family: Nunito,serif;
}
</style>
