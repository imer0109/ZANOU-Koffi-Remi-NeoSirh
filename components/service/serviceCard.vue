<template>
  <div class="flex justify-center">
    <div class="min-h-[22rem] w-[20rem] bg-white rounded-lg p-10 shadow-xl shadow-blue-100 mb-10">
      <!-- image -->
      <div class="flex justify-center">
        <img :src="image" alt="" class="size-16" />
      </div>

      <!-- title -->
      <p class="text-xl font-bold my-4">{{ title }}</p>

      <!-- sub title -->
      <p 
      class="text-[18px] mb-5 text-gray-500"
      :class="{'line-clamp-4' : !voirPlus}"
      >{{ subTitle }}</p>

      <!-- voir plus -->
      <div
        @click="voirPlus = !voirPlus"
       class="flex justify-center items-center space-x-3 text-primary cursor-pointer">
        <span>Voir plus</span>
        <ArrowLeftIcon class="size-6"/>
      </div>
    </div>
  </div>
</template>

<script setup>
import ArrowLeftIcon from '../icons/arrowLeftIcon.vue';

defineProps({
  image: {
    required: true,
  },

  title: {
    required: true,
  },

  subTitle: {
    required: true,
  },
});


const voirPlus = ref(false);

</script>

<style>
</style>