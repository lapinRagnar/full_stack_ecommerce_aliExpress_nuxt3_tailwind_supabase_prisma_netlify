<template>
  <MainLayout>
    <div id="IndexPage" class="mt-4 max-w-[1200px]  mx-auto px-2">
      <div class="grid xl:grid-cols-6 lg:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4">
        <div v-if="products" v-for="product in products" :key="product">
          <ProductComponent :product="product" />
        </div>
      </div>
    </div>
  </MainLayout>
</template>

<script setup>
  import MainLayout from '~/layouts/MainLayout.vue'

  const products = [
    {id: 1, title: 'title 1', description: 'description 1', price: 9999, url: 'https://picsum.photos/id/7/800/600'},
    {id: 2, title: 'title 2', description: 'description 2', price: 9989, url: 'https://picsum.photos/id/4/800/600'},
    {id: 3, title: 'title 3', description: 'description 3', price: 5999, url: 'https://picsum.photos/id/1/800/600'},
    {id: 4, title: 'title 4', description: 'description 4', price: 1999, url: 'https://picsum.photos/id/2/800/600'},
    {id: 5, title: 'title 5', description: 'description 5', price: 5999, url: 'https://picsum.photos/id/3/800/600'},
    {id: 6, title: 'title 6', description: 'description 6', price: 8999, url: 'https://picsum.photos/id/6/800/600'},
    {id: 7, title: 'title 7', description: 'description 7', price: 2299, url: 'https://picsum.photos/id/5/800/600'},
    {id: 8, title: 'title 8', description: 'description 8', price: 5621, url: 'https://picsum.photos/id/8/800/600'},
    {id: 9, title: 'title 9', description: 'description 9', price: 5846, url: 'https://picsum.photos/id/9/800/600'},
    {id: 10, title: 'title 10', description: 'description 10', price: 7546, url: 'https://picsum.photos/10/7/800/600'},
  ]
</script>

<style lang="scss" scoped>

</style>