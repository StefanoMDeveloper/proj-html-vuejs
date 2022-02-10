<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h3 class="text-capitalize fw-bold">what our client say</h3>
      </div>
      <div class="card-container row g-3">
        <CardsReview
          v-for="(elem, index) in arrayCarte"
          :key="index"
          :info="elem"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardsReview from "../commons/CardsReview.vue";
export default {
  name: "Review",
  components: {
    CardsReview,
  },
  data() {
    return {
      arrayCarte: [
        {
          testimonial: "/img/testimonials-2.0a469679.jpg",
          commento:
            "Ability proceeds froma afusion of skills, knowledge, understanding and imgination, consolidated by experience",
          nome: "Luis Desalvo",
          azienda: "CREO TECH",
          visibile: true,
        },
        {
          testimonial: "/img/testimonials-1.aa095ba8.jpg",
          commento:
            "Intentio certe non prodest, quod petimus mortales animas. Gratias omnibus pro collatione vestra, speramus te mox iterum videre, in inferno!",
          nome: "Anne Roxoff",
          azienda: "W-orld DOMAINc.",
          visibile: false,
        },
      ],
    };
  },
  created() {
    setInterval(this.animazione, 5000);
  },
  methods: {
    animazione() {
      if (this.arrayCarte[0].visibile) {
          this.arrayCarte[0].visibile = false;
          this.arrayCarte[1].visibile = true;
      }else{
          this.arrayCarte[1].visibile = false;
          this.arrayCarte[0].visibile = true;
      }
    },
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.text-container {
  width: 50%;
  margin: 0 auto;
}

.card-container {
  width: 80%;
  margin: 0 auto;
  justify-content: space-evenly;

}

.sezione {
  background-color: white;
  padding-top: 80px;
  padding-bottom: 50px;
}

p {
  color: $scorpion;
  padding: 10px 0 30px 0;
}
.bottone {
  text-align: center;
  padding: 60px;
}

h3 {
  margin-bottom: 30px;
}
</style>