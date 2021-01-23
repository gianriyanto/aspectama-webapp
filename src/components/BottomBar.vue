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
  },
}
</script>

<style lang="scss" scoped>

@media only screen and (min-width: 769px) {

  #BottomBar {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    #SocialLinks {
      width: 110px;
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
    height: fit-content;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;

    #SocialLinks {
      width: 60%;
      margin-bottom: 4vh;
    }

    #ContactDetails {
      width: 100%;
      margin-bottom: 8vh;
    }
  }
}

</style>