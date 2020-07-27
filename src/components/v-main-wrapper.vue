<template>
  <div class="v-main-wrapper">
    <p>{{ title }}</p>
    <v-catalog />
    <v-cart />
  </div>
</template>

<script>
import vCatalog from "./v-catalog";
import vCart from "./v-cart";

export default {
  name: "v-main-wrapper",
  components: {
    vCatalog,
    vCart,
  },
  // data from parent
  props: {},
  // data of this components
  data() {
    return {
      title: "U can",
    };
  },
};
</script>

<style>
.v-main-wrapper {
  max-width: 900px;
  margin: 0 auto;
}
</style>
