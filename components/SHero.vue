<template>
  <section
    class="flex flex-col justify-center items-center gap-3 py-12 px-[1.875rem] bg-[var(--tailwind-v-400-green-200,#B9F8CF)]">
    <h2
      class="flex justify-center items-center text-[var(--tailwind-v-400-black,#000)] font-[Poppins] text-[2rem] not-italic font-semibold leading-normal">
      {{ header }}
    </h2>
    <p
      class="flex justify-center items-center text-[var(--tailwind-v-400-black,#000)] font-[Poppins] text-base not-italic font-normal leading-normal">
      {{ paragraph }}
    </p>
    <div v-if="button" class="flex h-9 items-center">
      <button
        class="flex flex-col justify-center items-center self-stretch py-0 px-3 bg-[var(--tailwind-v-400-indigo-600,#4F39F6)] text-[var(--tailwind-v-400-white,#FFF)] font-[Poppins] text-base not-italic font-bold leading-normal">
        {{ button }}
      </button>
    </div>
  </section>
</template>

<script lang="ts" setup>
const props = defineProps({
  header: {
    type: String
  },
  paragraph: {
    type: String
  },
  button: {
    type: String
  }
});

</script>

<style></style>