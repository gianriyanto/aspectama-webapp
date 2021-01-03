<template>
  <div id="BottomBar">
    <div id="SocialLinks">
      <a class="link"> Instagram </a>
      <span class="slash"> / </span>
      <a class="link"> Facebook </a>
      <span class="slash"> / </span>
      <a class="link"> Aspectama </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomBar"
}
</script>

<style lang="scss" scoped>

#BottomBar{
  width: 100%;
  height: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

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
    }

    .slash{
      font-family: "Bw Modelica Bold", serif;
      font-size: 13px;
      color: #292929;
    }
  }
}

</style>