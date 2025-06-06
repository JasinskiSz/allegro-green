<template>
  <SHero header="Zielone zakupy, lepszy świat"
    paragraph="Oferujemy produkty eco, lokalne i zrównoważone. Zacznij zmieniać świat już dziś!"
    button="Przeglądaj produkty" />
  <button @click="openModal" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
    open modal
  </button>
  <Modal v-model:visible="isModalOpen" :username="getUsername()" />
</template>
<script setup lang="ts">
const isModalOpen = ref(false);

const openModal = () => {
  if (isModalOpen.value) {
    console.warn("Modal is already open");
    return;
  }
  isModalOpen.value = true;
}

// fetch username from a function
const getUsername = (): string => {
  const username = "Szymon Jasiński"; // Mocked username, replace with fetch from API or other source
  if (!username || typeof username !== "string") {
    console.error("Invalid username detected");
    return "Unknown user";
  }
  return username;
}

</script>