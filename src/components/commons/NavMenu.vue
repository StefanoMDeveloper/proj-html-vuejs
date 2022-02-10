<template>
  <div>
    <ul>
      <li class="text-orange"><a href="#hero">home</a></li>
      <li><a href="#meetUs">Who We Are</a></li>
      <li><a href="#services">What we Do</a></li>
      <li><a href="#ourWork">Where We Work</a></li>
      <li><a href="#plans">Careers <span class="apply">apply</span></a></li>
      <li><a href="#news">News</a></li>
      <li class="btn rounded-pill orange-button text-white"><a href="#consultation">Get in touch now</a></li>
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