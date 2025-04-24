<script setup>
  import ExperienceSection from '@/components/Sections/ExperienceSection.vue';
  import ProjectsSection from '@/components/Sections/ProjectsSection.vue';
  import AboutSection from '@/components/Sections/AboutSection.vue';
  import ContactSection from '@/components/Sections/ContactSection.vue';

</script>
<template>
  <div class="content">
    <section id="about">
      <AboutSection />
    </section>
    <section id="experience">
      <ExperienceSection />
    </section>
    <section id="projects">
      <ProjectsSection />
    </section>
    <section id="contact">
      <ContactSection />
    </section>
  </div>
</template>

<style scoped>
.content {
  padding: 20px;
}

section {
  margin-bottom: 40px;
}
</style>
