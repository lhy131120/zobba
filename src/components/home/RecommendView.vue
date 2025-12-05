<script setup lang="ts">
  import { ref } from 'vue';

  const hoveredIndex = ref<number | null>(null)

  interface Card {
    title: string;
    description: string;
    imgUrl: string;
  }

  const cardsInfo= ref<Card[]>([
    {
      title:'峇里島渡假漫遊',
      description: '精選五星級海灘度假村，專屬私人管家服務，讓您徹底放鬆身心。',
      imgUrl: '/src/assets/images/home/hero-img1.jpg',
    },
    {
      title:'日本深度賞櫻計畫',
      description: '春季限定，東京、京都、大阪賞櫻之旅，體驗日本文化的精髓。',
      imgUrl: '/src/assets/images/home/hero-img2.jpg',
    },
    {
      title:'紐西蘭雪山探險',
      description: '探索南島壯麗的自然風光，體驗各種極限運動和戶外活動。',
      imgUrl: '/src/assets/images/home/hero-img3.jpg',
    },
    {
      title:'摩洛哥迷幻之旅',
      description: '漫步沙漠與古城之間，探索千年文化與色彩繽紛的市集風情。',
      imgUrl: '/src/assets/images/home/hero-img4.jpg',
    },
  ]);
</script>

<template>
  <div class="bg-linear-to-b from-[#221F1E] to-[#221F1E] py-10 lg:py-[120px]">
    <div class="max-w-[1320px] mx-auto w-full px-3">
      <div class="flex items-center lg:justify-between flex-wrap lg:flex-nowrap text-white gap-6 lg:gap-4 mb-10 lg:mb-20">
        <h2 class="text-3xl lg:text-7xl">你的<br>專屬推薦</h2>
        <div class="font-bold w-full lg:w-auto">
          <p class="mb-1 lg:mb-2 text-sm lg:text-xl leading-normal lg:leading-tight">來看我們的精選推薦行程，滿意度高達 99.2%</p>
          <p class="mb-3 lg:mb-6 text-sm lg:text-xl leading-normal lg:leading-tight">給自己一個難忘的旅遊行程吧！</p>
          <a href="javascript:;" class="inline-flex items-center gap-1">
            <span class="text">查看全部行程</span>
            <span class="block w-4 lg:w-6 h-4 lg:h-6">
              <svg class="w-full h-full" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g clip-path="url(#clip0_187_42521)"><path d="M12 4L10.59 5.41L16.17 11H4V13H16.17L10.59 18.59L12 20L20 12L12 4Z" fill="white"/></g><defs><clipPath id="clip0_187_42521"><rect width="24" height="24" fill="white"/></clipPath></defs></svg>
            </span>
          </a>
        </div>
      </div>

      <!-- Cards -->
      <div>
        <ul class="list-none flex gap-6">
          <li v-for="(card, index) in cardsInfo" :key="card.title" @mouseenter="hoveredIndex = index"  @mouseleave="hoveredIndex = null" class="group relative h-[600px] overflow-hidden rounded-3xl transition-all duration-500 ease-out":class="hoveredIndex === index ? 'lg:w-[416px] lg:min-w-[416px]' : 'lg:w-full lg:min-w-0'">
            <!-- 背景圖 -->
            <div class="absolute inset-0 bg-cover bg-center transition-transform duration-500 group-hover:scale-110" :style="{ backgroundImage: `url(${card.imgUrl})` }"></div>
            <!-- 黑色漸層遮罩 + 文字 -->
            <div class="relative h-full p-8 flex flex-col justify-end">
              <div class="text-white transform-gpu transition-all duration-800 ease-out translate-y-2">
                <h3 class="mb-3 text-[40px] leading-tight drop-shadow-2xl">{{ card.title }}</h3>
                <p class="drop-shadow-lg">{{ card.description }}</p>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
  .card {
    max-width: 416px;
    width: auto;
  }
</style>