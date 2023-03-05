<template>
  <div class="home">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <HeroSection />
    <Example />
  </div>
</template>

<script>
// @ is an alias to /src
import Example from '@/components/ExampleComponent.vue';
import HelloWorld from '@/components/HelloWorld.vue'
import HeroSection from '@/components/partials/HeroSection.vue';

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    HeroSection,
    Example
}
}
</script>
