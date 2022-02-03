<template>
  <article>
    <div class="listapps-cntr">
      <div class="listapps-img">
        <img class="my-img" :src=img>
      </div>
      <div class="listapps-info">
        <h4 class="my-h4">{{name}}</h4>
        <span class="my-span">{{state}}</span>
        <div class="my-lnk-app">
          <a class="my-a" :href=linkApp>preview</a>
          <a class="icon-app" :href=linkBehance>
            <i class="fab fa-behance" aria-hidden="true"></i>
          </a>
          <a class="icon-app" :href=linkGithub>
            <i class="fab fa-github" aria-hidden="true"></i>
          </a>
        </div>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name:'App',
  props:{
    img:String,
    name:String,
    state:String,
    linkApp:String,
    linkBehance:String,
    linkGithub:String,
  }
}
</script>