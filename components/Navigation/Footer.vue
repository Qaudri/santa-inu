<template>
  <footer class="">
    <div class="max-w-7xl container mx-auto px-6 py-8 gap-4 md:gap-8 grid place-items-center md:flex items-center justify-center">
      <div class="flex gap-8">
        <NuxtLink to="https://t.me/santainu1only" class="group h-12 w-12 text-white focus:text-white hover:text-white bg-primary hover:bg-secondary focus:outline-primary font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTelegram class="w-7 h-7 text-white " />
        </NuxtLink>
        <NuxtLink to="https://twitter.com/santainuch/" class="group h-12 w-12 text-black focus:text-white hover:text-white bg-primary hover:bg-secondary focus:outline-primary font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTwitter class="w-7 h-7 text-white" />
        </NuxtLink>
      </div>
      <UiTypographyP class="mt-2">&copy; Santa Inu, {{new Date().getFullYear()}}</UiTypographyP>
    </div>
  </footer>
</template>