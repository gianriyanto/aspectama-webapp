<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
      <transition appear name="fade">
        <span class="header-container">
          <h1 class="header-text"> Hi! I'm <span class="highlight-name"> Ervina. </span> </h1>
          <h1 class="header-text"> Your education counselor. </h1>
        </span>
      </transition>
      <span class="subheader-container">
        <h2 class="subheader-text"> I help architect a personalised education blueprint for aspiring professionals like you. </h2>
        <h2 class="subheader-text"> Find out how I can help, I’d love to hear from you. </h2>
      </span>
      <CallToAction id="CallToAction"/>
      <MosaicTiles id="MosaicTiles"/>
      <BottomBar id="BottomBar"/>
    </div>
    <transition appear name="fade">
      <SideBar id="SideBar"/>
    </transition>
  </section>
</template>

<script>

import TopBar from "@/components/TopBar";
import MosaicTiles from "@/components/MosaicTiles";
import BottomBar from "@/components/BottomBar";
import SideBar from "@/components/SideBar";
import CallToAction from "@/components/CallToAction";

export default {
  name: "Home",
  components: {
    CallToAction,
    SideBar,
    BottomBar,
    MosaicTiles,
    TopBar
  }
}
</script>

<style lang="scss" scoped>

@import "/src/styles/animations.scss";

#Home{
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100vh;

  .main-wrapper{
    width: 74%;
    height: 96%;
    display: flex;
    flex-direction: column;
    align-items: center;

    .header-container{
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 600px;
      text-align: center;
      margin-top: 11vh;

      h1{
        margin: 0;
        font-family: "Bw Modelica Bold", serif;
        font-size: 37px;
        color: #1f1f1f;
        letter-spacing: -0.5px;
        line-height: 1.2;

        .highlight-name{
          color: #5675e7;
        }
      }
    }
    .subheader-container{
      padding-top: 12px;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: fit-content;
      text-align: center;

      h2{
        margin: 0;
        font-family: "Gilroy Light", serif;
        font-size: 14px;
        color: #1f1f1f;
        line-height: 1.7;
      }
    }
    #CallToAction{
      padding-top: 2vh;
      width: fit-content;
      height: fit-content;
      border: thin solid white;
    }
    #MosaicTiles{
      padding-top: 4vh;
      width: 62%;
      min-width: 650px;
      max-width: 700px;
      height: 280px;
    }
    #BottomBar{
      margin-top: auto;
    }
  }
  #SideBar{
    width: 24%;
    min-width: 320px;
    height: 93%;
    padding: 15px 0;
    margin: 0 15px;
  }
}

</style>