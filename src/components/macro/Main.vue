<template>
  <div>
    <Hero/>
    <MeetUs/>
    <Servicies/>
    <OurWork/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
import Servicies from "../sections/Servicies.vue"
import OurWork from "../sections/OurWork.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs,
      Servicies,
      OurWork,
    }
}
</script>

<style scoped lang="scss">

</style>