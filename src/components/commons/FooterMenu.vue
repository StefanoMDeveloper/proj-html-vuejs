<template>
  <div  class="menu">
    <ul>
      <li class="text-orange"><a href="#hero">home</a></li>
      <li><a href="#meetUs">Who We Are</a></li>
      <li><a href="#services">What we Do</a></li>
      <li><a href="#ourWork">Where We Work</a></li>
      <li><a href="#plans">Careers</a></li>
      <li><a href="#news">News</a></li>
      <li><a href="#consultation">Get in touch now</a></li>
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