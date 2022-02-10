<template>
  <div class="sezione">
    <div class="my-container text-center">
      <img src="../../assets/img/logo_seo_1x.png" alt="" />
      <FooterMenu />

      <p class="crediti">
        @ Copyright 2012-2022 | Avada Theme by <span>StefanoMDeveloper</span> |
        All Rigths Not Reserved | Not Powered By <span>Wordpress</span>
      </p>
      <i class="fas fa-brands fa-facebook-f"></i>
      <i class="fas fa-brands fa-instagram"></i>
      <i class="fas fa-brands fa-twitter"></i>
      <i class="fas fa-brands fa-youtube"></i>
    </div>
  </div>
</template>

<script>
import FooterMenu from "../commons/FooterMenu.vue";
export default {
  name: "Footer",
  components: {
    FooterMenu,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.sezione {
  background-color: white;
  padding: 50px 0;
}

span {
  color: black;
}

.crediti, svg {
  color: grey;
}

svg{
  font-size: 30px;
  padding: 10px 20px;
}
</style>