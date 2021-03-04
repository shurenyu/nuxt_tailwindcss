<template>
  <div class="card-container">
    <div class="title-box">
      <div>Projects</div>
      <div>
        <button class="plus-btn">+</button>
      </div>
    </div>
    <div class="card-content">
      <div class="project-item">
        <div>
          <div>Flowychart Editor</div>
          <div class="sub-title">Enigm</div>
        </div>
        <div class="flex items-center">
          <div class="status-box"><div class="status-bar1"></div></div>
        </div>
      </div>
      <div class="project-item">
        <div>
          <div>Flowychart Editor</div>
          <div class="sub-title">Giddifi</div>
        </div>
        <div class="flex items-center">
          <div class="status-box"><div class="status-bar2"></div></div>
        </div>
      </div>
      <div class="project-item">
        <div>
          <div>Flowychart Editor</div>
          <div class="sub-title">Mondemi</div>
        </div>
        <div class="flex items-center">
          <div class="status-box"><div class="status-bar3"></div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "ProjectCard"
  }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .card-container {
    @apply rounded-md w-full mb-4 overflow-hidden;
    background-color: #ffffff;
    box-shadow: 1px 2px 6px 2px #e2e2e2;
  }
  .title-box {
    @apply flex items-center px-4 font-bold border-b justify-between;
    color: #110F24;
    background-color: #F6F6F9;
    font-size: 16px;
    height: 56px;
  }
  .card-dropdown {
    width: 120px;
    height: 32px;
    border-radius: 3px;
    border: 1px solid #ECECEE;
  }
  .card-content {
    background-color: #FFFFFF;
  }
  .plus-btn {
    @apply flex justify-center items-center rounded-sm ml-2;
    background-color: #ECECEE;
    width: 32px;
    height: 32px;
  }
  .project-item {
    @apply p-4 border-b grid;
    grid-template-columns: 140px auto;
  }
  .sub-title {
    color: rgba(17, 15, 36, 0.4);
    font-size: 14px;
  }
  .status-box {
    /*@apply relative rounded-sm;*/
    @apply rounded-sm w-full ml-2;
    height: 4px;
    background-color: #ECECEE;
  }
  .status-bar1 {
    /*@apply absolute*/
    height: 4px;
    width: 40%;
    background-color: #FFBF2F;
  }
  .status-bar2 {
    /*@apply absolute*/
    height: 4px;
    width: 21%;
    background-color: #E52B20;
  }
  .status-bar3 {
    /*@apply absolute*/
    height: 4px;
    width: 66%;
    background-color: #63CE63;
  }
</style>
