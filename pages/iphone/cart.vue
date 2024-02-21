<template>
    <div>
        <div class="grid grid-cols-4 gap-4 ">
            <div v-for="item of items" >
            <p> iphone{{ item.name }}</p>
            <img width="200" :src="`/images/iphone${item.name}.webp`" alt="">
            <button class="text-white px-4 sm:px-8 py-2 sm:py-3 bg-red-700 hover:bg-red-800" @click="removeFromCart(item)">Delete</button>
            
        </div>
        </div>
        
    </div>
</template>

<script setup>
   const cart=useCart();
const items=ref(cart.value);
const removeFromCart=(item)=>{
    const index=items.findIndex((obj) => obj.id === item.name);
    console.log(index)
//    items.splice(item)
    
}
</script>

<style lang="scss" scoped>

</style>

