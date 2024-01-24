<template>
  <div
    class="image-card relative w-full overflow-hidden rounded-xl bg-blue-400"
  >
    <img class="h-full w-full object-cover" :src="image.imageUrl" />
  </div>
</template>
<script lang="ts" setup>
const props = defineProps<{
  image: {
    id: number;
    imageUrl: string;
    title: string;
    description: string;
  };
}>();
</script>
