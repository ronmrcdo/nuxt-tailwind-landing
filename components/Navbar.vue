<template>
  <header class="relative w-full px-8 text-gray-700 bg-white body-font">
    <div
      class="container flex flex-col flex-wrap items-center justify-between py-5 mx-auto md:flex-row max-w-7xl"
    >
      <a
        href="#_"
        class="text--logo text-gradient bg-gradient-to-r from-blue-600 via-indigo-400 to-purple-300"
      >
        starter.
      </a>

      <div class="relative z-10 inline-flex items-center space-x-3 md:ml-5 lg:justify-end">
        <nav class="hidden md:block">
          <div class="flex items-baseline space-x-10">
            <a
              href="#_"
              class="item--link"
            >
              <span class="block">Home</span>
            </a>

            <a
              href="#_"
              class="item--link"
            >
              <span class="block">Services</span>
            </a>

            <a
              href="#_"
              class="item--link"
            >
              <span class="block">Portfolio</span>
            </a>

            <span class="inline-flex rounded-md shadow-sm">
              <a
                href="#"
                class="btn btn--primary text-white shadow-primary whitespace-no-wrap "
              >
                Contact Us
              </a>
            </span>
          </div>
        </nav>

      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style lang="postcss" scoped>
.text--logo {
  @apply relative z-10 flex items-center w-auto text-2xl font-extrabold leading-none select-none;
}

nav .item--link {
  @apply relative font-medium leading-6 mx-2 text-gray-600 transition duration-150 ease-out;
}

nav .item--link:hover {
  @apply text-gray-900;
}

.btn {
  @apply inline-flex items-center justify-center;
  @apply px-4 py-2 text-base font-medium leading-6 rounded-md;
  @apply transition duration-150 ease-out;
}

.btn.btn--primary {
  @apply bg-primary border border-primary;
}

.btn.btn--primary:hover {
  @apply bg-blue-600 border-blue-600;
}

.btn.btn--primary:focus {
  @apply outline-none ring-2 ring-offset-2 ring-blue-500;
}

.btn.btn--outline {
  @apply bg-white border border-gray-200 shadow-sm;
}

.btn.btn--outline:hover {
  @apply bg-gray-50;
}

.btn.btn--outline:focus {
  @apply outline-none shadow-none;
}
</style>
