<script setup>
let currentYear = new Date().getFullYear();
let name = "Bilawal Mehfooz";
</script>
<template>
  <footer class="w-full px-4 md:px-0">
    <div
      class="flex flex-col md:flex-row items-center justify-between leading-relaxed"
    >
      <div class="w-full md:w-1/2 text-center md:text-left">
        <p class="font-semibold">©{{ currentYear }} {{ name }}</p>
        <p class="text-slate-700">
          Developed with &#x2764;&#xfe0f; by <a href="https://khawarmehfooz.com" class="hover:underline text-gray-900">Khawar Mehfooz</a>
        </p>
      </div>
      <div class="w-full md:w-1/2 text-center md:text-right mt-4 md:mt-0">
        <p class="font-semibold">Get in touch</p>
        <p class="text-slate-700">
          <a
            href="https://github.com/aschmelyun"
            target="_blank"
            rel="noopener"
            class="hover:underline text-slate-700 hover:text-gray-900"
            >Email</a
          >
          <span class="text-slate-300">&nbsp;—&nbsp;</span>
          <a
            href="https://linkedin.com/"
            target="_blank"
            rel="noopener"
            class="hover:underline text-slate-700 hover:text-gray-900"
            >LinkedIn</a
          >
          <span class="text-slate-300">&nbsp;—&nbsp;</span>
          <a
            href="https://twitter.com/"
            target="_blank"
            rel="noopener"
            class="hover:underline text-slate-700 hover:text-gray-900"
            >Twitter</a
          >
        </p>
      </div>
    </div>
  </footer>
</template>
