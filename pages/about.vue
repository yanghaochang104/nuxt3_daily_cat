<template>
  <div>
    <h1 class="about-title">About</h1>
    <p>興趣使然的愛貓工程師</p>
  </div>
</template>
<script setup>
useHead({
  title: "About the App",
  meta: [
    {
      hid: "description",
      name: "description",
      content: "stories about web engineer and cats",
    },
  ],
});
</script>
<style>
.about-title {
  color: #526488;
}
</style>
