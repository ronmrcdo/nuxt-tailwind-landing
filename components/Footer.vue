<template>
  <footer class="relative shadow-inner bg-gray-50 pt-16 pb-6">
    <div class="container mx-auto md:flex-row max-w-7xl">
      <div class="w-full flex flex-wrap justify-between items-start mb-10">

        <div class="w-full lg:w-6/12 px-4">
          <div class="w-1/2">
            <a href="#_" class="relative z-10 flex items-center w-auto text-2xl font-extrabold leading-none text-accent select-none">
              starter.
            </a>
          </div>
          <div class="my-2">
            <h5 class="text-md my-0 text-gray-400">A starter landing page using nuxt and tailwindcss.</h5>
          </div>
        </div>

        <div class="w-full lg:w-4/12 px-4">
          <div class="w-full flex-wrap flex justify-between items-start">

            <div class="w-full lg:w-6/12 ml-auto">
              <ul class="list-none text-md text-gray-400">
                <li class="mb-2 font-semibold uppercase block">
                  Links
                </li>
                <li class="mb-2 block">
                  About us
                </li>
                <li class="mb-2 block">
                  Services
                </li>
                <li class="mb-2 block">
                  Portfolio
                </li>
              </ul>
            </div>

            <div class="w-full lg:w-6/12 ml-auto">
              <ul class="list-none text-md text-gray-400">
                <li class="mb-2 font-semibold uppercase block">
                  Resources
                </li>
                <li class="mb-2 block">
                  Terms and Conditions
                </li>
                <li class="mb-2 block">
                  Privacy Policy
                </li>
              </ul>
            </div>

          </div>
        </div>

      </div>
      <hr class="my-6 border-gray-200 shadow-sm" />
      <div class="w-full flex flex-wrap items-center md:justify-between justify-center">
        <div class="w-full px-4 mx-auto text-center text-gray-400">
          Copyright © 2021 Starter, Inc. All rights reserved.
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>
