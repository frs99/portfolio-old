<template>
  <section class="main-title">
    <h1 class="h1-title" :id="id">{{info}}</h1>
  </section>
</template>

<script>
export default {
  name:'Title',
  props:{
    info:String,
    id:String,
  }
}
</script>