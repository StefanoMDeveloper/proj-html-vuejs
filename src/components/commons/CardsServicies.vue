<template>
  <div class="col text-center my-cards">
    <i :class="info.simbolo" ></i>
    <h4 class="fw-bold text-capitalize m-2">{{info.titolo}}</h4>
    <p class="m-2 description">{{info.testo}}</p>
    <p class="read-more text-capitalize">Read more ></p>
  </div>
</template>

<script>
export default {
    name: "CardsServicies",
    props: {
      info: Object,
    },
}
</script>

<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';
.my-cards{
  background-color: $daisy-blush;
  padding: 20px;
  margin: 10px;
  color: white;
}

.description{
  font-size: 14px;
  line-height: 30px;
}

.read-more{
    color: $yellow-orange;
}

svg{
  color: $yellow-orange;
  font-size: 35px;
  margin: 20px 0;
}

h4{
    padding: 10px 0;
}
</style>