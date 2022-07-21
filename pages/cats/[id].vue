<template>
  <div class="center-content">
    <h3>name: {{ id }}</h3>
    <img :src="data.url" />
    <div class="center-content row">
      <button
        style="background-color: transparent; border: none; cursor: pointer"
        @click="likeCount++"
      >
        <img src="@/assets/like_icon.png" width="40" height="40" />
      </button>
      <span style="font-size: 20px; margin-left: 5px">{{ likeCount }}</span>
    </div>
  </div>
</template>
<script setup>
const {
  params: { id },
} = useRoute();

const { data } = await useFetch(`https://api.thecatapi.com/v1/images/${id}`, {
  initialCache: false,
});

const likeCount = useState("likeCount", () => 0);
</script>
<style>
.center-content {
  display: flex;
  flex-direction: column;
  justify-self: center;
  align-items: flex-start;
}
.row {
  flex-direction: row;
  align-items: center;
}
</style>
