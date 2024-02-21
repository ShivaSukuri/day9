<template>
    <div>
    
<h1>Heloo iam index</h1>
<button @click="navigate">Navigate</button>
<h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
    <button class="text-white px-4 sm:px-8 py-2 sm:py-3 bg-sky-700 hover:bg-sky-800">submit</button>
    </div>
</template>

<script setup>
  const navigate=()=>{
    navigateTo('/Home')
  }
</script>

<style lang="scss" scoped>

</style>