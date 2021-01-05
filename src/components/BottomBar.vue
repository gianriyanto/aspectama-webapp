<template>
  <div id="BottomBar">
    <SocialLinks/>
  </div>
</template>

<script>
import SocialLinks from "@/components/SocialLinks";
export default {
  name: "BottomBar",
  components: {SocialLinks}
}
</script>

<style lang="scss" scoped>

#BottomBar{
  width: 95%;
  height: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  #SocialLinks {

  }
}

</style>