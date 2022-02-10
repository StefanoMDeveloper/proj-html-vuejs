<template>
  <div>
    <Hero/>
    <MeetUs/>
    <Servicies/>
    <OurWork/>
    <Plans/>
    <News/>
    <Review/>
    <Partners/>
    <Consultation/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
import Servicies from "../sections/Servicies.vue"
import OurWork from "../sections/OurWork.vue"
import Plans from "../sections/Plans.vue"
import News from "../sections/News.vue"
import Review from "../sections/Review.vue"
import Partners from "../sections/Partners.vue"
import Consultation from "../sections/Consultation.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs,
      Servicies,
      OurWork,
      Plans,
      News,
      Review,
      Partners,
      Consultation,
    }
}
</script>

<style scoped lang="scss">

</style>