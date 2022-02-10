<template>
  <div class="sezione">
    <div class="my-container row row-cols-4">
      <img class="col" src="../../assets/img/clients_partner_5-200x202.png" alt="" />
      <img class="col" src="../../assets/img/clients_partner_6-200x202.png" alt="" />
      <img class="col" src="../../assets/img/clients_partner_1-200x202.png" alt="" />
      <img class="col" src="../../assets/img/clients_partner_2-200x202.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Partners",
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.sezione {
  background-color: white;
  padding: 50px 0;

  border-top: 1px solid $regent-gray;
}

.my-container{
    justify-content: space-evenly;
}

img{
    width: 100px;
}
</style>