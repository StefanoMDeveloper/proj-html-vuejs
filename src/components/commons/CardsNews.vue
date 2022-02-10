<template>
  <div class="col-4 my-cards">
    <img :src="info.immagine" alt="immagine non disponibile">
    <p class="fw-bold text-capitalize m-2 text-orange">{{info.titolo}}</p>
    <p class="data fw-bold">{{info.data}}</p>
    <p class="m-2">{{info.testo}}</p>
  </div>
</template>

<script>
export default {
    name: "CardsNews",
    props: {
      info: Object,
    },
}
</script>

<style scoped lang="scss">
@import '../../assets/style/partials/variables.scss';
.my-cards{
    text-align: center;

}

p{
  font-size: 14px;
  color: $scorpion;
  line-height: 25px;
}

img{
    width: 100%;
}

.data{
    font-style: italic;
    font-size: 12px;

}

.text-orange{
    font-size: 18px;
}
</style>