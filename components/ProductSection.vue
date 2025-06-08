<template>
  <section :style="{ backgroundColor: `var(${bgColor})` }" class="flex flex-col items-center gap-5 py-12 px-[4.125rem]">
    <div class="flex flex-col items-center gap-5">
      <h2
        class="text-[var(--tailwind-v-400-black,#000)] font-[Poppins] text-xl not-italic font-semibold leading-normal">
        {{ sectionTitle }}
      </h2>
      <div class="flex justify-center items-start gap-6 pt-0 px-1 pb-1.5">
        <ProductCard src="/img/landscape-placeholder-img.png" alt="placeholder-img" />
        <ProductCard src="/img/landscape-placeholder-img.png" alt="placeholder-img" />
        <ProductCard src="/img/landscape-placeholder-img.png" alt="placeholder-img" />
        <ProductCard src="/img/landscape-placeholder-img.png" alt="placeholder-img" />
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup>
// TODO: div element with product cards may be changed to list
// TODO: ProductCard component may be looped

const props = defineProps({
  sectionTitle: String,
  bgColor: {
    type: String,
    default: "#fff"
  }
});
</script>

<style></style>