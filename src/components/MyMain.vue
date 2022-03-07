<template>
  <main>
      <MyJumbo/>
      <ConsultingSection/>
      <AboutSection/>
      <CtaSection/>
      <ProjectSection/>
      <TestimonialSection/>
  </main>
</template>

<script>
import MyJumbo from './partials/MyJumbo.vue';
import ConsultingSection from './partials/ConsultingSection.vue';
import AboutSection from './partials/AboutSection.vue';
import CtaSection from './partials/CtaSection.vue';
import ProjectSection from './partials/ProjectSection.vue';
import TestimonialSection from './partials/TestimonialSection.vue';

export default {
    name: 'MyMain',
    components: {
        MyJumbo,
        ConsultingSection,
        AboutSection,
        CtaSection,
        ProjectSection,
        TestimonialSection,
    }
}
</script>

<style lang="scss" scoped>

</style>