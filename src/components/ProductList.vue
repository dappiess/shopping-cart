<template>
  <div class="row">
    <div
      class="card"
      style="width: 12rem"
      v-for="item in products"
      :key="item.id"
    >
      <img :src="item.imgUrl" class="card-img-top" :alt="item.tittle" />
      <div class="card-body">
        <p class="card-title">{{ item.tittle }}</p>
        <p class="card-text">$ {{ item.price }}</p>
        <a href="#" class="btn btn-primary">Add to cart</a>
      </div>
    </div>
  </div>
</template>

<script>
import { mapGetters, mapActions } from "vuex";

export default {
  name: "ProductList",
  computed: {
    ...mapGetters(["products"]),
  },
  methods: {
    ...mapActions(["getProducts"]),
  },

  mounted() {
    this.getProducts();
  },
};
</script>

<style scoped>
.card {
  padding: 20px;
  border: none;
}
</style>
