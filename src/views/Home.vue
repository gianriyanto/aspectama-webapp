<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
      <transition appear name="fade">
        <span class="header-container">
          <span class="header-text"> Hi! I'm <span class="highlight-name"> Ervina. </span> </span>
          <span class="header-text"> Your education counselor. </span>
        </span>
      </transition>
      <span class="subheader-container">
        <h2 class="subheader-text-0"> I help architect a personalised education blueprint for aspiring professionals like you. </h2>
        <h2 class="subheader-text-1"> Find out how I can help, I’d love to hear from you. </h2>
      </span>
      <CallToAction id="CallToAction"/>
      <MosaicTiles id="MosaicTiles"/>
      <BottomBar id="BottomBar"/>
    </div>
    <transition appear name="fade">
      <SideBar id="SideBar"/>
    </transition>
    <BottomBar id="BottomBarMobile" />
    <FloatingActionButton id="FloatingActionButton"/>
  </section>
</template>

<script>

import TopBar from "@/components/TopBar";
import MosaicTiles from "@/components/MosaicTiles";
import BottomBar from "@/components/BottomBar";
import SideBar from "@/components/SideBar";
import CallToAction from "@/components/CallToAction";
import FloatingActionButton from "@/components/FloatingActionButton";

export default {
  name: "Home",
  components: {
    FloatingActionButton,
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

@media only screen and (min-width: 769px) {
  #Home {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    width: 100vw;
    height: 100vh;

    .main-wrapper {
      width: 74%;
      height: 96%;
      display: flex;
      flex-direction: column;
      align-items: center;

      #TopBar {

      }

      .header-container {
        display: flex;
        flex-direction: column;
        height: fit-content;
        width: 600px;
        text-align: center;
        margin-top: 11vh;

        .header-text {
          margin: 0;
          font-family: "Bw Modelica Bold", serif;
          font-size: 37px;
          color: #1f1f1f;
          letter-spacing: -0.5px;
          line-height: 1.2;

          .highlight-name {
            color: #5675e7;
          }
        }
      }

      .subheader-container {
        padding-top: 12px;
        display: flex;
        flex-direction: column;
        height: fit-content;
        width: fit-content;
        text-align: center;

        .subheader-text-0, .subheader-text-1 {
          margin: 0;
          font-family: "Gilroy Light", serif;
          font-size: 14px;
          color: #1f1f1f;
          line-height: 1.7;
        }
      }

      #CallToAction {
        padding-top: 2vh;
        width: fit-content;
        height: fit-content;
        border: thin solid white;
      }

      #MosaicTiles {
        padding-top: 4vh;
        width: 62%;
        min-width: 650px;
        max-width: 700px;
        height: 260px;
      }

      #BottomBar {
        margin-top: auto;
      }
    }

    #SideBar {
      width: 24%;
      min-width: 320px;
      height: 93%;
      padding: 15px 0;
      margin: 0 15px;
    }
  }
  #FloatingActionButton{
    display: none;
  }
}

@media only screen and (max-width: 768px) {

  #Home{
    display: flex;
    flex-direction: column;
    height: fit-content;

    #TopBar{
      margin-top: 10vh;
    }

    .header-container{
      margin: 5vh auto 0;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 98%;
      text-align: center;

      .header-text{
        margin: 0;
        font-family: "Bw Modelica Bold", serif;
        font-size: 24px;
        color: #1f1f1f;
        letter-spacing: -0.5px;
        line-height: 1.3;

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
      width: 80%;
      margin: 0 auto;
      text-align: center;

      .subheader-text-0{
        margin: 0;
        font-family: "Gilroy Light", serif;
        font-size: 15px;
        color: #1f1f1f;
        line-height: 1.7;
      }
      .subheader-text-1{
        margin: 0;
        font-family: "Gilroy Light", serif;
        font-size: 15px;
        color: #1f1f1f;
        line-height: 1.7;
      }
    }

    #CallToAction{
      padding-top: 4vh;
      width: 90%;
      height: 40vh;
      margin: 0 auto;
    }

    #MosaicTiles{
      padding-top: 3vh;
      padding-bottom: 2vh;
    }

    #BottomBar{
      display: none;
    }
  }
  #SideBar{
    width: 93%;
    height: fit-content;
    padding: 15px 0;
    margin: 0 auto 9vh auto;
  }

  #BottomBarMobile{
    margin: 0 auto;
  }
  #FloatingActionButton{

  }
}

</style>