<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavItem from './components/NavItem.vue'
import MenuIcon from 'vue-material-design-icons/Menu.vue'
import logo from '@/assets/logo-noel.svg'
</script>

<template>
  <header
    class="relative mx-auto flex items-center justify-between border-b-[1px] border-solid border-[#F1F1F1] p-3"
  >
    <h1>
      <img :src="logo" alt="logo" />
    </h1>
    <div>
      <MenuIcon fillColor="black" :size="30" class="text-center" />
    </div>
    <nav
      class="absolute bottom-0 left-0 right-0 top-full mx-auto flex w-full flex-col p-7 text-center"
    >
      <RouterLink class="group" to="/">
        <NavItem item-text="首頁" />
      </RouterLink>
      <RouterLink class="group" to="/">
        <NavItem item-text="作品集" />
      </RouterLink>
      <RouterLink class="group" to="/">
        <NavItem item-text="服務項目" />
      </RouterLink>
      <RouterLink class="group" to="/">
        <NavItem item-text="部落格" />
      </RouterLink>
      <RouterLink class="group" to="/">
        <NavItem item-text="聯絡我" />
      </RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped></style>
