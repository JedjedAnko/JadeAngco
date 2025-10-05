<template>
  <Suspense>
    <UApp>
      <header
        class="flex items-center justify-between p-4 sticky top-0 bg-background/90 backdrop-blur z-10"
      >
        <RouterLink to="/" class="text-xs sm:text-xl">
          Jade Angco - UI/UX Designer & Frontend Developer
        </RouterLink>

        <div class="flex items-center gap-2">
          <UButton
            to="https://www.instagram.com/adi.adept/"
            target="_blank"
            icon="mdi:instagram"
            variant="ghost"
          />
          <UButton
            to="https://www.facebook.com/Adi.Adept/"
            target="_blank"
            icon="mdi:facebook"
            variant="ghost"
          />
          <UButton to="mailto:jedboyjabagat@gmail.com" icon="mdi:email" variant="ghost" />
          <UColorModeButton />
        </div>
      </header>

      <UMain>
        <RouterView />
      </UMain>

      <USeparator icon="simple-icons:vuedotjs" />

      <UFooter>
        <template #left>
          <p class="text-sm text-muted">
            Built with Nuxt UI • © {{ new Date().getFullYear() }}
          </p>
        </template>
      </UFooter>
    </UApp>
  </Suspense>
</template>
