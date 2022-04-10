<template>
  <section class="main-listapps">
    <App 
      img="img/ProfilePicture.png"
      name="FrsCodes"
      state="alive"
      linkApp="https://frscodes.github.io/"
      linkBehance="https://www.behance.net/gallery/133362257/FrsCodes-brand-identity"
      linkGithub="https://github.com/frscodes/frscodes.github.io"
    />

    <App 
      img="img/marj3i.jpg"
      name="Marj3i"
      state="alive"
      linkApp="https://marj3i.github.io/"
      linkBehance="unavailable"
      linkGithub="https://github.com/Marj3i"
    />

    <App 
      img="img/dalil.jpg"
      name="Dalilmutabarie"
      state="closed"
      linkApp="https://frscodes.github.io/dalilmutabarie/"
      linkBehance="https://www.behance.net/gallery/112138003/dalilmutabarie"
      linkGithub="https://github.com/frscodes/dalilmutabarie"
    />

    <App 
      img="img/apps.jpg"
      name="Google Play app gallery"
      state="closed"
      linkApp="https://frscodes.github.io/GooglePlay-EN/"
      linkBehance="unavailable"
      linkGithub="unavailable"
    />

    <App 
      img="img/acila.jpg"
      name="Acila accessories"
      state="closed"
      linkApp="unavailable"
      linkBehance="https://www.behance.net/gallery/126639795/Acila-for-accessories-brand"
      linkGithub="unavailable"
    />

    <App 
      img="img/elyatro.png"
      name="Elyatro"
      state="soon"
      linkApp="unavailable"
      linkBehance="https://www.behance.net/gallery/126922357/Elyatro"
      linkGithub="unavailable"
    />

    <App 
      img="img/ubexpay.png"
      name="UBEXPay"
      state="closed"
      linkApp="unavailable"
      linkBehance="unavailable"
      linkGithub="unavailable"
    />

    <App 
      img="img/Gaith.jpg"
      name="Gaith"
      state="soon"
      linkApp="unavailable"
      linkBehance="unavailable"
      linkGithub="unavailable"
    />
  </section>
</template>

<script>
import App from './blog/App.vue';
export default {
  name:'ListApps',
  components:{
    App,
  },
  mounted(){
    let allLink = document.querySelectorAll(".main-listapps a");
    var i = 0;
    for (i = 0; i < allLink.length; i++){
      if(allLink[i].href.indexOf("unavailable") > 0){
        allLink[i].classList.add("soon");
      }
    }
  },
}
</script>