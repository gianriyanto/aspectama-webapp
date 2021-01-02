<template>
  <section id="Home">
    <div class="main-wrapper">
      <TopBar id="TopBar"/>
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
  }

  .sidebar-wrapper{
    width: 26%;
    height: 95%;
    border: thin solid mediumpurple;
  }
}

</style>