<template>
    <div>
        <Head>
            <Title>Nuxt3-{{ name }}</Title>
        </Head>
    </div>
    <div>
        <h1>iphone {{ name }}</h1>
        <img :src="`/images/iphone${route.params.name}.webp`" alt="">
        <button class="text-white px-4 sm:px-8 py-2 sm:py-3 bg-sky-700 hover:bg-sky-800" @click="addToCart">Buy now</button>
    </div>
</template>

<script setup>
const cart = useCart();
const route= useRoute();
    const name=computed(()=>{
    return route.params.name.replaceAll('-',' ');
})
const addToCart=()=>{
    cart.value.push({
        name:`${route.params.name}`
    })
    console.log(cart.value)
}
</script>

<style lang="scss" scoped>

</style>