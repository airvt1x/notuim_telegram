<script setup lang="ts">
definePageMeta({
  layout: 'auth',
  middleware: 'sign-in'
});

useSeoMeta({
  title: 'Login | Notium'
});
</script>

<template>
  <div class="container relative h-dvh">
    <div class="mx-auto flex h-full w-full flex-col items-center justify-center">
      <div class="flex flex-col space-y-2 text-center">
        <h1 class="text-2xl font-semibold tracking-tight dark:text-zinc-100">Welcome back</h1>
        <p class="pb-4 text-sm text-[#72717a] dark:text-zinc-200">
          Enter your info below to sign in your account
        </p>
        <AuthForm />
        <AuthLine />
        <AuthGithub />
        <AuthPolicy />
      </div>
    </div>
  </div>
</template>
