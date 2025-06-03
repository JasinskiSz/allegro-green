<template>
  <header class="flex justify-between items-center px-16 py-8 bg-[var(--tailwind-v-400-green-600,#00A63E)]">
    <div class="flex justify-center items-center">
      <p class="text-[var(--tailwind-v-400-white,#FFF)] font-[Poppins] text-[1.5rem] font-bold leading-normal">
        Green Allegro
      </p>
    </div>

    <div
      class="flex flex-[1_0_0] justify-center items-center min-w-[37.5rem] max-w-[62.5rem] self-stretch py-0 px-[4.125rem]">
      <div class="flex flex-[1_0_0] justify-center items-center self-stretch bg-[var(--tailwind-v-400-white,#FFF)]">
        <input type="text"
          class="flex flex-[1_0_0] justify-center items-center py-0 px-3 self-stretch font-[Poppins] text-[1rem] font-normal not-italic"
          placeholder="Czego szukasz?">
      </div>

      <div class="flex items-center self-stretch">

      </div>
    </div>

    <nav>
      <ul class="flex items-center gap-3">
        <li class="flex flex-col justify-center items-center">
          <NuxtLink class="nav-link self-stretch" to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink class="nav-link self-stretch" to="/categories">Kategorie</NuxtLink>
        </li>
        <li>
          <NuxtLink class="nav-link self-stretch" to="/promotions">Promocje</NuxtLink>
        </li>
        <li>
          <NuxtLink class="nav-link self-stretch" to="/contact">Kontakt</NuxtLink>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script lang="ts" setup>

</script>

<style scoped>
.nav-link {
  color: var(--tailwind-v-400-white, #FFF);
  font-family: Poppins;
  font-style: normal;
  font-weight: 500;
  font-size: 1rem;
  line-height: normal;
}
</style>