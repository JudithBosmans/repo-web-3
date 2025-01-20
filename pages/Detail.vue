<template>
  <div class="relative z-10 pr-5 bg-transparent">
    <Drawer />
  </div>

  <nuxt-link to="/" class="absolute top-9 left-9 z-[99]">
    <svg
      class="w-6 h-6 arrow"
      aria-hidden="true"
      xmlns="http://www.w3.org/2000/svg"
      width="24"
      height="24"
      fill="none"
      viewBox="0 0 24 24"
    >
      <path
        stroke="currentColor"
        stroke-linecap="round"
        stroke-linejoin="round"
        stroke-width="2"
        d="M5 12h14M5 12l4-4m-4 4 4 4"
      />
    </svg>
  </nuxt-link>

  <main class="flex flex-col items-center justify-center bodyText mb-[20vh]">
    <img
      :src="work.img"
      class="w-[50vh] h-[50vh] mx-auto mt-[5%] object-cover"
      :alt="work.title"
    />
    <div
      class="grid grid-cols-3 grid-rows-1 gap-4 w-[90%] mx-auto mt-[5%] bodyText"
    >
      <div>
        <p class="h-[10vh]">{{ work.title }}</p>
        <img :src="work.img1" class="w-[25vw] h-[25vw] mt-3" />
      </div>
      <div>
        <p class="h-[10vh]">{{ work.skills }}</p>
        <img :src="work.img1" class="w-[25vw] h-[25vw] mt-3" />
      </div>
      <div>
        <p class="h-[10vh] w-[70%]">{{ work.desc }}</p>
        <img :src="work.img1" class="w-[25vw] h-[25vw] mt-3" />
      </div>
    </div>
  </main>
</template>

<script>
export default {
  data() {
    return {
      work: {},
    };
  },
  mounted() {
    this.work = JSON.parse(this.$route.query.work || "{}");
  },
};
</script>
