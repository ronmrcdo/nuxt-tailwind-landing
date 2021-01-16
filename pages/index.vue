<template>
  <div>
    <Hero />

    <section class="py-20 bg-gray-50 shadow-inner">
      <div class="px-4 mx-auto text-center max-w-7xl sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold tracking-tight text-accent sm:text-4xl md:text-5xl xl:text-6xl">
          Built exclusively for you
        </h2>
        <p class="max-w-md mx-auto mt-3 text-base text-gray-500 sm:text-lg md:mt-5 md:text-xl md:max-w-3xl">
          Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.
        </p>
      </div>

      <div class="container max-w-6xl mx-auto">
        <div class="grid grid-cols-4 gap-8 mt-10 sm:grid-cols-4 lg:grid-cols-12 sm:px-8 xl:px-0">
          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 " viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <path d="M14 3v4a1 1 0 0 0 1 1h4" />
                <path d="M5 8v-3a2 2 0 0 1 2 -2h7l5 5v11a2 2 0 0 1 -2 2h-5" />
                <circle cx="6" cy="14" r="3" />
                <path d="M4.5 17l-1.5 5l3 -1.5l3 1.5l-1.5 -5" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
              Sed ut perspiciatis
            </h4>
            <p class="text-base text-center text-gray-500">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            </p>
          </div>

          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 " viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <path d="M14 3v4a1 1 0 0 0 1 1h4" />
                <path d="M5 8v-3a2 2 0 0 1 2 -2h7l5 5v11a2 2 0 0 1 -2 2h-5" />
                <circle cx="6" cy="14" r="3" />
                <path d="M4.5 17l-1.5 5l3 -1.5l3 1.5l-1.5 -5" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
              Ut enim ad minim veniam
            </h4>
            <p class="text-base text-center text-gray-500">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            </p>
          </div>

          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8 " viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <path d="M14 3v4a1 1 0 0 0 1 1h4" />
                <path d="M5 8v-3a2 2 0 0 1 2 -2h7l5 5v11a2 2 0 0 1 -2 2h-5" />
                <circle cx="6" cy="14" r="3" />
                <path d="M4.5 17l-1.5 5l3 -1.5l3 1.5l-1.5 -5" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
              Excepteur sint occaecat
            </h4>
            <p class="text-base text-center text-gray-500">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            </p>
          </div>
        </div>
      </div>
    </section>

    <Testimonials :testimonials="testimonials"/>

    <CallAction />
  </div>
</template>

<script>
import Hero from '~/components/Hero.vue';
import Testimonials from '~/components/Testimonials.vue';
import CallAction from '~/components/CallAction.vue';

export default {
  components: {
    Hero,
    Testimonials,
    CallAction
  },
  data: () => ({
    testimonials: [
      {
        id: 1,
        name: 'James Durant',
        jobTitle: 'Owner, Steak House',
        message: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium'
      },
      {
        id: 2,
        name: 'Christopher Buddy',
        jobTitle: 'CEO, HouseDesign Ltd.',
        message: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium'
      },
      {
        id: 3,
        name: 'Alphonse Todd',
        jobTitle: 'CTO, MarketplaceDesign Inc.',
        message: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium'
      }
    ]
  })
}
</script>
