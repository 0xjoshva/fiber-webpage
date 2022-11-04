<template>
  <main>
    <HomeLanding />
    <HomeAbout />
    <HomeBluePanel/>
    <HomeTestimonials />
  </main>
</template>

<script>
import HomeLanding from "@/components/HomeLanding.vue";
import HomeAbout from "@/components/HomeAbout.vue";
import HomeTestimonials from "@/components/HomeTestimonials.vue";
import HomeBluePanel from "@/components/HomeBluePanel.vue"

export default {
  components: {
    HomeLanding,
    HomeAbout,
    HomeTestimonials,
    HomeBluePanel
  },
};
</script>
