<script setup lang="ts">
import { ref } from 'vue';

import mobicartLogo from '../../assets/mobicart-without-bg.png';

interface IMenuItem {
  text: string
  to: string
}

const menu = ref<Array<IMenuItem>>([
  {
    text: "Início",
    to: "#"
  },
  {
    text: "Sobre",
    to: "#sobre"
  },
  {
    text: "Contato",
    to: "#contato"
  }
])

</script>

<template>
  <header class="w-full flex items-center bg-black gap-3">
    <div class="">
      <img class="w-12 animate-pulse skew-y-6" :src="mobicartLogo" />
    </div>
    <aside class="flex items-center justify-evenly w-full font-semibold text-amber-400">
      <a v-for="item of menu" :key="item.to" :href="item.to" class="hover:underline" >
        {{ item.text }}
      </a>
    </aside>
  </header>
</template>
