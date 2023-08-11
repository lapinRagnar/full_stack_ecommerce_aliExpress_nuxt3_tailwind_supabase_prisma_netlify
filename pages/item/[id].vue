<template>
  <MainLayout>
    <div id="ItemPage class=mt-4 max-w-[1200px] mx-auto px-2">
      <div class="md:flex justify-between gap-4 mx-auto w-full">
        <div class="md:w-[40%]">
          <img 
            class="rounded-lg object-fit"
            src="https://picsum.photos/id/212/800/800"
          >

          <div v-if="images[0] !== ''" class="flex items-center justify-center mt-2">
            <div v-for="image in images" :key="image">
              <img 
                @mouseover="currentImage = image"
                @click="currentImage = image"
                width="70"
                class="rounded-md object-fit border-[3px] cursor-pointer"
                :class="currentImage === image ? 'border-[#FF5353]' : ''"
                :src="image"
              >
            </div>
          </div>

        </div>
      </div>
    </div>
  </MainLayout>

</template>

<script setup>

  import MainLayout from '~/layouts/MainLayout.vue'

  let currentImage = ref(null)

  onMounted(() => {
    watchEffect(() => {
      currentImage.value = 'https://picsum.photos/id/77/800/800',
      images.value[0] = 'https://picsum.photos/id/77/800/800'
    })
  })

  const images = ref([
    '',
    'https://picsum.photos/id/212/800/800',
    'https://picsum.photos/id/213/800/800',
    'https://picsum.photos/id/214/800/800',
    'https://picsum.photos/id/215/800/800',
    'https://picsum.photos/id/216/800/800',
    'https://picsum.photos/id/217/800/800',
    'https://picsum.photos/id/218/800/800',
    'https://picsum.photos/id/219/800/800',
    'https://picsum.photos/id/220/800/800'
    
  ])

</script>

<style lang="scss" scoped>

</style>