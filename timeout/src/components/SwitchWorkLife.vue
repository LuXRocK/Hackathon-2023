<template>
    <section class="switch">
        <button class="switch__work">Work</button>
        <button class="switch__life">Life</button>
    </section>
</template>
  
<script>
  
export default {
  name: 'SwitchWorkLife',
  props: {
  }
}
</script>
  
<style lang="scss">
    .switch{
        padding: 20% 0 10% 0;
        &__work, &__life{
            width: 20%;
            height: 5vh;
        }
    }

</style>
  