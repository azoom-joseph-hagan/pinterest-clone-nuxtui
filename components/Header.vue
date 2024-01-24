<template>
  <nav class="flex justify-center items- p-4 gap-2">
    <UButton
      color="white"
      variant="soft"
      size="xl"
      icon="i-heroicons-arrow-up-circle-solid"
      :ui="{ rounded: 'rounded-full' }"
      class="text-red-600 hover:bg-gray-100"
    />
    <UButton
      color="black"
      variant="solid"
      size="xl"
      :ui="{ rounded: 'rounded-full' }"
      class="py-3"
      >Home</UButton
    >
    <UButton
      color="black"
      variant="ghost"
      size="xl"
      :ui="{ rounded: 'rounded-full' }"
      class="py-3"
      >Create</UButton
    >
    <UInput
      color="gray"
      size="xl"
      placeholder="Search"
      class="flex grow focus:ring-red-400"
      :ui="{ rounded: 'rounded-full' }"
    >
      <template #leading>
        <UIcon
          name="i-heroicons-magnifying-glass-16-solid"
          class="text-gray-500 text-xl"
        />
      </template>
    </UInput>
    <UButton
      color="white"
      variant="soft"
      size="md"
      :ui="{ rounded: 'rounded-full' }"
      class="text-gray-500 hover:bg-gray-100"
    >
      <UIcon name="i-heroicons-bell-16-solid" class="text-neutral-600 text-3xl"
    /></UButton>
    <UButton
      color="white"
      variant="soft"
      size="md"
      :ui="{ rounded: 'rounded-full' }"
      class="text-neutral-600 hover:bg-gray-100"
    >
      <UIcon
        name="i-heroicons-chat-bubble-oval-left-ellipsis-16-solid"
        class="text-neutral-600 text-3xl"
    /></UButton>
    <UButton
      color="white"
      variant="soft"
      size="md"
      :ui="{ rounded: 'rounded-full' }"
      class="text-neutral-600 hover:bg-gray-100"
    >
      <UAvatar
        src="https://avatars.githubusercontent.com/u/739984?v=4"
        alt="Avatar"
      />
    </UButton>
    <DropdownMenu />
  </nav>
</template>
<script lang="ts" setup>
const value = ref("");
</script>
