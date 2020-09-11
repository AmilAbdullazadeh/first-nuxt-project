<template>
  <div>
    <Logo />

    <h3>Products</h3>
    <p>Lorem ipsum dolor sit amet.</p>

    <div class="btns">
      <a href="/products" class="button--grey">Products (SSR)</a>
      <nuxt-link to="/products" tag="a" class="button--grey"
        >Products</nuxt-link
      >
    </div>
    <br />
    <Logo />
  </div>
</template>

<script>
import Logo from "@/components/Logo";
// import Logo from "~/components/Logo"

export default {
  components: {
    Logo
  }
};
</script>
