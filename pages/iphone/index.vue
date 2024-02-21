<template>
    <div  class="grid grid-cols-4 gap-3 mt-20">
        <!-- <NuxtLink to="iphone/iphone-12" class="shadow-lg text-center">
            <h1>Samsung ultra</h1>
            <img width="200" src="/images/samsung.webp" alt="">
        </NuxtLink> -->
        <NuxtLink to="iphone/iphone-15" class="shadow-lg text-center">
            <h1>iphone 15</h1>
            <img width="200" src="/images/iphone15.webp" alt="">
        </NuxtLink>
        <NuxtLink to="iphone/iphone-14" class="shadow-lg text-center">
            <h1>iphone 14</h1>
            <img width="200" src="/images/iphone14.webp" alt="">
        </NuxtLink>
        <NuxtLink to="iphone/iphone-13" class="shadow-lg text-center">
            <h1>iphone 13</h1>
            <img width="200" src="/images/iphone13.webp" alt="">
        </NuxtLink>
    </div>
</template>

<script setup>
useHead({
    title:"nuxt3-phones"
})
    
</script>

<style lang="scss" scoped>
// .content{
//     display: grid;
//     grid-template-columns: repeat(auto-fill,minmax(200px,1fr));
//     text-align: center  ;

// }
</style>