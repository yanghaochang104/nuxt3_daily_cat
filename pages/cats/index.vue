<template>
  <div>
    <h1>Cat-binet</h1>
    <div v-for="(cat, index) in cats" :key="cat.id">
      <nuxt-link :to="'cats/' + cat.id">
        <img
          :src="cat.url"
          :width="400"
          :height="(cat.height * 400) / cat.width"
        />
      </nuxt-link>
    </div>
  </div>
</template>
<script setup>
useHead({
  title: "Cat-binet",
  viewport: "width=device-width, initial-scale=1, maximum-scale=1",
  charset: "utf-8",
  meta: [
    {
      hid: "description",
      name: "description",
      content: "cat, cat and ... more cats！",
    },
  ],
});
const { data: cats } = await useFetch(
  "https://api.thecatapi.com/v1/images/search?limit=5&page=10&order=desc"
);
</script>
