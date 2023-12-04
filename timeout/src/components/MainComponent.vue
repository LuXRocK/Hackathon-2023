<template>
    <MainHeader/>
    <SwitchWorkLife/>
</template>
  
<script>
import MainHeader from './MainHeader.vue'
import SwitchWorkLife from './SwitchWorkLife.vue';

export default {
  name: 'MainContent',
  props: {},
  components: {
    MainHeader,
    SwitchWorkLife
}
}

</script>
  
<style>
</style>
  