<template>
  <div class="sezione">

    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">start your free consultations</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatum
          aperiam at, nostrum eaque laudantium unde recusandae, molestiae
          officia!
        </p>
        <p class="btn rounded-pill orange-button text-white">contact us now</p>
      </div>
    </div>
        <div class="immagine-sezione"></div>
  </div>
</template>

<script>
export default {
  name: "Consultation",
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.text-container {
  width: 50%;
  margin: 0 auto;
  color: white;
}
.my-container{
    position: relative;
    z-index: 100;
}

.sezione {
  padding: 60px 0;
  background-size: cover;

  position: relative;
  z-index: 1;
}

.immagine-sezione {
  background-image: url("../../assets/img/CTA-seo-1.jpg");
  background-position: center center;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  filter: brightness(30%);
  z-index: 99;
}

p {
  padding: 10px 0;
}

h2 {
  margin-top: 30px;
}
</style>