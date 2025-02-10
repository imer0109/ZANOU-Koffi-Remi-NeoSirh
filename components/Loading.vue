<template>
  <!-- Modal -->
  <client-only>
    <TransitionRoot appear :show="isLoading" as="template">
      <Dialog as="div" @close="isLoading = false" class="relative z-[51]">
        <TransitionChild
          as="template"
          enter="duration-300 ease-out"
          enter-from="opacity-0"
          enter-to="opacity-100"
          leave="duration-200 ease-in"
          leave-from="opacity-100"
          leave-to="opacity-0"
        >
          <DialogOverlay class="fixed inset-0 bg-[black]/60" />
        </TransitionChild>

        <div class="fixed inset-0 overflow-y-auto flex justify-center">
          <span class="m-auto inline-block h-32 w-32 animate-[ping_2s_linear_infinite] align-middle">
            <img src="/assets/images/icon-sirh.png" alt="">
        </span>
        </div>
      </Dialog>
    </TransitionRoot>
  </client-only>
</template>

<script setup>
import { TransitionRoot, TransitionChild, Dialog, DialogPanel, DialogOverlay, TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';

defineProps({
  isLoading: {
    type: Boolean,
    required: true,
    default: false,
  },
});
</script>