<template>
  <div id="SocialLinks">
    <a class="link" v-on:click="goToSite('https://www.instagram.com/aspectamaalamsutera/?hl=en')"> Instagram </a>
    <span class="slash"> / </span>
    <a class="link" v-on:click="goToSite('https://www.facebook.com/Aspectama-AlamSutera-288109908569927/')"> Facebook </a>
    <span class="slash"> / </span>
    <a class="link" v-on:click="goToSite('http://aspectamaalsut.co.id')"> Aspectama </a>
  </div>
</template>

<script>
export default {
  name: "SocialLinks",
  methods: {
    goToSite(url) {
      window.open(url, '_blank');
    }
  },
}
</script>

<style lang="scss" scoped>

#SocialLinks{
  width: 250px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  .link{
    font-family: "Bw Modelica Bold", serif;
    font-size: 13px;
    color: #292929;
    cursor: pointer;
  }

  .slash{
    font-family: "Bw Modelica Bold", serif;
    font-size: 13px;
    color: #292929;
  }
}

</style>