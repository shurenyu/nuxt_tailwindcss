<template>
  <div class="main-container">
    <div>
      <ChatCard title="This Month" :chatData="chatData"/>
    </div>
    <div class="bottom-wrapper">
        <TaskCard/>
        <ProjectCard/>
    </div>
  </div>
</template>

<script>
  import ChatCard from "./widget/ChatCard";
  import TaskCard from "./widget/TaskCard";
  import ProjectCard from "./widget/ProjectCard";

  export default {
    name: "Home",
    components: {
      ChatCard,
      TaskCard,
      ProjectCard,
    },
    data () {
      return {
        chatData: [
          {month: 'Jan', value: 30},
          {month: 'Feb', value: 15},
          {month: 'Mar', value: 45},
          {month: 'Apr', value: 60},
          {month: 'May', value: 45},
          {month: 'Jun', value: 105},
          {month: 'Jul', value: 150},
          {month: 'Aug', value: 90},
          {month: 'Sep', value: 75},
          {month: 'Oct', value: 105},
          {month: 'Nov', value: 135},
          {month: 'Dec', value: 90},
        ],
      }
    }
  }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .main-container {
    @apply min-h-screen w-full px-4 pt-16;
    background-color: #F2F2F2;
  }
  .bottom-wrapper {
    @apply grid;
    grid-template-columns: 2fr 1fr;
    grid-gap: 16px;
  }

  @media only screen and (max-width: 992px) {
    .bottom-wrapper {
      grid-template-columns: 1fr;
    }
  }
</style>
