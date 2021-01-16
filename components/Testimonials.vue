<template>
  <section class="py-16 bg-white min-w-screen flex items-center justify-center shadow-inner">
    <div class="max-w-6xl px-12 mx-auto md:px-16 xl:px-10">
      <div class="flex flex-col items-center lg:flex-row">
        <div class="flex flex-col items-center lg:flex-row">
          <div class="flex flex-col items-start justify-center w-full h-full mb-10 lg:mb-0 lg:w-1/2">
            <p class="mb-2 text-base font-medium tracking-tight text-primary">
              Our customers love our product
            </p>
            <h2 class="text-4xl font-extrabold leading-10 tracking-tight text-accent sm:text-5xl sm:leading-none md:text-6xl lg:text-5xl xl:text-6xl">
              What they say about us
            </h2>
            <p class="my-6 text-base text-gray-500">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            </p>
          </div>
          <div class="w-full lg:w-1/2 space-y-6">
            <blockquote
              v-for="{ message, name, jobTitle, id } in testimonials"
              :key="id"
              class="flex items-center justify-between w-full col-span-1 p-6 bg-white rounded-lg shadow-xl"
            >
              <div class="flex flex-col pr-8">
                <div class="relative pl-12">
                  <svg class="absolute left-0 w-10 h-10 text-indigo-500 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 125">
                    <path d="M30.7 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2C12.7 83.1 5 72.6 5 61.5c0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S30.7 31.6 30.7 42zM82.4 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2-11.8 0-19.5-10.5-19.5-21.6 0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S82.4 31.6 82.4 42z" />
                  </svg>
                  <p class="mt-2 text-sm text-gray-600 sm:text-base lg:text-sm xl:text-base">
                    {{ message }}
                  </p>
                </div>

                <h3 class="pl-12 mt-3 text-sm font-medium leading-5 text-gray-800 truncate sm:text-base lg:text-sm">
                  {{ name }}
                  <span class="mt-1 text-sm leading-5 text-gray-500 truncate">- {{ jobTitle }}</span>
                </h3>
              </div>
            </blockquote>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Testimonials',
  props: {
    testimonials: {
      type: Array,
      default: []
    }
  }
}
</script>
