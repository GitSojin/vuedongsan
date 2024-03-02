<template>
  <div class="menu">
    <a v-for="작명 in 메뉴들" :key="작명">{{ 작명 }}</a>
  </div>
  <div v-for="(item, index) in products" :key="index">
    <h4 class="blue" :style="color">{{ item.product }} 원룸</h4>
    <p>{{ item.price }} 만원</p>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      스타일: "color:blue",
      메뉴들: ["Home", "Shop", "About"],
      products: [
        { product: "역삼동원룸", price: 50 },
        { product: "천호동원룸", price: 60 },
        { product: "마포구원룸", price: 70 },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding: 10px;
}
</style>
