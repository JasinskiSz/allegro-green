<template>
  <article class="inline-flex flex-col items-start shadow-[0_4px_4px_0_rgba(0,0,0,0.25)]">
    <img :src :alt class="w-[17.875rem] h-[11.9375rem] aspect-[286/191]">
    <section
      class="flex flex-col items-start gap-1.5 bg-[var(--tailwind-v-400-white,#FFF)] min-h-[7.6875rem] p-[1.125rem] pb-3">
      <h3 class="text-[var(--tailwind-v-400-black,#000)] font-[Poppins] text-base not-italic font-bold leading-normal">
        {{ title }}
      </h3>
      <p
        class="w-[15.625rem] text-[var(--tailwind-v-400-black,#000)] font-[Poppins] text-xs not-italic font-normal leading-normal">
        {{ shortDesc }}
      </p>
      <p
        class="text-[var(--tailwind-v-400-green-600,#00A63E)] font-[Poppins] text-sm not-italic font-semibold leading-normal">
        {{ price }}
      </p>
    </section>
  </article>
</template>

<script lang="ts" setup>
// img tag in html above contains class specifying width, height and aspect ratio to properly display if incorrect src value is passed

const props = defineProps({
  src: {
    type: String,
    required: true,
    default: "/img/landscape-placeholder-img.png"
  },
  alt: {
    type: String,
    required: true
  }
});

const title = "Product name";
const shortDesc = "Product short description";
const price = "39.99 zł";
</script>

<style></style>