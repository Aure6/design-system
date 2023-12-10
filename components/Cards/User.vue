<script setup>
defineProps({
  to: {
    type: String,
    required: true,
  },
  avatar: {
    type: String,
    required: true,
  },
  fullname: {
    type: String,
    required: true,
  },
  info: {
    type: String,
    required: false,
  },
  src: {
    type: String,
    required: true,
  },
  alt: {
    type: String,
    required: false,
  },
});
</script>

<template>
  <NuxtLink :to="to"
    class="flex flex-col p-4 max-w-xs group hover:bg-gray-200/75 transition items-center justify-center ring-2 ring-gray-200/75 my-8 space-y-2"
    :avatar="avatar" :info="info" :src="src" :alt="alt">
    <div class=" text-5xl text-gray-400 group-hover:text-gray-800 transition">
      <img :src=src alt="">
      <!-- slot avatar -->
      <slot name="avatar" />
    </div>

    <div class="text-xl text-gray-100 group-hover:text-black group-hover:underline transition">
      <slot name="fullname" />
    </div>
    <div class="block text-gray-100 group-hover:text-black group-hover:underline transition">
      <slot name="info" />
    </div>
  </NuxtLink>
</template>

<!-- <template>
  <NuxtLink :to="to"
    class="flex flex-col p-4 max-w-xs group hover:bg-gray-200/75 transition items-center justify-center ring-2 ring-gray-200/75 my-8 space-y-2"
    :avatar="avatar" :info="info" :src="src" :alt="alt">
    <div class=" text-5xl text-gray-400 group-hover:text-gray-800 transition">
      <slot name="avatar" />
    </div>

    <div class="text-xl text-gray-100 group-hover:text-black group-hover:underline transition">
      <slot name="fullname" />
    </div>
    <div class="block text-gray-100 group-hover:text-black group-hover:underline transition">
      <slot name="info" />
    </div>
  </NuxtLink>
</template> -->
