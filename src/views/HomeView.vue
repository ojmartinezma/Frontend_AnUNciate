<template>
  <NavBar></NavBar>
  <div>
    <MainHeader></MainHeader>
  </div>
  <div>
    <ProductList></ProductList>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import NavBar from "@/components/NavBar.vue";
import MainHeader from "@/components/MainHeader.vue";
import ProductList from "@/components/ProductList.vue";

export default defineComponent({
  name: "MainPage",
  components: { NavBar, MainHeader, ProductList },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
