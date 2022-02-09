<template>
  <div class="hero-container">
    <div class="my-container">
      <div class="hero-text">
        <h1 class="fw-bold">SEM Campaigns Made Simple With Avada</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident,
          blanditiis cupiditate?
        </p>
        <div class="buttons mt-3">
          <span class="btn rounded-pill orange-button">buy avada now</span>
          <span class="btn rounded-pill blue-button ms-5">contact us</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style scoped lang="scss">
.hero-container {
  height: 700px;
  background-image: url("../../assets/img/1-hero-image.png");
  background-size: cover;
  background-position: center center;
}

.my-container {
  position: relative;
}
.buttons{
  padding-top: 10px;
}
.hero-text {
  color: white;
  width: 40%;
  position: absolute;
  bottom: 250px;
  left: 40px;
  span {
    color: white;
  }
}
</style>