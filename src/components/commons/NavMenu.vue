<template>
  <div>
    <ul>
      <li class="text-orange">home</li>
      <li>Who We Are</li>
      <li>What we Do</li>
      <li>Where We Work</li>
      <li>Careers <span class="apply">apply</span></li>
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
@import '../../assets/style/partials/variables.scss';
ul {
  list-style-type: none;
  padding: 10px 0px;
  float: right;
  li {
    display: inline;
    margin: 0 12px;
    text-transform: capitalize;
    font-size: 14px;
    color: white;
  }
}

.apply{
  padding: 5px;
  border: 1px solid $yellow-orange;
  color: $yellow-orange;
  font-size: 12px;
  margin-left: 5px;
  border-radius: 7px;
  text-transform: uppercase;
}
</style>