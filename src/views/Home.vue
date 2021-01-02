<template>
  <section id="Home">
    <div class="main-wrapper">


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
  width: 100vw;
  height: 100vh;
  border: thin solid blue;

  .main-wrapper {
    width: 70%;
    height: 95%;
    margin: auto;
    border: thin solid green;
  }

  .sidebar-wrapper{
    width: 25%;
    height: 95%;
    margin: auto;
    border: thin solid mediumpurple;
  }
}

</style>