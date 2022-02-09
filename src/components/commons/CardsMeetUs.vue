<template>
  <div class="col text-center my-cards">
    <i :class="info.simbolo" ></i>
    <h5 class="fw-bold text-capitalize m-2">{{info.titolo}}</h5>
    <p class="m-2">{{info.testo}}</p>
  </div>
</template>

<script>
export default {
    name: "CardsMeetUs",
    props: {
      info: Object,
    },
}
</script>

<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';
.my-cards{
  background-color: white;
  padding: 20px;
  margin: 10px;
  

}

p{
  font-size: 14px;
  color: $scorpion;
}

svg{
  color: $yellow-orange;
  font-size: 35px
}
</style>