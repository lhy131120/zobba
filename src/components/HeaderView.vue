<script setup lang="ts"></script>

<template>
  <header class="max-w-[1320px] mx-auto px-3 lg:px-5">
    <div class="flex gap-2 md:gap-6 py-3 lg:py-4">
      <h1><a href="javascript:;" class="block leading-0"><img src="/src/assets/logo.png" alt="ZOBAA"></a></h1>
      <div class="flex">
        <div>
          <form action="" class="relative">
            <div></div>
            <input id="headerSearch" type="text" class="py-2.5 ps-10 pe-3 leading-[1.2] placeholder-neutral-60 font-semibold border border-nertral-40 focus:border-nertral-40 rounded-lg" placeholder="搜尋景點、地點或城市">
          </form>
        </div>
        <div class="flex items-center gap-4">
          <button type="button" class="cursor-pointer flex h-10 w-12 bg-amber-200"></button>
          <button type="button" class="cursor-pointer py-4 px-8 bg-primary-100 text-white rounded-xl">登入 / 註冊</button>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped></style>
