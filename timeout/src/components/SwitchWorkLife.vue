<template>
    <section class="switch">
        <button class="switch__work" :class="{ 'active': activeButton }" @click="classSwap('work')">Work</button>
        <button class="switch__life" :class="{ 'active': !activeButton }" @click="classSwap('life')">Life</button>
    </section>
</template>
  
<script>
  
export default {
  name: 'SwitchWorkLife',
  data() {
    return {
        activeButton: true,
        buttonWork: true,
        buttonLife: false,
        };
    },
    methods: {
        classSwap(button) {
            if ((button == 'work' && this.buttonWork) || (button == 'life' && this.buttonLife)) {
                return;
            }

            this.activeButton = !this.activeButton;
            this.buttonWork = button === 'work';
            this.buttonLife = button === 'life';
        },
    },
}

</script>
  
<style lang="scss">
    .switch{
        padding: 20% 0 10% 0;
        &__work, &__life{
            width: 20%;
            height: 5vh;
            border: none;
            color: rgb(71, 71, 71);
            background-color: #212121;
        }        

        &__life{
            border-radius: 0px 5px 5px 0px;
        }

        &__work{
            border-radius: 5px 0px 0px 5px;
        }
    }

    .active{
        background-color: #1ED760;
        transition: 0.3s linear;
    }
</style>
  