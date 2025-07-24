<template>
  <section class="p-8 bg-white">
    <h2 class="text-2xl font-bold mb-6 text-center">আমাদের সেবাসমূহ</h2>
    <div class="grid grid-cols-1 sm:grid-cols-3 md:grid-cols-6 gap-6">
      <div v-for="service in services" :key="service.id" class="border rounded p-4 text-center shadow hover:shadow-lg transition">
        <img :src="service.icon" alt="" class="mx-auto mb-2 h-12 w-12" />
        <h3 class="font-semibold">{{ service.title }}</h3>
        <p class="text-sm text-gray-600">{{ service.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const services = [
  {
    id: 1,
    title: "myGov",
    description: "সরকারের সেবা",
    icon: "/public/file.svg"
  },
  {
    id: 2,
    title: "GRS",
    description: "গভর্নমেন্ট রিকর্ড সিস্টেম",
    icon: "/public/file.svg"
  },
  {
    id: 3,
    title: "আয়কর রিটার্ন",
    description: "ট্যাক্স রিটার্ন সেবা",
    icon: "/public/file.svg"
  },
  {
    id: 4,
    title: "বাংলাদেশ পাসপোর্ট সেবা",
    description: "পাসপোর্ট আবেদন",
    icon: "/public/file.svg"
  },
  {
    id: 5,
    title: "সরকারি নিয়োগ বিজ্ঞপ্তি",
    description: "নিয়োগ বিজ্ঞপ্তি",
    icon: "/public/file.svg"
  },
  {
    id: 6,
    title: "বিলিং ও কর্পোরেট",
    description: "বিলিং সেবা",
    icon: "/public/file.svg"
  }
]
</script>

<style scoped>
</style>
