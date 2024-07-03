<script setup lang="ts">
import About from "./components/about.vue";
import Footer from "./components/footer.vue";
import Header from "./components/header.vue";
import Main from "./components/main.vue";
</script>

<template>
  <div class="relative container flex flex-col items-center gap-10 w-full bg-black m-auto rounded-md h-full text-white px-4 scroll-smooth">

    <Header id="#" class="sticky top-0 left-0 right-0" />
    <Main class="" />
    <About id="sobre" />
    <Footer id="contato" />
  </div>
</template>
