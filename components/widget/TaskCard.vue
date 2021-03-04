<template>
  <div class="card-container">
    <div class="title-box">
      <div>Tasks</div>
      <div class="flex">
        <div class="relative">
          <img src="../../assets/image/Arrow.svg" alt="" class="select-arrow">
          <select name="card-dropdown" id="card-dropdown" class="card-dropdown">
            <option value="0">Sort</option>
            <option value="1">Other</option>
          </select>
        </div>
        <button class="plus-btn">+</button>
      </div>
    </div>
    <div class="card-content">
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_1.svg" alt=""></div>
        <div class="task-name flex items-center">Send prototype to team</div>
        <div class="task-date flex items-center">Today</div>
        <div class="flex items-center"><img src="../../assets/image/icon-attach-file.svg" alt=""></div>
        <div class="flex items-center"><img src="../../assets/image/Checked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_1.svg" alt=""></div>
        <div class="task-name flex items-center">Review content with copywriter</div>
        <div class="task-date flex items-center">Yesterday</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_1.svg" alt=""></div>
        <div class="task-name flex items-center">Add loading screen after sign up</div>
        <div class="task-date flex items-center">16 July</div>
        <div class="flex items-center"><img src="../../assets/image/icon-attach-file.svg" alt=""></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_1.svg" alt=""></div>
        <div class="task-name flex items-center">Get file structure ready for cms</div>
        <div class="task-date flex items-center">14 July</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Checked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Update style guide with new colors</div>
        <div class="task-date flex items-center">28 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Define grid for editor</div>
        <div class="task-date flex items-center">25 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Fix footer on mobile</div>
        <div class="task-date flex items-center">24 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Mobile navigation not working in ie</div>
        <div class="task-date flex items-center">24 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Mobile navigation not working in ie</div>
        <div class="task-date flex items-center">24 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
      <div class="task-row">
        <div class="flex items-center"><img src="../../assets/image/Checkbox_2.svg" alt=""></div>
        <div class="task-name1 flex items-center">Mobile navigation not working in ie</div>
        <div class="task-date flex items-center">24 June</div>
        <div class="flex items-center"></div>
        <div class="flex items-center"><img src="../../assets/image/Unchecked.svg" alt=""></div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "TaskCard"
    }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .card-container {
    @apply rounded-md w-full mb-4 overflow-hidden;
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
  .plus-btn {
    @apply flex justify-center items-center rounded-sm ml-2;
    background-color: #ECECEE;
    width: 32px;
    height: 32px;
  }
  .card-content {
    background-color: #FFFFFF;
  }
  .task-row {
    @apply grid p-4 border-b;
    grid-template-columns: 25px 2fr 1fr 45px 25px;
    grid-gap: 8px;
  }
  .task-name {
    color: #110F24;
    font-size: 16px;
  }
  .task-name1 {
    text-decoration: line-through;
    color: #110F24;
    font-size: 16px;
    color: rgba(17, 15, 36, 0.4);
  }
  .task-date {
    @apply pr-3;
    color: rgba(17, 15, 36, 0.4);
    font-size: 14px;
  }
  select {
    @apply pl-2;
    -moz-appearance: none;
    -webkit-appearance: none;
  }
  select::-ms-expand {
    display: none;
  }
  .select-arrow {
    @apply absolute;
    top: 7px;
    right: 3px;
  }

</style>
