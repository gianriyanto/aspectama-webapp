<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
      <span class="header-container">
        <h1 class="header-text"> {{ header[0] }} </h1>
        <h1 class="header-text"> {{ header[1] }} </h1>
      </span>
      <span class="subheader-container">
        <h2 class="subheader-text"> {{ subheader[0] }} </h2>
        <h2 class="subheader-text"> {{ subheader[1] }} </h2>
      </span>
      <ContactBar id="ContactBar"/>
      <MosaicTiles id="MosaicTiles"/>
      <BottomBar id="BottomBar"/>
    </div>
    <SideBar id="SideBar"/>
  </section>
</template>

<script>

import TopBar from "@/components/TopBar";
import MosaicTiles from "@/components/MosaicTiles";
import ContactBar from "@/components/ContactBar";
import BottomBar from "@/components/BottomBar";
import SideBar from "@/components/SideBar";

export default {
  name: "Home",
  components: {
    SideBar,
    BottomBar,
    ContactBar,
    MosaicTiles,
    TopBar
  },
  data() {
    return {
      header: ["Hi! I'm Ervina your", "education counselor."],
      subheader: ["I help architect a personalised education blueprint for aspiring professionals like you.", "Find out how I can help, I’d love to hear from you."]
    }
  }
}
</script>

<style lang="scss" scoped>

#Home{
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100vh;

  .main-wrapper{
    width: 70%;
    height: 96%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-right: 22px;

    .header-container{
      padding-top: 80px;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 600px;
      text-align: center;

      h1{
        margin: 0;
        font-family: "Gilroy SemiBold", serif;
        font-size: 37px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.1;
      }
    }
    .subheader-container{
      padding-top: 10px;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: fit-content;
      text-align: center;

      h2{
        margin: 0;
        font-family: "Bw Modelica Regular", serif;
        font-size: 13px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.7;
      }
    }
    #ContactBar{
      padding-top: 25px;
      width: 380px;
      height: fit-content;
    }
    #MosaicTiles{
      padding-top: 35px;
      width: 68%;
      height: 35%;
    }
    #BottomBar{
      margin-top: auto;
    }
  }
  #SideBar{
    width: 24%;
    min-width: 320px;
    height: 92%;
    padding: 15px 15px;
  }
}

</style>