<template>
  <div class="sezione">
    <div class="my-container">
      <div class="text-container text-center">
        <h2 class="text-capitalize fw-bold">our work</h2>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat sequi
          et sed distinctio, culpa iure cumque!
        </p>
      </div>
      <div class="card-container row row-cols-3 g-3">
        <img
          class="col"
          src="../../assets/img/case-study-gallery-3-1.jpg"
          alt=""
        />
        <img
          class="col"
          src="../../assets/img/case-study-gallery-2.jpg"
          alt=""
        />
        <img
          class="col"
          src="../../assets/img/case-study-gallery-1-1.jpg"
          alt=""
        />
        <img
          class="col"
          src="../../assets/img/case-study-gallery-4-1.jpg"
          alt=""
        />
        <img
          class="col"
          src="../../assets/img/case-study-gallery-5-1.jpg"
          alt=""
        />
        <img
          class="col"
          src="../../assets/img/case-study-gallery-6-1.jpg"
          alt=""
        />
      </div>
      <div class="bottone">
        <span class="btn rounded-pill orange-button text-white">view our work</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurWork",
};
</script>

<style scoped lang="scss">
@import "../../assets/style/partials/variables.scss";
.text-container {
  width: 50%;
  margin: 0 auto;
}

.card-container {
  margin: 0 auto;
}

.sezione {
  background-color: $alabaster;
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