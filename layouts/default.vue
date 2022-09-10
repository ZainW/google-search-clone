<script setup lang="ts">
import { Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
</script>

<template>
  <main>
    <nav class="flex justify-between mx-5 my-3">
      <div class="gap-2">
        <a href="#">
          About
        </a>
        <a href="#">
          Store
        </a>
      </div>
      <div flex justify="center" content="center" class="gap-2">
        <a href="#">
          Gmail
        </a>
        <a href="#">
          Images
        </a>
        <Menu>
          <MenuButton>
            <div i-ic-baseline-apps bg-light-200 />
          </MenuButton>
          <MenuItems class="z-50">
            <MenuItem>
              <a href="#">
                Account settings
              </a>
            </MenuItem>
            <MenuItem>
              <a href="#">
                Documentation
              </a>
            </MenuItem>
          </MenuItems>
        </menu>
      </div>
    </nav>
    <slot />
  </main>
</template>
