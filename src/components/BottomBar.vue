<template>
  <div>
    <div id="BottomBar">
      <SocialLinks/>
      <ContactDetails/>
    </div>
    <div id="BottomBarMobile">
      <SocialLinks/>
      <ContactDetails/>
    </div>
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

@media only screen and (min-width: 768px) {
  #BottomBar {
    width: 95%;
    height: 30px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    #SocialLinks {
      width: 90px;
    }

    #ContactDetails {
      width: 290px;
    }
  }

  #BottomBarMobile {
    display: none;
  }
}

@media only screen and (max-width: 768px) {

  #BottomBar{
    display: none;
  }

  #BottomBarMobile {
    width: 95%;
    height: 30px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    border: thin solid hotpink;

    #SocialLinks {
      width: 90px;
    }

    #ContactDetails {
      width: 290px;
    }
  }
}

</style>