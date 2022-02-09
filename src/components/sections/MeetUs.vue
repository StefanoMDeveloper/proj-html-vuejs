<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">
          meet the new agency SEO template from the avada team
        </h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat
          voluptate quisquam numquam vel porro quo laborum sint!
        </p>
      </div>
      <div class="card-container row">
        <CardsMeetUs
          v-for="(elem, index) in arrayCarte"
          :key="index"
          :info="elem"
        />
      </div>
      <div class="immagine text-center">
        <img src="../../assets/img/agency-seo-desk-front-800x380.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
import CardsMeetUs from "../commons/CardsMeetUs.vue";
export default {
  name: "MeetUs",
  components: {
    CardsMeetUs,
  },
  data() {
    return {
      arrayCarte: [
        {
          simbolo: "fas fa-solid fa-road",
          titolo: "establish goals",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          simbolo: "fas fa-solid fa-video",
          titolo: "work with a team",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          simbolo: "fas fa-solid fa-droplet",
          titolo: "get results",
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
  width: 50%;
  margin: 0 auto;
}

.card-container{
  width: 80%;
  margin: 0 auto;
}

.sezione {
  background-color: $alabaster;
  padding-top: 80px;
}

p{
  color: $scorpion;
  padding: 10px 0 30px 0;
}
</style>