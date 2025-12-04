<script setup lang="ts"></script>

<template>
  <header>
    <div class="max-w-[1320px] mx-auto px-3 lg:px-5">
      <div class="flex items-center gap-2 md:gap-6 py-3 lg:py-4">
        <h1><a href="javascript:;" class="block leading-0"><img src="/src/assets/logo.png" alt="ZOBAA"></a></h1>
        <div class="flex justify-between items-center w-full">
          <div class="max-w-[400px] w-full">
            <form action="" class="relative">
              <div class="w-6 h-6 absolute start-3 top-1/2 -translate-y-1/2">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M19.6 21L13.3 14.7C12.8 15.1 12.225 15.4167 11.575 15.65C10.925 15.8833 10.2333 16 9.5 16C7.68333 16 6.14583 15.3708 4.8875 14.1125C3.62917 12.8542 3 11.3167 3 9.5C3 7.68333 3.62917 6.14583 4.8875 4.8875C6.14583 3.62917 7.68333 3 9.5 3C11.3167 3 12.8542 3.62917 14.1125 4.8875C15.3708 6.14583 16 7.68333 16 9.5C16 10.2333 15.8833 10.925 15.65 11.575C15.4167 12.225 15.1 12.8 14.7 13.3L21 19.6L19.6 21ZM9.5 14C10.75 14 11.8125 13.5625 12.6875 12.6875C13.5625 11.8125 14 10.75 14 9.5C14 8.25 13.5625 7.1875 12.6875 6.3125C11.8125 5.4375 10.75 5 9.5 5C8.25 5 7.1875 5.4375 6.3125 6.3125C5.4375 7.1875 5 8.25 5 9.5C5 10.75 5.4375 11.8125 6.3125 12.6875C7.1875 13.5625 8.25 14 9.5 14Z" fill="#909090"/>
                </svg>
              </div>
              <input id="headerSearch" type="text" class="py-2.5 ps-10 pe-3 leading-[1.2] placeholder-neutral-60 font-semibold bg-white border border-nertral-40 focus:border-nertral-40 rounded-lg w-full" placeholder="搜尋景點、地點或城市">
            </form>
          </div>
          <div class="flex items-center gap-4">
            <button type="button" class="hover:cursor-pointer flex items-center justify-center h-10 w-12">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M8.00179 22C7.45162 22 6.98082 21.8043 6.58937 21.413C6.19725 21.021 6.00119 20.55 6.00119 20C6.00119 19.45 6.19725 18.979 6.58937 18.587C6.98082 18.1957 7.45162 18 8.00179 18C8.55195 18 9.02276 18.1957 9.41421 18.587C9.80632 18.979 10.0024 19.45 10.0024 20C10.0024 20.55 9.80632 21.021 9.41421 21.413C9.02276 21.8043 8.55195 22 8.00179 22ZM18.0048 22C17.4546 22 16.9838 21.8043 16.5923 21.413C16.2002 21.021 16.0042 20.55 16.0042 20C16.0042 19.45 16.2002 18.979 16.5923 18.587C16.9838 18.1957 17.4546 18 18.0048 18C18.5549 18 19.0261 18.1957 19.4182 18.587C19.8096 18.979 20.0054 19.45 20.0054 20C20.0054 20.55 19.8096 21.021 19.4182 21.413C19.0261 21.8043 18.5549 22 18.0048 22ZM7.15153 6L9.55225 11H16.5543L19.3052 6H7.15153ZM6.20125 4H20.9556C21.4058 4 21.7142 4.16667 21.8809 4.5C22.0476 4.83333 22.0393 5.18333 21.8559 5.55L18.3049 11.95C18.1215 12.2833 17.8797 12.5417 17.5796 12.725C17.2795 12.9083 16.9378 13 16.5543 13H9.10211L8.00179 15H20.0054V17H8.00179C7.25156 17 6.68473 16.6707 6.30128 16.012C5.91783 15.354 5.90116 14.7 6.25127 14.05L7.60167 11.6L4.0006 4H2V2H5.25097L6.20125 4Z" fill="#4B4B4B"/></svg>
            </button>
            <button type="button" class="cursor-pointer py-4 px-8 bg-primary-100 text-white rounded-xl">登入 / 註冊</button>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
  header {
    background-color: #D5D5DD;
    backdrop-filter: blur(40px);
  }
</style>
