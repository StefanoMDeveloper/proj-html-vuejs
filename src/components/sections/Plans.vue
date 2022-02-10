<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">our plans</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatum
          aperiam at, nostrum eaque laudantium unde recusandae, molestiae
          officia!
        </p>
      </div>
      <div class="card-container row row-cols-4 flex-nowrap">
        <CardsPlans
          v-for="(elem, index) in arrayCarte"
          :key="index"
          :info="elem"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardsPlans from "../commons/CardsPlans.vue";
export default {
  name: "Plans",
  components: {
    CardsPlans,
  },
  data() {
    return {
      arrayCarte: [
        {
          titolo: "Standard",
          prezzo: "19",
          centesimi: ".99",
          abbonamento: "monthly",
          nProgetti: "5 projects",
          memoria: "5 GB Storage",
          nUtenti: "Unlimited Users",
          attivo: false
        },
        {
          titolo: "Premium",
          prezzo: "29",
          centesimi: ".99",
          abbonamento: "monthly",
          nProgetti: "5 projects",
          memoria: "5 GB Storage",
          nUtenti: "Unlimited Users",
          attivo: false
        },
        {
          titolo: "Professional",
          prezzo: "39",
          centesimi: ".99",
          abbonamento: "monthly",
          nProgetti: "5 projects",
          memoria: "5 GB Storage",
          nUtenti: "Unlimited Users",
          attivo: true
        },
        {
          titolo: "Extreme",
          prezzo: "59",
          centesimi: ".99",
          abbonamento: "monthly",
          nProgetti: "5 projects",
          memoria: "5 GB Storage",
          nUtenti: "Unlimited Users",
          attivo: false
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.text-container {
  width: 50%;
  margin: 0 auto;
  color: white;
}

.card-container {
  width: 80%;
  margin: 0 auto;
  padding-bottom: 100px;
  justify-content: space-evenly;
}

.sezione {
  background-image: url("../../assets/img/background1.jpg");
  padding-top: 60px;
  background-color: $deep-cove;
  background-size: cover;
  background-position: center center;
}
p {
  padding: 10px 0 50px 0;
}

h2 {
  margin-top: 30px;
}
</style>