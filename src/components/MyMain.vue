<template>
  <main>
      <MyJumbo/>
      <ConsultingSection/>
      <AboutSection/>
      <CtaSection/>
      <ProjectSection/>
  </main>
</template>

<script>
import MyJumbo from './partials/MyJumbo.vue';
import ConsultingSection from './partials/ConsultingSection.vue';
import AboutSection from './partials/AboutSection.vue';
import CtaSection from './partials/CtaSection.vue';
import ProjectSection from './partials/ProjectSection.vue';

export default {
    name: 'MyMain',
    components: {
        MyJumbo,
        ConsultingSection,
        AboutSection,
        CtaSection,
        ProjectSection,
    }
}
</script>

<style lang="scss" scoped>

</style>