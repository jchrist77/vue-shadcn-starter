<script setup lang="ts">
import ModeToggle from '@/components/ModeToggle.vue'
import ThemePicker from '@/components/ThemePicker.vue'
import { Button } from "@/components/ui/button"
</script>

<template>
  <header class="fixed flex flex-row w-full h-16 px-4 gap-6 bg-background/80 text-base-content shadow-sm items-center">
    <div class="flex">
      <router-link to="/" class="text-xl flex items-center">
        <img src="@/assets/vue.svg" />
        Vue3 Starter
      </router-link>
    </div>

    <div class="flex-1 align-center">
      <ul class="text-xl flex flex-row gap-6">
        <li><router-link to="/" active-class="bg-base-300 font-bold">Home</router-link></li>
        <li><router-link to="/users" active-class="bg-base-300 font-bold">Users</router-link></li>
        <li><router-link to="/login" active-class="bg-base-300 font-bold">Login</router-link></li>
      </ul>
    </div>

    <div class="text-lg flex align-center gap-6">
      <ModeToggle />
    </div>
  </header>
</template>
