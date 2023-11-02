<template>
  <footer class="bg-secondary">
    <div class="max-w-7xl container mx-auto px-6 py-8 gap-8 grid place-items-center md:flex items-center justify-center">
      <div class="flex gap-8">
        <NuxtLink to="https://t.me/Mickyratbsc" class="group h-12 w-12 text-black focus:text-white hover:text-white bg-secondary hover:bg-primary focus:outline-primary border-primary border font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTelegram class="w-7 h-7 text-black group-hover:text-white duration-300 ease-in-out" />
        </NuxtLink>
        <NuxtLink to="https://t.me/Mickyratbsc" class="group h-12 w-12 text-black focus:text-white hover:text-white bg-secondary hover:bg-primary focus:outline-primary border-primary border font-medium text-base 2xl:text-lg justify-center duration-300 ease-in-out rounded-md outline-none focus:outline-none flex items-center gap-4">
          <IconsTwitter to="https://twitter.com/rat_micky55647" class="w-7 h-7 text-black group-hover:text-white duration-300 ease-in-out" />
        </NuxtLink>
      </div>
      <UiTypographyP class="mt-2">&copy; Micky Rat, {{new Date().getFullYear()}}</UiTypographyP>
    </div>
  </footer>
</template>