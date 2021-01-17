<template>
  <section class="w-full py-16 bg-white flex items-center justify-center shadow-inner">
    <div class="container items-center justify-center max-w-6xl px-5 md:px-16 xl:px-10">
      <div class="flex flex-col items-center lg:flex-row">
          <div class="flex flex-col items-start justify-center w-full h-full mb-10 lg:mb-0 lg:w-1/2">
            <p class="testimonial--subheading">
              Our customers love our product
            </p>
            <h3 class="testimonial--heading">
              What they say about us
            </h3>
            <p class="testimonial--description">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            </p>
          </div>
          <div class="w-full lg:w-1/2 space-y-4">
            <blockquote
              v-for="{ message, name, jobTitle, id } in testimonials"
              :key="id"
              class="quote--container"
            >
              <div class="flex flex-col">
                <div class="relative pl-12">
                  <svg class="absolute left-0 w-10 h-10 text-primary fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 125">
                    <path d="M30.7 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2C12.7 83.1 5 72.6 5 61.5c0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S30.7 31.6 30.7 42zM82.4 42c0 6.1 12.6 7 12.6 22 0 11-7.9 19.2-18.9 19.2-11.8 0-19.5-10.5-19.5-21.6 0-19.2 18-44.6 29.2-44.6 2.8 0 7.9 2 7.9 5.4S82.4 31.6 82.4 42z" />
                  </svg>
                  <p class="quote--message">{{ message }}</p>
                </div>

                <h3 class="quote--name">
                  {{ name }}
                  <span class="quote--job">- {{ jobTitle }}</span>
                </h3>
              </div>
            </blockquote>
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

<style lang="postcss" scoped>
.testimonial--heading {
  @apply text-3xl font-extrabold leading-10 tracking-tight text-accent;

  @screen sm {
    @apply text-5xl leading-none;
  }

  @screen md {
    @apply text-6xl;
  }

  @screen lg {
    @apply text-5xl;
  }

  @screen xl {
    @apply text-6xl;
  }
}

.testimonial--subheading {
  @apply mb-2 text-base font-medium tracking-tight text-primary;
}

.testimonial--description {
  @apply my-6 text-base text-gray-500;
}

.quote--container {
  @apply flex items-center justify-between w-full col-span-1 p-6 bg-white rounded-lg shadow-xl;
}

.quote--container .quote--message {
  @apply mt-2 text-sm text-gray-600 whitespace-normal;

  @screen sm {
    @apply text-base;
  }

  @screen lg {
    @apply text-sm;
  }

  @screen xl {
    @apply text-base;
  }
}

.quote--container .quote--name {
  @apply pl-12 mt-3 text-sm font-medium leading-5 text-gray-800 truncate;

  @screen sm {
    @apply text-base;
  }

  @screen lg {
    @apply text-sm;
  }
}

.quote--container .quote--name>.quote--job {
  @apply mt-1 text-sm leading-5 text-gray-500 whitespace-normal;
}
</style>
