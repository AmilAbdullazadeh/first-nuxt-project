<template>
  <div style="margin-bottom: 10px">
    <div class="inputs">
      <input type="text" v-model="productID" />
      <button class="button--green" @click="showProduct">Show Product</button>
    </div>
  </div>
</template>

<script>
export default {
  layout: "product",

  data() {
    return {
      productID: null
    };
  },

  methods: {
    showProduct() {
      this.$router.push("/products/" + this.productID);
    }
  }
};
</script>
