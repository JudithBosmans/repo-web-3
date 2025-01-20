<template>
  <main class="flex items-center justify-center min-h-screen bodyText">
    <div class="grid grid-cols-12 grid-rows-12 gap-4 w-[90vw]">
      <div class="col-start-1 col-end-5 row-start-2 row-end-5">
        <h2 class="subtitle">
          But don't take <span class="italic">my word</span> for it
        </h2>
        <p class="bodyText text-left text-base mt-[2vh] mb-[2vh]">
          Here are some works from the past years, mostly school projects but
          also some personal stuff.
        </p>
        <nuxt-link class="button" to="/Detail">Check it out</nuxt-link>
      </div>

      <div
        v-for="(work, index) in works"
        :key="index"
        :class="gridClasses[index]"
      >
        <nuxt-link
          :to="{ path: '/detail', query: { work: JSON.stringify(work) } }"
        >
          <img
            :src="work.img"
            class="object-cover w-[100%] h-[100%] greyscaleImg"
            :alt="work.title"
        /></nuxt-link>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  data() {
    return {
      works: [],
      gridClasses: [
        "col-start-3 col-end-6 row-start-4 row-end-9",
        "col-start-6 col-end-9 row-start-1 row-end-5",
        "col-start-6 col-end-9 row-start-5 row-end-9",
        "col-start-9 col-end-12 row-start-2 row-end-6",
        "col-start-9 col-end-12 row-start-6 row-end-9",
      ],
    };
  },
  async created() {
    try {
      const response = await fetch("/_data/detail.json");
      const data = await response.json();
      this.works = Object.values(data.works[0]);
    } catch (error) {
      console.error("Failed to load works data:", error);
    }
  },
};
</script>

<style>
.greyscaleImg {
  filter: grayscale(100%);
}
</style>
