<template>
  <div class="home-container">
    <span>
      <h1 class="home-title">Daily Cat</h1>
    </span>
    <img src="@/assets/fat_cat.jpeg" alt="fat-cat" class="cat-img" />
    <span>
      <h3>I am a big big big fat cat ฅ (≈ >ܫ&lt; ≈) ฅ</h3>
    </span>
  </div>
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
<style>
.home-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.home-title {
  color: #526488;
}
</style>
