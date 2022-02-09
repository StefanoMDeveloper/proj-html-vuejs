<template>
  <div>
    <Hero/>
    <MeetUs/>
    <Servicies/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
import Servicies from "../sections/Servicies.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs,
      Servicies
    }
}
</script>

<style scoped lang="scss">

</style>