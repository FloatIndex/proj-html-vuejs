<template>
  <main>
      <MyJumbo/>
      <ConsultingSection/>
      <AboutSection/>
      <MidCtaSection/>
      <ProjectSection/>
      <TestimonialSection/>
      <BlogSection/>
      <FinalCtaSection/>
  </main>
</template>

<script>
import MyJumbo from './partials/MyJumbo.vue';
import ConsultingSection from './partials/ConsultingSection.vue';
import AboutSection from './partials/AboutSection.vue';
import MidCtaSection from './partials/MidCtaSection.vue';
import ProjectSection from './partials/ProjectSection.vue';
import TestimonialSection from './partials/TestimonialSection.vue';
import BlogSection from './partials/BlogSection.vue';
import FinalCtaSection from './partials/FinalCtaSection.vue';

export default {
    name: 'MyMain',
    components: {
        MyJumbo,
        ConsultingSection,
        AboutSection,
        MidCtaSection,
        ProjectSection,
        TestimonialSection,
        BlogSection,
        FinalCtaSection,
    }
}
</script>

<style lang="scss" scoped>

</style>