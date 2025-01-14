<script setup>
import { ref, onMounted } from "vue";
import About from "../components/About.vue";

const router = useRouter();

const homepageSettings = ref(null); // For homepage.json data
const generalSettings = ref(null); // For settings.json data

const isLoading = ref(true); // Loading state
const hasError = ref(false); // Error state

onMounted(async () => {
  try {
    // Fetch homepage.json
    const homepageResponse = await fetch("/_data/homepage.json");
    if (!homepageResponse.ok) {
      throw new Error(
        `Homepage settings error! status: ${homepageResponse.status}`
      );
    }
    const homepageData = await homepageResponse.json();
    homepageSettings.value = homepageData;

    // Fetch settings.json
    const settingsResponse = await fetch("/_data/settings.json");
    if (!settingsResponse.ok) {
      throw new Error(
        `General settings error! status: ${settingsResponse.status}`
      );
    }
    generalSettings.value = await settingsResponse.json();

    isLoading.value = false; // Stop loading when both files are fetched
  } catch (error) {
    hasError.value = true; // Show error message if fetching fails
    console.error("Error loading settings:", error);
  }
});
</script>

<template>
  <div>
    <!-- Loading state -->
    <div v-if="isLoading" class="flex items-center justify-center h-screen">
      <p>Loading...</p>
    </div>

    <!-- Error state -->
    <div v-else-if="hasError" class="flex items-center justify-center h-screen">
      <p>Error loading settings. Please try again later.</p>
    </div>

    <!-- Main content -->
    <div v-else class="h-screen relative">
      <!-- Background container -->

      <div class="relative z-10 pr-5 bg-transparent">
        <Drawer />
      </div>
      <div
        class="info flex flex-col items-center justify-center h-screen relative"
      >
        <div class="text-left p-1 titleText">
          <div
            id="titleHome"
            class="titleText left-[50%] translate-Y-[-30%] absolute translate-x-[-50%] z-10000 top-[65%] xl:top-[65%] lg:top-[75%] md:top-[75%] sm:top-[80%]"
          >
            <h2>
              <span class="text-[32vw]">Judith</span>
            </h2>
            <h2 class="mt-[10vh]">
              <span class="text-[10vw]">Bosmans</span>
            </h2>
          </div>

          <!-- <Floating :ColorMode="ColorMode.preference" :modelPath="modelPath" /> -->
          <!-- <Flower class="z-100000" /> -->
          <About id="about" class="w-[100vw] absolute top-[150vh] left-0" />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
@keyframes blink {
  0%,
  100% {
    border-color: transparent;
  }
  50% {
    border-color: white;
  }
}

.animate-blink {
  animation: blink 0.7s step-end infinite;
}

/* Blurred text styling */
.blur-text {
  position: absolute; /* Place the blurred text behind the original */
  top: 0;
  left: 0;
  color: black; /* Black text for contrast */
  opacity: 0.4; /* Adjust for a subtle blur */
  filter: blur(8px); /* Apply Gaussian blur */
  z-index: -1; /* Ensure it's below the main text */
}
</style>
