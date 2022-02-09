<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">
          see our top notch services
        </h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat
          voluptate quisquam numquam vel porro quo laborum sint!
        </p>
      </div>
      <div class="card-container row">
        <CardsServicies
          v-for="(elem, index) in arrayCarte"
          :key="index"
          :info="elem"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CardsServicies from "../commons/CardsServicies.vue";
export default {
  name: "Servicies",
  components: {
    CardsServicies,
  },
  data() {
    return {
      arrayCarte: [
        {
          simbolo: "fas fa-brands fa-google",
          titolo: "Google SEO",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          simbolo: "fas fa-solid fa-gear",
          titolo: "Brand Strategy",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          simbolo: "fas fa-solid fa-building",
          titolo: "Local SEO",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          simbolo: "fas fa-solid fa-chart-column",
          titolo: "SEO analysis",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.text-container {
  width: 40%;
  margin: 0 auto;
  color: white;
}

.card-container{
  width: 80%;
  margin: 0 auto;
  padding-bottom: 100px;
}

.sezione {
  background-image: url("../../assets/img/pattern_background.png");
  padding-top: 60px;
  background-color: $deep-cove;
  background-size: contain;
}
p{
  padding: 10px 0 50px 0;
}

h2{
  margin-top: 30px;
}
</style>