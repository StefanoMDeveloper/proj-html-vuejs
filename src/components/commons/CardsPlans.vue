<template>
  <div class="col text-center my-cards">
    <h4 class="fw-bold text-capitalize m-2">{{ info.titolo }}</h4>
    <div class="abbonamento fw-bold">
      <span class="dollaro">$</span>
        <span class="prezzo">
          {{ info.prezzo }}
        </span>
        <span class="centesimi">{{ info.centesimi }}</span>
        <span class="durata-abbonamento"> {{ info.abbonamento }}</span>
    </div>
    <div class="description">
      <p class="m-2">{{ info.nProgetti }}</p>
      <p class="m-2">{{ info.memoria }}</p>
      <p class="m-2">{{ info.nUtenti }}</p>
    </div>
    <div class="btn rounded-pill orange-button text-white fw-bold">start today</div>
  </div>
</template>

<script>
export default {
  name: "CardsPlans",
  props: {
    info: Object,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.my-cards {
  background-color: white;
  padding: 20px;
  margin: 10px;
}

.description {
  font-size: 14px;
  line-height: 50px;
}

h4 {
  padding: 10px 0;
}

.durata-abbonamento {
  font-size: 10px;
  font-style: italic;
  padding-left: 5px;
}

.prezzo {
  font-size: 50px;
  color: $science-blue;
}

.centesimi {
  color: $science-blue;
  vertical-align: text-top;
}

.abbonamento{
    padding: 20px 0;
    span{
        display: inline-block;
        line-height: 100%;
    }
}

.dollaro{
    vertical-align: text-top;
}

</style>