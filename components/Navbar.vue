<<template>
    <div>

        <div id="nav" class="flex  justify-around items-center bg-purple-600">
            <nuxt-link to="/" >index</nuxt-link>
            <nuxt-link to="/Home" >Home</nuxt-link>
            <nuxt-link to="/profile" >profile</nuxt-link>
            <nuxt-link to="/iphone">phones</nuxt-link>
            <nuxt-link to="/iphone/cart">Cart({{ item.length }})</nuxt-link>
        </div>
     
    </div>
</template>

<script setup>
   const cart=useCart();
   const item=ref(cart.value)
   console.log(cart.value)
</script>

<style lang="scss" scoped>

#nav{
    height:60px;
}
</style>