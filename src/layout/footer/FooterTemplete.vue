<script setup>
import CommunityTraders from "./CommunityTraders.vue";
import ContentFooter from "./ContentFooter.vue";
import ServiceComponents from "./ServiceComponents.vue";
import TechnologyServices from "./TechnologyServices.vue";
</script>

<template>
  <div class="footer">
    <section>
      <ServiceComponents />
    </section>
    <section>
      <TechnologyServices />
    </section>
    <section>
      <CommunityTraders />
    </section>
    <section>
      <ContentFooter />
    </section>
  </div>
</template>

<style scoped>
.footer {
  width: 100%;
  display: flex;
  flex-direction: column;
}
</style>
