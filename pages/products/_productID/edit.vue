<template>
  <div class="container">
    <h3>This page is Detail</h3>
    <small>This page is ID: {{ $route.params.productID }}</small>

    <div style="margin-top: 5px; margin-bottom: 10px;" class="btns">
      <nuxt-link
        :to="'/products/' + $route.params.productID"
        tag="a"
        class="button--grey"
        >Back</nuxt-link
      >
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
