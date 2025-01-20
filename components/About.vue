<template>
  <main class="flex items-center justify-center h-[70vh]">
    <section class="w-[85%] px-6">
      <div class="flex items-center justify-between flex-wrap md:flex-nowrap">
        <!-- Image Section -->
        <div class="flex items-center justify-center flex-col w-30%">
          <img
            src="/img/profile.png"
            alt="Profile Picture"
            class="rounded-full w-[200px] h-[200px] object-cover"
          />
        </div>

        <!-- Description Section -->
        <div
          class="flex flex-col space-y-4 md:flex-grow min-w-[45vw] max-w-[55vw]"
        >
          <p class="bodyText text-left text-base mb-[2vh] w-[50vw]">
            <span class="font-semibold">
              Student MIND @Luca and Developer @AKQA.
            </span>
            <br /><br />
            I’m passionate about combining creativity and technology to solve
            problems. With a strong foundation in design and development, I
            thrive on tackling challenges, building meaningful experiences, and
            continuously learning to grow in this dynamic field.
          </p>

          <!-- Skills List -->
          <ul class="bodyText grid grid-cols-2 gap-4 md:grid-cols-3">
            <li class="flex items-center space-x-5">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              HTML
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              CSS
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              JavaScript
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              Teamplayer
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              React & Vue
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              Adobe Suite & Figma
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              UX/UI
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              Growth Mindset
            </li>
            <li class="flex items-center space-x-2">
              <svg
                class="w-6 h-6 text-prettyRed mr-2"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
              >
                <path
                  d="M8.5 11.5L11 14l4-4m6 2a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                />
              </svg>
              Agile
            </li>
          </ul>
        </div>
      </div>
    </section>
  </main>
</template>
