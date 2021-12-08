<template>
  <div class="products">
    <div class="cards">
      <div class="card" v-for="product in products" :key="product.id">
        <img src="../assets/product1.jpg" alt="img_product" />
        <div class="card-body">
          <h3>{{ product.productName }}</h3>
          <span class="price">Rp 19.000</span>
          <span class="discountPrice">Rp 8.000</span>
          <p>Kota Bandung</p>
        </div>
      </div>
    </div>
    <div class="pagination">
      <a href="/">Previous</a>
      <a href="/">Next</a>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const products = ref([
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
      {
        id: 1,
        productName: "Sepatu 1",
        img: "../assets/product1.jpg",
        price: "200.000",
        discount: "185.000",
        cityName: "Kota Bandung",
      },
    ]);

    return { products };
  },
};
</script>

<style scoped>
.cards {
  margin: 25px 40px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}

.card {
  border-radius: 10px;
  box-shadow: 1px 2px 3px rgba(0, 0, 0, 0.2);
  width: 250px;
  margin: 25px;
}

img {
  width: 100%;
  border-radius: 10px;
}

.card-body {
  padding: 10px;
}

span {
  margin-right: 10px;
}

.price {
  text-decoration: line-through;
}

.pagination {
  display: flex;
  justify-content: end;
  margin: 25px 88px;
}

a {
  margin: 0 5px;
  text-decoration: none;
  border: 1px solid black;
  padding: 10px 20px;
  color: black;
}
</style>