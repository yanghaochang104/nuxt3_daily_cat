<template>
  <header class="header">
    <div class="title-container">
      <h1 class="title">Word of Cats</h1>
      <h3 class="subtitle">Make Everyday Your Caturday</h3>
    </div>
    <ul>
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/cats">Cats</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about">About</nuxt-link>
      </li>
    </ul>
  </header>
</template>
<script>
export default {
  name: "Header",
};
</script>
<style>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
  padding-left: 1rem;
  padding-right: 1rem;
  border-bottom: 1px dotted #ccc;
}
.header .title {
  font-size: 3rem;
  color: #526488;
}

.header ul {
  display: flex;
}

.header a {
  display: inline-block;
  background: #333;
  color: #fff;
  padding: 0.3rem 1rem;
  margin-right: 0.5rem;
}

.title-container {
  display: flex;
  flex-direction: column;
}

.subtitle {
  color: #949494;
}
</style>
