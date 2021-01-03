<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
      <span class="header-container">
        <h1 class="header-text">
          Hello, I'm Ervina, an
        </h1>
        <h1 class="header-text">
          education consultant.
        </h1>
      </span>
      <span class="subheader-container">
        <h2 class="subheader-text">
          I help craft a tailored education blueprint for aspiring professionals. Find out how I can help, I’d love to hear from you.
        </h2>
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
      width: 500px;
      text-align: center;

      h1{
        margin: 0;
        font-family: "Gilroy SemiBold", serif;
        font-size: 44px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.1;
      }
    }
    .subheader-container{
      padding-top: 5px;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 530px;
      text-align: center;

      h2{
        margin: 0;
        font-family: "Bw Modelica Light", serif;
        font-size: 14px;
        color: #1f1f1f;
        letter-spacing: 0;
        line-height: 1.7;
      }
    }
    #ContactBar{
      padding-top: 20px;

    }
    #MosaicTiles{
      padding-top: 20px;
    }
    #BottomBar{
      margin-top: auto;
    }
  }

  #SideBar{
    width: 26%;
    height: 96%;
    border-radius: 12px;
    background-color: white;
    box-shadow: 0 10px 30px 1px rgba(73, 74, 95, 0.2);
  }
}

</style>