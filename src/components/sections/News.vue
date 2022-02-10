<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">our news</h2>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deserunt,
          quia. Perspiciatis illo eveniet, voluptatem cumque provident.
        </p>
      </div>
      <div class="card-container row g-3">
        <CardsNews
          v-for="(elem, index) in arrayCarte"
          :key="index"
          :info="elem"
        />
      </div>
      <div class="bottone">
        <span class="btn rounded-pill orange-button text-white">go to news</span>
      </div>
    </div>
  </div>
</template>

<script>
import CardsNews from "../commons/CardsNews.vue";
export default {
  name: "News",
  components: {
    CardsNews,
  },
  data() {
    return {
      arrayCarte: [
        {
          immagine: 'img/related-service-2-320x202.89e0ded3.jpg',
          titolo: "why you need a SEO agency now",
          data: "November 1st, 2017",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          immagine: 'img/related-service-4-320x202.64ea40a8.jpg',
          titolo: "SEO tips for your startup",
          data: "November 1st, 2017",
          testo:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque ullam est laudantium sapiente, delectus magni animi dolorum quo.",
        },
        {
          immagine: 'img/blog-post-6-320x202.eb4561d0.jpg',
          titolo: "image optimization for your site",
          data: "November 1st, 2017",
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

.card-container {
  width: 80%;
  margin: 0 auto;
      justify-content: space-evenly;
}

.sezione {
  background-color: $concrete;
  padding-top: 80px;
}

p {
  color: $scorpion;
  padding: 10px 0 30px 0;
}
.bottone{
    text-align: center;
    padding: 60px;
}
</style>