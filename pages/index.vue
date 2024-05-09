<template>
  <nav class="bg-blue-800 p-4">
    <div class="container mx-auto flex items-center justify-between">
      <div class="logo">
        <nuxt-link to="/" class="text-white text-4xl font-bold"><span
            class="text-white text-4xl font-bold">KRIZIA'S</span> TRAVEL BLOG</nuxt-link>
      </div>
      <input type="checkbox" id="menu-toggle" class="hidden" />
      <label for="menu-toggle" class="menu-icon text-white text-2xl cursor-pointer md:hidden">&#9776;</label>
      <ul class="menu hidden md:flex space-x-6">
        <li><nuxt-link to="/" class="text-white hover:text-gray-200">Home</nuxt-link></li>
        <li><nuxt-link to="/about" class="text-white hover:text-gray-200">Aboutus</nuxt-link></li>
        <li><nuxt-link to="/blog" class="text-white hover:text-gray-200">Blog</nuxt-link></li>
        <li><nuxt-link to="/bookings" class="text-white hover:text-gray-200">Bookings</nuxt-link></li>
        <li><nuxt-link to="/help" class="text-white hover:text-gray-200">Help</nuxt-link></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  mounted() {
    const menuToggle = document.getElementById('menu-toggle');
    const menu = document.querySelector('.menu');

    menuToggle.addEventListener('change', () => {
      menu.classList.toggle('hidden');
      menu.classList.toggle('flex');
      menu.classList.toggle('flex-col');
      menu.classList.toggle('md:flex-row');
      menu.classList.toggle('md:space-x-6');
      menu.classList.toggle('mt-4');
      menu.classList.toggle('md:mt-0');
    });
  },
};
</script>

<style scoped></style>