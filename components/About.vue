<template>
  <main class="flex items-center justify-center h-[70vh]">
    <section class="w-[85%] px-6">
      <div class="flex items-center justify-between flex-wrap md:flex-nowrap">
        <!-- Image Section -->
        <div class="flex items-center justify-center flex-col w-30%">
          <img
            src="/img/profile.png"
            alt="Profile Picture"
            class="rounded-full w-[180px] h-[180px] object-cover"
          />
          <div class="bodyText text-left">
            <p>
              Developer <br />
              Designer
            </p>
          </div>
        </div>

        <!-- Description Section -->
        <div
          class="flex flex-col space-y-4 md:flex-grow min-w-[45vw] max-w-[55vw]"
        >
          <p class="bodyText text-left text-base mb-[2vh] w-[50vw]">
            Lorem ipsum dolor sit amet. Qui modi illum ab quod optio est
            exercitationem aliquid et consequatur quibusdam sed sint ipsa. Sed
            consequuntur repellendus vel perferendis rerum ad officia architecto
            aut quos nostrum sed accusantium repellat. Sit facilis fuga qui
            officiis laborum non fuga quasi? Aut officia illum aut voluptas
            doloribus eos voluptatum fugiat aut facilis sint et modi vitae.
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
              Adobe Suite
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
          </ul>
        </div>
      </div>
    </section>
  </main>
</template>
