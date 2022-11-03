<template>
  <main>
    <HomeLanding />
    <HomeAbout />
    <HomeTestimonials />
  </main>
</template>

<script>
import HomeLanding from "@/components/HomeLanding.vue";
import HomeAbout from "@/components/HomeAbout.vue";
import HomeTestimonials from "@/components/HomeTestimonials.vue";

export default {
  components: {
    HomeLanding,
    HomeAbout,
    HomeTestimonials,
  },
};
</script>
