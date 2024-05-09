<template>

  <main>
    <slot />
  </main>
  <nav class="bg-white shadow-md flex justify-between items-center px-4 py-2">

    <button @click="toggleMenu" class="md:hidden focus:outline-none">
      <svg class="h-6 w-6 text-gray-800" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M4 6H20M4 12H20M4 18H11M13 18H20" stroke="currentColor" stroke-width="2" stroke-linecap="round"
          stroke-linejoin="round"></path>
      </svg>
    </button>
  </nav>



</template>

<script setup>

</script>

<style scoped></style>