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
    </div>
    <div class="sidebar-wrapper">

    </div>
  </section>
</template>

<script>

import TopBar from "@/components/TopBar";

export default {
  name: "Home",
  components: {
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
  border: thin solid blue;

  .main-wrapper{
    width: 68%;
    height: 95%;
    border: thin solid green;
    padding-right: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;

    .header-container{
      padding-top: 100px;
      display: flex;
      flex-direction: column;
      height: fit-content;
      width: 500px;
      text-align: center;

      h1{
        margin: 0;
        font-family: "Gilroy SemiBold", serif;
        font-size: 44px;
        color: black;
        letter-spacing: 0;
        line-height: 1.1;
      }
    }
  }

  .sidebar-wrapper{
    width: 26%;
    height: 95%;
    border: thin solid mediumpurple;
  }
}

</style>