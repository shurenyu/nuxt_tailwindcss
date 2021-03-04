<template>
  <div class="card-container">
    <div class="title-box">
      <div>{{title}}</div>
      <div class="relative">
        <img src="../../assets/image/Arrow.svg" alt="" class="select-arrow">
        <select name="card-dropdown" id="card-dropdown" class="card-dropdown">
          <option value="0">Sales</option>
          <option value="1">Other</option>
        </select>
      </div>
    </div>
    <div class="chat-wrapper">
      <div class="chat-box">
        <div class="first-chat-part">
          <div class="chat-item">
            <div class="chat-bar h-1"/>
            <div class="month">Jan</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-2"/>
            <div class="month">Feb</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-3"/>
            <div class="month">Mar</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-4"/>
            <div class="month">Apr</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-5"/>
            <div class="month">May</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-6"/>
            <div class="month">Jun</div>
          </div>
        </div>
        <div class="second-chat-part">
          <div class="chat-item">
            <div class="chat-bar h-7"/>
            <div class="month">Jul</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-8"/>
            <div class="month">Aug</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-9"/>
            <div class="month">Sep</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-10"/>
            <div class="month">Oct</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-11"/>
            <div class="month">Nov</div>
          </div>
          <div class="chat-item">
            <div class="chat-bar h-12"/>
            <div class="month">Dec</div>
          </div>
        </div>
        <div class="h-line1"/>
        <div class="h-line2"/>
        <div class="h-line3"/>
        <div class="h-line4"/>
        <div class="h-line5"/>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "ChatCard",
    props: {
      title: String,
      chatData: Object,
    }
  }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .card-container {
    @apply rounded-md w-full mb-4 overflow-hidden;
    height: 264px;
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
  .chat-wrapper {
    @apply px-4 py-3;
    height: 208px;
    background-color: #FFFFFF;
  }
  .chat-box {
    @apply h-full grid grid-cols-2 relative;
  }
  .first-chat-part, .second-chat-part {
    @apply h-full grid grid-cols-6 relative;
  }
  .h-line1 {
    @apply w-full absolute border-b;
    top: 0;
    left: 0;
    height: 0;
  }
  .h-line2 {
    @apply w-full absolute border-b;
    top: 40px;
    left: 0;
    height: 0;
  }
  .h-line3 {
    @apply w-full absolute border-b;
    top: 80px;
    left: 0;
    height: 0;
  }
  .h-line4 {
    @apply w-full absolute border-b;
    top: 121px;
    left: 0;
    height: 0;
  }
  .h-line5 {
    @apply w-full absolute border-b;
    top: 163px;
    left: 0;
    height: 0;
  }
  .chat-item {
    @apply flex flex-col justify-end px-2 z-50;
  }
  .chat-bar {
    background-color: #575BDE;
    border-radius: 3px 3px 0 0;
  }
  .h-1 {
    height: 30px;
  }
  .h-2 {
    height: 15px;
  }
  .h-3 {
    height: 45px;
  }
  .h-4 {
    height: 60px;
  }
  .h-5 {
    height: 45px;
  }
  .h-6 {
    height: 105px;
  }
  .h-7 {
    height: 150px;
  }
  .h-8 {
    height: 90px;
  }
  .h-9 {
    height: 75px;
  }
  .h-10 {
    height: 105px;
  }
  .h-11 {
    height: 135px;
  }
  .h-12 {
    height: 90px;
  }
  .month {
    @apply flex justify-center items-center;
    height: 20px;
    font-size: 12px;
    color: rgba(17, 15, 36, 0.4);
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
  @media only screen and (max-width: 992px) {
    .chat-box {
      @apply h-full grid grid-cols-1 relative;
    }
    .first-chat-part {
      @apply hidden;
    }
  }
</style>
