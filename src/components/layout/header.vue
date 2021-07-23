<template>
  <a-layout-header class="header">
    <img :src="logoIcon" alt="" />
  </a-layout-header>
</template>

<script>
import Logo from "../../assets/icons/logo.svg";

export default {
  name: "header",
  data() {
    return {
      logoIcon: Logo,
    };
  },
};
</script>

<style scoped>
.header {
  background-color: #5a1e82;
}
</style>
