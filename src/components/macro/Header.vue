<template>
  <div class="container fixed-top">
    <div class="header-container row g-0">
      <div class="col-2">
        <img src="../../assets/img/logo_seo_w_2x.png" alt="" />
      </div>
      <div class="col-10">
        <NavMenu />
      </div>
    </div>
  </div>
</template>

<script>
import NavMenu from "../commons/NavMenu.vue"
export default {
  name: "Header",
  components: {
    NavMenu
  }
};
</script>

<style scoped lang="scss">
.header-container {
  height: 100px;
  width: 100%;
  padding: 30px;
  justify-content: space-between;
  position: absolute;
  top: 0;
  left: 0;
  img {
    height: 100%;
  }
}

div {
  height: 100%;
}
</style>