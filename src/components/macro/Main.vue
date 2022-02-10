<template>
  <div>
    <Hero/>
    <MeetUs/>
    <Servicies/>
    <OurWork/>
    <Plans/>
    <News/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
import Servicies from "../sections/Servicies.vue"
import OurWork from "../sections/OurWork.vue"
import Plans from "../sections/Plans.vue"
import News from "../sections/News.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs,
      Servicies,
      OurWork,
      Plans,
      News,
    }
}
</script>

<style scoped lang="scss">

</style>