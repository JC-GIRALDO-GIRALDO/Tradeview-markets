<script setup>
import CommunityTraders from "./CommunityTraders.vue";
import ContentFooter from "./ContentFooter.vue";
import ServiceComponents from "./ServiceComponents.vue";
import TechnologyServices from "./TechnologyServices.vue";
</script>

<template>
  <div class="footer">
    <section class="ServiceComponents">
      <ServiceComponents />
    </section>
    <section class="TechnologyServices">
      <TechnologyServices />
    </section>
    <section class="CommunityTraders">
      <CommunityTraders />
    </section>
    <section class="ContentFooter">
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
.ServiceComponents {
  margin-top: 55rem;
  background-color: #ffffff;
}
@media (max-width: 768px) {
  .ServiceComponents,
  .TechnologyServices,
  .CommunityTraders,
  .ContentFooter {
    width: 100%;
  }
}
</style>
