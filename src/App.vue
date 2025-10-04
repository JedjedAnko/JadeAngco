<template>
  <Suspense>
    <UApp>
      <UHeader>
        <template #left>
          <RouterLink to="/">
            <h1>Jade Angco - UI/UX Designer & Frontend Developer</h1>
          </RouterLink>
        </template>

        <template #right>
          <UColorModeButton />

          <!-- <UButton
            to="https://github.com/JedjedAnko"
            target="_blank"
            icon="simple-icons:github"
            aria-label="GitHub"
            color="neutral"
            variant="ghost"
          /> -->
        </template>
      </UHeader>

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
