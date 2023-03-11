<template>
  <div class="home">
    <TopNavigation/>
    <HeroSection/>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HeroSection from '@/components/partials/HeroSection.vue';
import TopNavigation from "@/components/structure/TopNavigation";

export default {
  name: 'HomeView',
  components: {
    TopNavigation,
    HeroSection
  }
}
</script>
