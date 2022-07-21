<template>
  <h1>I am a big fat cat</h1>
  <img src="@/assets/fat_cat.jpeg" alt="fat-cat" />
</template>
<script>
export default {
  head() {
    return {
      title: "Daily Cat",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "a cat a day saves doctor away",
        },
      ],
    };
  },
};
</script>
