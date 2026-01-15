<script setup lang="ts">
import Highlight from "~/components/Highlight.vue";
import Service from "~/components/Service.vue";

useHead({
  title: "PT. Ady Trans Jaya - Jasa Transportasi",
  meta: [
    {
      name: "description",
      content:
        "PT. Ady Trans Jaya menyediakan jasa transportasi barang profesional dan terpercaya",
    },
    {
      name: "robots",
      content: "index, follow",
    },
    {
      property: "og:title",
      content: "PT. Ady Trans Jaya - Jasa Transportasi",
    },
    {
      property: "og:description",
      content: "Jasa transportasi barang profesional dan terpercaya di Indonesia",
    },
    {
      property: "og:type",
      content: "website",
    },
  ],
});
</script>

<template>
  <Hero />
  <Highlight />
  <Service />
</template>
