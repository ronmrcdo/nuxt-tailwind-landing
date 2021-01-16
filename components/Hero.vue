<template>
  <section class="hero md:px-0">
    <div class="container items-center max-w-6xl px-5 mx-auto space-y-6 text-center;">
      <h1 class="text-4xl font-extrabold tracking-tight text-accent text-left sm:text-5xl md:text-6xl md:text-center">
        <span class="block">Level up your <span class="block text-gradient bg-gradient-to-r from-blue-600 via-indigo-400 to-purple-300 lg:inline lg:mt-0 mt-1">Website</span></span>
      </h1>
      <p class="w-full mx-auto text-base text-left text-gray-500 md:max-w-md sm:text-lg lg:text-2xl md:text-center">
        Anim aute id magna aliqua ad ad non deserunt sunt.
      </p>
      <div class="relative flex flex-col justify-center md:flex-row md:space-x-4">
        <a href="#" class="flex items-center w-full px-6 py-3 mb-3 text-lg text-white bg-primary shadow-primary rounded-md md:mb-0 hover:bg-blue-600 border-blue-600 md:w-auto">
          Get Started
        </a>
        <a href="#" class="flex items-center px-6 py-3 text-gray-500 bg-gray-100 rounded-md hover:bg-gray-200 hover:text-gray-600">
          Learn more
        </a>
      </div>
    </div>
    <div class="container items-center max-w-4xl px-5 mx-auto mt-16 text-center">
      <img src="~/assets/images/hero.svg" alt="Hero">
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style lang="postcss" scoped>
.hero {
  @apply px-2 pt-32 pb-10 bg-white;
}

</style>
