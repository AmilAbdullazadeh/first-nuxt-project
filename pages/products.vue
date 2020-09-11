<template>
  <div>
    <SearchProduct />
    <nuxt-child />
  </div>
</template>

<script>
import SearchProduct from "@/components/SearchProduct";

export default {
  components: {
    SearchProduct
  }
};
</script>

<style></style>
