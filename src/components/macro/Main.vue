<template>
  <div>
    <Hero/>
    <MeetUs/>
  </div>
</template>

<script>
import Hero from "../sections/Hero.vue"
import MeetUs from "../sections/MeetUs.vue"
export default {
    name: "Main",
    components: {
      Hero,
      MeetUs
    }
}
</script>

<style scoped lang="scss">

</style>