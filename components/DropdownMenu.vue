<template>
  <UPopover>
    <UButton
      color="white"
      variant="soft"
      size="xs"
      :ui="{ rounded: 'rounded-full' }"
      class="text-neutral-600 hover:bg-gray-100"
    >
      <UIcon
        name="i-heroicons-chevron-down-16-solid"
        class="text-neutral-600 text-2xl"
      />
    </UButton>
    <template #panel>
      <div class="p-2 py-4 flex flex-col gap-1">
        <p class="text-xs">Currently In</p>
        <div
          class="flex p-2 gap-2 bg-neutral-200 rounded-lg my-2 hover:bg-gray-300"
        >
          <UAvatar
            src="https://avatars.githubusercontent.com/u/739984?v=4"
            alt="Avatar"
          />
          <p>User details</p>
        </div>
        <p class="text-xs mt-2">Your Accounts</p>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Add Account</p>
        </div>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Convert to business</p>
        </div>
        <p class="text-xs mt-2">More options</p>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Settings</p>
        </div>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Tune your home feed</p>
        </div>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Settings</p>
        </div>
        <div
          class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer flex justify-between items-center gap-2"
        >
          <p class="font-bold text-gray-900">Tune your home feed</p>
          <UIcon
            name="i-heroicons-arrow-top-right-on-square-20-solid"
            class="text-gray-900 text-md"
          />
        </div>
        <div class="py-1 hover:bg-gray-200 p-2 rounded-lg cursor-pointer">
          <p class="font-bold text-gray-900">Log out</p>
        </div>
      </div>
    </template>
  </UPopover>
</template>
