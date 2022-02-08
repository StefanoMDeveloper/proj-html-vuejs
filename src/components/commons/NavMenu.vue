<template>
  <div>
    <ul>
      <li class="text-orange">home</li>
      <li>Who We Are</li>
      <li>What we Do</li>
      <li>Where We Work</li>
      <li>Careers <span>applay</span></li>
      <li>News</li>
      <li class="btn rounded-pill orange-button">Get in touch now</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NavMenu",
};
</script>

<style scoped lang="scss">
ul {
  list-style-type: none;
  padding: 10px 0px;
  float: right;
  li {
    display: inline;
    margin: 0 15px;
    text-transform: capitalize;
    font-size: 14px;
    color: white;
  }
}
</style>