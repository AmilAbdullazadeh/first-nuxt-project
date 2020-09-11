<template>
  <div class="container">
    <h5>This page is ID: {{ $route.params.productID }}</h5>

    <div style="margin-top: 5px; margin-bottom: 10px;" class="btns">
      <nuxt-link to="/products" tag="a" class="button--grey">Back</nuxt-link>
      <button class="button--green" @click="editProduct">Edit</button>
    </div>
  </div>
</template>

<script>
export default {
  validate(arg) {
    return /^\d+$/.test(arg.params.productID);
  },

  methods: {
    editProduct() {
      this.$router.push("/products/" + this.$route.params.productID + "/edit");
    }
  }
};
</script>
