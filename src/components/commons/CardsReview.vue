<template>
  <div class="col-12 my-cards">
    <div v-if="info.visibile">
      <img
        class="rounded-circle"
        :src="info.testimonial"
        alt="immagine non disponibile"
      />
      <p class="m-2 fst-italic fw-bold">{{ info.commento }}</p>
      <span class="fw-bold">{{ info.nome }},</span>
      <span class="m-2">{{ info.azienda }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardsReview",
  props: {
    info: Object,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.my-cards {
  text-align: center;
}

p {
  font-size: 14px;
  color: $scorpion;
  line-height: 25px;
}

img {
  width: 140px;
}

span {
  font-size: 14px;
}
</style>