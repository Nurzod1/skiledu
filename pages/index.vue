<template>
  <div class="page">
    <Header />
    <Clients />
    <Cloud />
    <SkilLine />
    <ClassRoom />
    <Features />
    <Integration />
    <News />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Clients from "@/components/Clients.vue";
import Cloud from "@/components/Cloud.vue";
import SkilLine from "@/components/SkilLine.vue";
import ClassRoom from "@/components/ClassRoom.vue";
import Features from "@/components/Features.vue";
import Integration from "@/components/Integration.vue";
import News from "@/components/News.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "IndexPage",

  components: {
    Header,
    Clients,
    Cloud,
    SkilLine,
    ClassRoom,
    Features,
    Integration,
    News,
    Footer,
  },
};
</script>
