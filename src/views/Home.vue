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
      header: ["Hi! I'm Ervina your", "education counsellor."],
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
      padding-top: 75px;
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
      padding-top: 13px;
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
        line-height: 1.8;
      }
    }
    #ContactBar{
      padding-top: 20px;
      width: 410px;
      height: fit-content;
    }
    #MosaicTiles{
      padding-top: 30px;
      width: 65%;
      height: 300px;
    }
    #BottomBar{
      margin-top: auto;
    }
  }
  #SideBar{
    width: 24%;
    height: 92%;
    padding: 15px 15px;
  }
}

</style>