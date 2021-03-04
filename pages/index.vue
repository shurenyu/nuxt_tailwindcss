<template>
  <div class="wrapper">
    <div class="side-wrapper">
      <SideBar v-on:handleFlag="handleFlag"/>
    </div>
    <div class="header-wrapper">
      <HeaderBar/>
    </div>
    <div v-if="flag" class="home-wrapper w-full">
      <Home/>
    </div>
    <div v-if="!flag" class="conversation-wrapper w-full">
      <Conversation/>
    </div>
  </div>
</template>

<script>
  import SideBar from "../components/SideBar";
  import Home from "../components/Home";

  export default {
    components: {
      SideBar,
      Home,
    },
    data () {
      return {
        flag: true,
      }
    },
    methods: {
      handleFlag (value) {
        this.flag = value;
      },
     }
  }
</script>

<style>
  * {
    font-family: 'Lato', sans-serif;
  }
  .wrapper {
    @apply min-h-screen flex;
  }
  .side-wrapper {
    @apply block;
  }
  .header-wrapper {
    @apply hidden;
  }

  @media only screen and (max-width: 992px) {
    .wrapper {
      @apply flex-col;
    }
    .side-wrapper {
      @apply hidden;
    }
    .header-wrapper {
      @apply block;
    }
  }
</style>
