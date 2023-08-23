<template>
  <div class="flex flex-col">
    <div v-for="route in router.getRoutes()" :key="route.path">
      <nuxt-link :to="route.path">{{ route.name }}</nuxt-link>
    </div>
  </div>
</template>

<script setup>
const router = useRouter()
</script>
