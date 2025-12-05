<template>
  <div id="hemoHero" class="bg-primary-400 flex justify-center">
    <div class="max-w-[904px] w-full mx-auto px-3 mt-12 lg:mt-[10%]">
      <!-- text area -->
      <div class="mb-6 lg:mb-10 font-bold">
        <div class="inline-block text-primary-100 bg-primary-10 rounded-2xl text-xl mb-3 p-2 lg:p-4">ZOBAA 旅行推薦平台</div>
        <h2 class="text-primary-100 text-3xl lg:text-7xl mb-2 lg:mb-6">用旅行，<br class="lg:hidden">收藏世界的樣子</h2>
        <p class="text-sm lg:text-xl text-primary-80">ZOBAA 整合熱門景點推薦、即時優惠、獨家行程，從比價到訂購，一次完成你的完美出遊計畫。</p>
      </div>
      <!-- input area -->
      <div>
        <form action="" class="relative max-w-[720px]">
          <div class="w-6 h-6 absolute start-3 top-1/2 -translate-y-1/2">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M19.6 21L13.3 14.7C12.8 15.1 12.225 15.4167 11.575 15.65C10.925 15.8833 10.2333 16 9.5 16C7.68333 16 6.14583 15.3708 4.8875 14.1125C3.62917 12.8542 3 11.3167 3 9.5C3 7.68333 3.62917 6.14583 4.8875 4.8875C6.14583 3.62917 7.68333 3 9.5 3C11.3167 3 12.8542 3.62917 14.1125 4.8875C15.3708 6.14583 16 7.68333 16 9.5C16 10.2333 15.8833 10.925 15.65 11.575C15.4167 12.225 15.1 12.8 14.7 13.3L21 19.6L19.6 21ZM9.5 14C10.75 14 11.8125 13.5625 12.6875 12.6875C13.5625 11.8125 14 10.75 14 9.5C14 8.25 13.5625 7.1875 12.6875 6.3125C11.8125 5.4375 10.75 5 9.5 5C8.25 5 7.1875 5.4375 6.3125 6.3125C5.4375 7.1875 5 8.25 5 9.5C5 10.75 5.4375 11.8125 6.3125 12.6875C7.1875 13.5625 8.25 14 9.5 14Z" fill="#909090"/>
            </svg>
          </div>
          <input id="headerSearch" type="text" class="ps-10 py-[22px] pe-[150px] leading-tight placeholder-neutral-60 font-semibold bg-white border border-nertral-40 focus:border-nertral-40 rounded-2xl w-full text-base" placeholder="搜尋景點、地點或城市">
          <button type="button" class="absolute top-1/2 end-2 -translate-y-1/2 tracking-main hover:cursor-pointer font-semibold py-3 px-4 text-white bg-primary-100 rounded-xl">開始探索旅程</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
  #hemoHero {
    background: url('/src/assets/images/home/home-hero.jpg') no-repeat center center / cover;
    aspect-ratio: 1920 / 1080;
  }

  @media (max-width: 991.98px) {
    #hemoHero {
      aspect-ratio: 480 / 375;
    }
  }
</style>