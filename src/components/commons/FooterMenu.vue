<template>
  <div  class="menu">
    <ul>
      <li class="text-orange">home</li>
      <li>Who We Are</li>
      <li>What we Do</li>
      <li>Where We Work</li>
      <li>Careers</li>
      <li>News</li>
      <li>Get in touch now</li>
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
  li {
    display: inline;
    margin: 0 18px;
    text-transform: capitalize;
    font-size: 14px;
  }
}

.menu{
    padding: 40px 0;
}

</style>