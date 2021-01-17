<template>
  <section class="hero md:px-0">
    <div class="hero--container">
      <h1 class="hero--headings">
        <span class="block">Level up your <span class="block text-gradient bg-gradient-to-r from-blue-600 via-indigo-400 to-purple-300 lg:inline lg:mt-0 mt-1">Website</span></span>
      </h1>
      <p class="hero--description">
        Anim aute id magna aliqua ad ad non deserunt sunt.
      </p>
      <div class="hero--actions md:space-x-4">
        <a href="#" class="btn btn--primary">
          Get Started
        </a>
        <a href="#" class="btn btn--default">
          Learn more
        </a>
      </div>
    </div>
    <div class="hero--img-container">
      <img src="~/assets/images/hero.svg" alt="Build website">
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

.hero .hero--container {
  @apply container items-center max-w-6xl px-5 mx-auto space-y-6 text-center;
}

.hero .hero--headings {
  @apply text-4xl font-extrabold tracking-tight text-accent text-left;

  @screen sm {
    @apply text-5xl;
  }

  @screen md {
    @apply text-6xl text-center;
  }
}

.hero .hero--description {
  @apply w-full mx-auto text-base text-left text-gray-500;

  @screen sm {
    @apply text-lg;
  }

  @screen md {
    @apply max-w-md text-center;
  }

  @screen lg {
    @apply text-2xl;
  }
}

.hero .hero--actions {
  @apply relative flex flex-col justify-center;

  @screen lg {
    @apply flex-row space-x-4;
  }
}

.hero .hero--img-container {
  @apply container items-center max-w-4xl px-5 mx-auto mt-16 text-center;
}

.hero .btn {
  @apply px-6 py-3 mb-3 text-lg rounded-md;
}
</style>
