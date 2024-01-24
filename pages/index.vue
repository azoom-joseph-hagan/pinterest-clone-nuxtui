<template>
  <div>
    <Header />
    <main class="flex justify-center">
      <div
        class="grid gap-4 p-4 grid-cols-2 sm:grid-cols-3 xl:grid-cols-4 max-w-5xl"
      >
        <ClientOnly>
          <ImageCard v-for="image in images" :image="image" :key="image.id">
          </ImageCard>
        </ClientOnly>
      </div>
    </main>
  </div>
</template>
<script lang="ts" setup>
const getRandomSize = (min: number, max: number) => {
  let height = Math.floor(Math.random() * (max - min + 1) + min);
  let width = Math.floor(Math.random() * (max - min + 1) + min);

  height = Math.round(height / 10) * 10;
  width = Math.round(width / 10) * 10;

  return `${height}x${width}`;
};
let images = Array.from({ length: 20 }, (_, index) => ({
  id: index + 1,
  imageUrl: `https://source.unsplash.com/random/${getRandomSize(300, 600)}`,
  title: `Title ${index + 1}`,
  description: `Description for image ${index + 1}`,
}));
</script>
