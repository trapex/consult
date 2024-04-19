<script setup>
import Consult from '../components/Consult.vue'
import CardBlock from '../components/CardBlock.vue'
import WhyChoose from '../components/WhyChoose.vue'
import Team from '../components/Team.vue'
import Strategy from '../components/Strategy.vue'
import FAQ from '../components/FAQ.vue'
import SetupCall from '../components/SetupCall.vue'
</script>

<template>
  <div>
    <Consult />
    <CardBlock />
    <WhyChoose/>
    <Team />
    <Strategy />
    <FAQ />
    <div class="setup-call-block">
      <SetupCall />
    </div>
  </div>
</template>

<style scoped>
  .setup-call-block {
    margin-top: 86px;
    margin-bottom: 50px;
  }
</style>