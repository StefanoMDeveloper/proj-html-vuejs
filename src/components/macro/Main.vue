<template>
  <div>
    <Hero/>
    <MeetUs/>
    <Servicies/>
    <OurWork/>
    <Plans/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
import Servicies from "../sections/Servicies.vue"
import OurWork from "../sections/OurWork.vue"
import Plans from "../sections/Plans.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs,
      Servicies,
      OurWork,
      Plans,
    }
}
</script>

<style scoped lang="scss">

</style>