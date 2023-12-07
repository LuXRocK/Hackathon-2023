<template>
    <header class="header">
        <img src="../assets/userProfile.svg" alt="User profile logo" class="header__logo">
        <h1 class="header__title">TimeOut</h1>
    </header>
</template>
  
<script>
  
export default {
  name: 'MainHeader',
  props: {
  }
}
</script>
  
<style lang="scss">
    .header{
        padding: 5%;
        display: grid;
        grid-template-columns: 20% 60% 20%;
        grid-template-areas: 
        "logo title ."
        ;

        &__logo{
            grid-area: logo;
            justify-self: center;
            align-self: center;
            width: 80%;
        }

        &__title{
            grid-area: title;
            justify-self: center;
            align-self: center;
        }
    }   
</style>
  