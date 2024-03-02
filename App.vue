<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div v-for="(product,index) in products" :key="index">
    <h4 class="blue" :style=color>{{ product }} 원룸</h4>
    <p>{{ price1 }} 만원</p>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      price1: 50,
      스타일: "color:blue",
      products : ['역삼동원룸','천호동원룸','마포구원룸']
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
  margin-top: 60px;
}
</style>