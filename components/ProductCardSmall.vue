<template>
  <article class="inline-flex flex-col items-start shadow-[0_4px_4px_0_rgba(0,0,0,0.25)]">
    <img :src :alt class="w-[11.91669rem] h-[11.91669rem] aspect-[1/1]">
    <section class="flex flex-col items-center self-stretch gap-1.5 h-[5.5625rem] p-[1.125rem] pt-2">
      <p
        class="text-[var(--tailwind-v-400-green-600,#00A63E)] font-[Poppins] text-sm not-italic font-semibold leading-normal">
        {{ price }}
      </p>
      <p class="text-center font-[Poppins] text-xs not-italic font-medium leading-normal self-stretch">
        {{ title }}
      </p>
    </section>
  </article>
</template>

<script lang="ts" setup>
// TODO: This card may be implemented differently. It could be some kind of variant of already exisiting ProductCard component.
// TODO: Something is wrong with background color on different ProductSections in this card.

const props = defineProps({
  src: {
    type: String,
    required: true,
    default: "/img/1to1-placeholder-img.png"
  },
  alt: {
    type: String,
    required: true
  }
});

const title = "Product name";
const price = "39.99 zł";

</script>

<style></style>