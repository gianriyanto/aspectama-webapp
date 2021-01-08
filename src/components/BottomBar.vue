<template>
  <div id="BottomBar">
    <SocialLinks/>
    <ContactDetails/>
  </div>
</template>

<script>
import SocialLinks from "@/components/SocialLinks";
import ContactDetails from "@/components/ContactDetails";
export default {
  name: "BottomBar",
  components: {
    ContactDetails,
    SocialLinks
  }
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
    width: 100px;
  }

  #ContactDetails{
    width: 290px;
  }
}

</style>