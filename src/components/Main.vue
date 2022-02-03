<template>
  <main id="main">
    <Title info="Featured work" />
    <SpclApp />

    <Title info="More Works" id="more-apps" />
    <ListApps />

    <Cards />
  </main>
</template>

<script>
import Title from './main/blog/Title.vue';
import SpclApp from './main/SpclApp.vue';
import ListApps from './main/AddApp.vue';
import Cards from './main/Cards.vue';
export default {
  name:'Main',
  components:{
    Title,
    SpclApp,
    ListApps,
    Cards,
  }
}
</script>