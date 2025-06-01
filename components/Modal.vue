<template>
  <div v-if="visible" class="fixed inset-0 z-50 flex items-center justify-center bg-black/50">
    <div class="relative bg-white rounded-lg shadow-lg w-96">
      <button @click="emitClose" class="absolute top-2 right-2 text-gray-500 hover:text-gray-700">
        X
      </button>
      <div class="p-6">
        <h2 class="text-2xl font-bold mb-4">
          This is Modal
        </h2>
        <p class="text-gray-700">
          Paragraph text in the modal
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
const props = defineProps({
  visible: {
    type: Boolean,
    required: true
  }
});

const emit = defineEmits(['update:visible']);

const emitClose = () => {
  emit('update:visible', false);
};

</script>

<style></style>