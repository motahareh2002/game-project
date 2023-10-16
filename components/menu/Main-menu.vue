
<script setup lang="ts">
const srcImg:Ref<string> = ref("https://ww2.freelogovectors.net/wp-content/uploads/2022/03/squad_logo_freelogovectors.net_.png")
</script>

<template>
    <div class="main-menu">
        <img :src="srcImg" alt="logo" class="w-[180px] h-auto">
        <button class="text-white md:hidden">
            <Icon name="zondicons:menu" size="25" />
        </button>
    </div>
</template>

<style scoped>
.main-menu{
    @apply bg-[#77747499]  px-10 py-[27px] sm:px-[50px] md:px-[150px] flex justify-between items-center
}
</style>