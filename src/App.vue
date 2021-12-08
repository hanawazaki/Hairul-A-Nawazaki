<script>
import ProductList from "./components/ProductList.vue";
export default {
  components: { ProductList },
};
</script>

<template>
  <div class="navbar">
    <ul class="nav">
      <li><a href="#">Home</a></li>
      <li><a href="#">Category</a></li>
      <li><a href="#">Category</a></li>
      <li><a href="#">Dropdown</a></li>
      <li><a href="#">Dropdown</a></li>
      <li><a href="#">Dropdown</a></li>
    </ul>
  </div>
  <ProductList />
</template>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.nav {
  display: flex;
  list-style: none;
  padding: 20px;
  background-color: #f44336;
}

li {
  margin: 0 10px;
}

li a {
  text-decoration: none;
  color: white;
}
</style>
