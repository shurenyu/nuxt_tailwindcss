<template>
    <div class="header-container">
      <div class="flex items-center">
        <img src="../assets/image/Icon_0.svg" alt="">
        <div class="txt-16 font-semibold ml-2">Dashboard UI Kit 2.0</div>
      </div>
      <div>
        <img src="../assets/image/Menu.svg" alt="">
      </div>
    </div>
</template>

<script>
    export default {
        name: "HeaderBar"
    }
</script>

<style scoped>
  .header-container {
    @apply px-4 py-3 flex justify-between items-center text-white;
    background-color: #211B4E;
    height: 56px;
  }
</style>
