<script setup>
const menuitems = [
  {
    title: "About",
    url: "https://dvnphysio.netlify.app/about",
  },
  {
    title: "Contact Us",
    url: "https://dvnphysio.netlify.app/contact",
  },
];
</script>

<template>
  <Container>
    <header class="flex flex-row flex-wrap items-center justify-between my-4 gap-x-6 gap-y-4">
      <div class="flex items-center justify-between">
        <a href="/" class="flex items-center space-x-2">
          <img src="/favicon.ico" alt="DVN Physio Logo" class="h-12" />
          <span> class="text-green-500" Devon Stroke and Neuro Physio</span>
        </a>
      </div>
      <nav class="flex w-auto">
        <ul class="flex flex-row gap-3 text-sm">
          <li v-for="item of menuitems">
            <a :href="item.url" class="flex px-3 py-2 text-gray-600 border rounded-sm hover:text-gray-800">
              {{ item.title }}
            </a>
          </li>
        </ul>
      </nav>
    </header>
  </Container>
</template>
