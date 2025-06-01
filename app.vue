<template>
  <div>
    <button @click="openModal" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
      open modal
    </button>
    <Modal v-model:visible="isModalOpen" />
  </div>
</template>
<script setup lang="ts">
const isModalOpen = ref(false);

const openModal = () => {
  isModalOpen.value = true;
}

</script>