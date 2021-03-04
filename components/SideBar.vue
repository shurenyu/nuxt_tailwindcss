<template>
  <div class="side-bar">
<!--    Begin logo part-->
    <div class="px-2 py-2 flex items-center">
      <img src="../assets/image/Icon_0.svg" alt="">
      <div class="txt-16 font-semibold ml-2">Dashboard UI Kit 2.0</div>
    </div>
<!--    End logo part-->

<!--    Begin main menu group-->
    <div class="group-title">MAIN</div>
    <div :class="homeMenuClass" @click="handleClick(true)">
      <img src="../assets/image/Icon_1.svg" alt="">
      <div class="menu-name">Home</div>
    </div>
    <div class="menu-item">
      <img src="../assets/image/Icon_2.svg" alt="">
      <div class="menu-name">Activity</div>
    </div>
    <div class="menu-item">
      <img src="../assets/image/Icon_3.svg" alt="">
      <div class="menu-name">Projects</div>
    </div>
    <div class="menu-item">
      <img src="../assets/image/Icon_4.svg" alt="">
      <div class="menu-name">Tasks</div>
    </div>
<!--    End main menu group-->

<!--    Begin People menu group-->
    <div class="group-title">PEOPLE</div>
    <div class="menu-item">
      <img src="../assets/image/Icon_5.svg" alt="">
      <div class="menu-name">Customers</div>
    </div>
    <div :class="conversationClass" @click="handleClick(false)">
      <img src="../assets/image/Icon_6.svg" alt="">
      <div class="menu-name">Conversations</div>
    </div>
<!--    End people menu group-->

<!--    Begin Account menu group-->
    <div class="group-title">ACCOUNT</div>
    <div class="menu-item">
      <img src="../assets/image/Icon_7.svg" alt="">
      <div class="menu-name">Users</div>
    </div>
    <div class="menu-item">
      <img src="../assets/image/Icon_8.svg" alt="">
      <div class="menu-name">Settings</div>
    </div>
<!--    End Account menu group-->

<!--    Begin Misc menu group-->
    <div class="group-title">MISC</div>
    <div class="menu-item">
      <img src="../assets/image/Icon_9.svg" alt="">
      <div class="menu-name">Empty State</div>
    </div>
    <div class="menu-item">
      <img src="../assets/image/Icon_10.svg" alt="">
      <div class="menu-name">Onboarding</div>
    </div>
<!--    End Misc menu group-->
  </div>
</template>

<script>
  export default {
    name: "SideBar",
    data () {
      return {
        homeMenuClass: 'light-menu-item',
        conversationClass: 'menu-item',
      }
    },
    methods: {
      handleClick (value) {
        this.homeMenuClass = value ? 'light-menu-item' : 'menu-item';
        this.conversationClass = value ? 'menu-item' : 'light-menu-item';

        this.$emit('handleFlag', value);
      }
    }
  }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .side-bar {
    @apply min-h-screen w-1/6 text-white p-3 h-full;
    min-width: 240px;
    background-color: #211B4E;
  }
  .group-title {
    @apply font-bold pt-4 pb-1 px-3;
    color: #7a7695;
    font-size: 12px;
  }
  .menu-item {
    @apply px-3 py-2 flex items-center
  }
  .menu-item:hover {
    @apply rounded-sm;
    background-color: #373488;
  }
  .light-menu-item {
    @apply px-3 py-2 flex items-center rounded-sm;
    background-color: #373488;
  }
  .menu-name {
    @apply font-normal ml-2;
    font-size: 14px;
    color: rgba(255, 255, 255, 0.9);
  }
</style>
