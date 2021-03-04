<template>
  <div class="main-container">
<!--    Top part on mobile -->
    <div class="mobile-top-part">
      <div>
        <div class="message-box p-4 border-t">
          <div class="relative">
            <img src="../assets/image/Icon_search.svg" alt="" class="search absolute">
            <input type="text" placeholder="Search..." class="search-box">
          </div>
          <div class="flex items-center justify-center">
            <img src="../assets/image/Icon_book.svg" alt="">
          </div>
          <div class="flex items-center justify-center">
            <img src="../assets/image/Icon_notice.svg" alt="">
          </div>
        </div>
      </div>
      <div class="px-4 pb-4">
        <div class="chat-list">
          <div class="p-4 flex justify-between items-center">
            <div class="flex items-center">
              <img src="../assets/image/Profile03.png" alt="">
              <div class="user-list">Camilla Tunney</div>
            </div>
            <img src="../assets/image/Icon-arrow.svg" alt="">
          </div>
        </div>
      </div>
    </div>
<!--    Uer list-->
    <div class="history-wrapper">
      <div class="p-3">
        <div class="menu-item">
          <img src="../assets/image/Profile03.png" alt="">
          <div class="menu-name">Camilla Tunney</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile04.svg" alt="">
          <div class="menu-name">Alise Stoke</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile05.svg" alt="">
          <div class="menu-name">Kristopher Fager</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile06.svg" alt="">
          <div class="menu-name">Winston L., Camilla T...</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile07.svg" alt="">
          <div class="menu-name">Laureen Deangelis</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile03.png" alt="">
          <div class="menu-name">Winston Lanni</div>
        </div>
        <div class="menu-item">
          <img src="../assets/image/Profile04.svg" alt="">
          <div class="menu-name">Manuel Kriz</div>
        </div>
      </div>
      <div class="button-wrapper">
        <button class="new-conv-btn rounded-sm">
          New Conversation
        </button>
        <img src="../assets/image/icon-tune.svg" alt="">
      </div>
    </div>
    <div class="chat-wrapper">
<!--      Chatting history-->
      <div class="chat-box">
        <div class="new-section">
          <div class="chat-subtitle p-4 extra-data">
            Camilla Tunney
          </div>
          <div class="px-3 pb-3">
            <div class="chat-item flex extra-data">
              <img src="../assets/image/Profile14.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Camilla Tunney <span>11:48</span></div>
                <div class="message">Hehe, meeting with Manu in a moment. We’ll probably need an hour or so to get this fixed.</div>
              </div>
            </div>
            <div class="chat-item flex extra-data">
              <img src="../assets/image/Profile01.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Felix Levan <span>11:48</span></div>
                <div class="message">Cool, I’ll let Market know.</div>
              </div>
            </div>
            <div class="pl-12 pb-7">
              <img src="../assets/image/Image.png" alt="">
            </div>
            <div class="chat-item flex">
              <img src="../assets/image/Profile14.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Camilla Tunney <span>11:48</span></div>
                <div class="message">Hehe, meeting with Manu in a moment. We’ll probably need an hour or so to get this fixed.</div>
              </div>
            </div>
            <div class="chat-item flex mb-12">
              <img src="../assets/image/Profile01.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Felix Levan <span>11:52</span></div>
                <div class="message">Cool, I’ll let Market know.</div>
              </div>
            </div>
          </div>
          <div class="new-section px-3 pb-3 pt-12 relative">
            <div class="absolute p-2 text-tiny-gray z-50">New messages</div>
            <div class="chat-item flex">
              <img src="../assets/image/Profile14.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Camilla Tunney <span>16:31</span></div>
                <div class="message">Finally done with Manu. Got the fps to be twice as smooth using the smo function instead. All links are now anchored as well.</div>
              </div>
            </div>
            <div class="chat-item flex">
              <img src="../assets/image/Profile01.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Felix Levan <span>16:32</span></div>
                <div class="message">Done!</div>
                <div class="border p-4 rounded-sm flex items-center my-2">
                  <img src="../assets/image/icon-file.svg" alt="">
                  <div class="ml-4">
                    <div class="flex items-center">
                      <div class="mr-3">landing.zip</div>
                      <img src="../assets/image/Checked.svg" alt="">
                    </div>
                    <div class="text-sm-gray">Zip</div>
                  </div>
                </div>
              </div>
            </div>
            <div class="chat-item flex">
              <img src="../assets/image/Profile14.png" alt="" class="avatar">
              <div class="pt-2">
                <div class="name">Camilla Tunney <span>17:05</span></div>
                <div class="message">Looks awesome, thx! I’ll make sure Ernie pushes this asap. Market will be like..
                  super-duper happy.</div>
              </div>
            </div>
          </div>
        </div>

<!--        Box of sending message-->
        <div class="message-box p-4 border-t">
          <input type="text" placeholder="Message...">
          <div class="flex items-center justify-center">
            <img src="../assets/image/icon-add.svg" alt="">
          </div>
          <div class="flex items-center justify-center">
            <img src="../assets/image/icon-face-happy.svg" alt="">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
    export default {
        name: "Conversation"
    }
</script>

<style scoped>
  * {
    font-family: 'Lato', sans-serif;
  }
  .main-container {
    @apply min-h-screen grid overflow-hidden;
    grid-template-columns: 240px auto;
    background-color: #F2F2F2;
  }
  .mobile-top-part {
    @apply hidden;
  }
  .history-wrapper {
    @apply min-h-screen relative;
    background: linear-gradient(180deg, #FFFFFF 0%, #F6F6F9 97.34%);
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  }
  .menu-item {
    @apply px-3 py-2 flex items-center
  }
  .search {
    top: 12px;
    left: 8px;
  }
  .menu-item:hover {
    @apply rounded-sm;
    background: #ECECEE;
  }
  .menu-name {
    @apply font-normal ml-2;
    font-size: 14px;
    color: #110F24;
  }
  .user-list {
    @apply font-bold ml-2;
    font-size: 16px;
    color: #110F24;
  }
  .button-wrapper {
    @apply flex justify-between items-center p-3 absolute bottom-0 left-0 w-full;
    background-color: #ffffff;
    height: 56px;
  }
  .new-conv-btn {
    @apply flex justify-center items-center;
    background-color: #ECECEE;
    width: 124px;
    height: 32px;
    font-size: 12px;
  }
  .chat-wrapper {
    @apply px-4 pb-4 ;
  }
  .chat-box {
    @apply w-full h-full overflow-hidden flex flex-col justify-end;
    background-color: #ffffff;
    border-radius: 8px;
    box-shadow: 1px 2px 6px 2px #e2e2e2;
  }
  .message-box {
    @apply grid;
    grid-template-columns: auto 32px 32px;
  }
  input {
    @apply mr-2 pl-2 border;
    height: 40px;
    background-color: #F6F6F9;
    border-radius: 3px;
  }
  .new-section {
    @apply border-t;
  }
  .chat-item {
    @apply grid py-2;
    grid-template-columns: 40px auto;
    grid-gap: 8px;
    color: #110F24;
    font-size: 16px;
  }
  .avatar {
    width: 40px;
    height: 40px;
  }
  .chat-item span {
    @apply font-normal;
    color: rgba(17, 15, 36, 0.4);
  }
  .name {
    @apply font-bold;
  }
  .text-sm-gray {
    color: rgba(17, 15, 36, 0.4);
    font-size: 14px;
  }
  .text-tiny-gray {
    top: -19px;
    left: 50%;
    transform: translateX(-50%);
    color: rgba(17, 15, 36, 0.4);
    font-size: 12px;
    background-color: #ffffff;
  }
  .search-box {
    @apply px-7;
    width: 200px;
    background-color: #ffffff;
  }
  .chat-list {
    background-color: #ffffff;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  }
  .chat-subtitle {
    @apply font-bold;
    background-color: #F6F6F9;
  }

  .extra-data {
    @apply hidden;
  }

  @media only screen and (max-width: 992px) {
    /*.chat-wrapper {*/
    /*  @apply h-screen;*/
    /*}*/
  }

  @media only screen and (max-width: 768px) {
    .main-container {
      grid-template-columns: 1fr;
    }
    .history-wrapper {
      @apply hidden;
    }
    .mobile-top-part {
      @apply block;
    }
    .extra-data {
      @apply block;
    }
  }
</style>
