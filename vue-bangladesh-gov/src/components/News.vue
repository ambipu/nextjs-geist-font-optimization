<template>
  <section class="p-8 bg-gray-50">
    <h2 class="text-2xl font-bold mb-6 text-center">সর্বশেষ আপডেট</h2>
    <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
      <div v-for="newsItem in news" :key="newsItem.id" class="bg-white p-4 rounded shadow hover:shadow-lg transition">
        <img :src="newsItem.image" alt="" class="mb-4 rounded" />
        <h3 class="font-semibold mb-2">{{ newsItem.title }}</h3>
        <p class="text-sm text-gray-600">{{ newsItem.date }}</p>
      </div>
    </div>
    <div class="text-center mt-6">
      <button class="bg-govRed text-white px-6 py-2 rounded">আরও দেখুন</button>
    </div>
  </section>
</template>

<script setup>
const news = [
  {
    id: 1,
    title: "জাতীয় দুর্যোগ পরিকল্পনা ২০২১-২০২৫",
    date: "মে ১৪, ২০২৩",
    image: "/public/file.svg"
  },
  {
    id: 2,
    title: "জাতীয় দুর্যোগ পরিকল্পনা ২০২১-২০২৫",
    date: "মে ১৪, ২০২৩",
    image: "/public/file.svg"
  },
  {
    id: 3,
    title: "বাজেট (২০২২-২০২৩)",
    date: "মে ১৪, ২০২৩",
    image: "/public/file.svg"
  },
  {
    id: 4,
    title: "জাতীয় দুর্যোগ পরিকল্পনা ২০২১-২০২৫",
    date: "মে ১৪, ২০২৩",
    image: "/public/file.svg"
  }
]
</script>

<style scoped>
</style>
