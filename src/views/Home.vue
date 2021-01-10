<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
      <transition appear name="fade">
        <span class="header-container">
          <h1 class="header-text"> {{ header[0] }} </h1>
          <h1 class="header-text"> {{ header[1] }} </h1>
        </span>
      </transition>
      <span class="subheader-container">
        <h2 class="subheader-text"> {{ subheader[0] }} </h2>
        <h2 class="subheader-text"> {{ subheader[1] }} </h2>
      </span>
      <ContactBar id="ContactBar"/>
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
      header: ["Hello! I'm Ervina", "your education counselor."],
      subheader: ["I help architect a personalised education blueprint for aspiring professionals like you.", "Find out how I can help, I’d love to hear from you."]
    }
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
    margin-right: 0px;

    .header-container{
      padding-top: 10vh;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 600px;
      text-align: center;

      h1{
        margin: 0;
        font-family: "Bw Modelica Bold", serif;
        font-size: 37px;
        color: #1f1f1f;
        letter-spacing: -0.5px;
        line-height: 1.1;
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
    #ContactBar{
      padding-top: 2vh;
      width: 390px;
      height: fit-content;
    }
    #MosaicTiles{
      padding-top: 5vh;
      width: 62%;
      min-width: 650px;
      max-width: 770px;
      height: 310px;
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