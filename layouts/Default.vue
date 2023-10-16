
<script setup lang="ts">
const srcImg:Ref<string> = ref("https://ww2.freelogovectors.net/wp-content/uploads/2022/03/squad_logo_freelogovectors.net_.png")
</script>

<template>
  <div class="bg-[#181c23] w-full h-full min-h-screen">
    <div
      class="header-top"
    >
      <Social-icon />
      <HeaderRight />
    </div>
    <div class="bg-[#77747499]  px-10 py-[27px] sm:px-[50px] md:px-[150px] flex justify-between items-center">
        <img :src="srcImg" alt="logo" class="w-[180px] h-auto">
        <button class="text-white md:hidden">
            <Icon name="zondicons:menu" size="25" />
        </button>
    </div>
    <slot />
  </div>
</template>


<style scoped>
    .header-top{
        @apply  flex flex-col items-center py-[8px] bg-[#292e38] sm:flex-row sm:justify-between sm:py-[0.5px] sm:px-[50px] md:px-[150px]
    }
</style>