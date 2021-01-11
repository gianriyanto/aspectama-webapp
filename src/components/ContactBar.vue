<template>
  <div id="ContactBar">
    <div class="bar-container">
      <smartphone-icon size="1x" class="phone-icon"></smartphone-icon>
      <contact-inline-input id="ContactInlineInput" v-bind:inputData="contact"/>
      <button class="send-button" @click="sendContact">
        <span class="button-label">
          Keep in touch
        </span>
      </button>
    </div>
  </div>
</template>

<script>
import ContactInlineInput from "@/components/ContactInlineInput";
import { SmartphoneIcon } from 'vue-feather-icons'

export default {
  name: "ContactBar",
  components: {
    ContactInlineInput,
    SmartphoneIcon
  },
  data() {
    return {
      contact: {prompt: 'Contact phone or email', input: 'Contact phone or email', edit: false, isValid: false},
    }
  },
  methods: {
    sendContact() {
      console.log(this.contact.input);
    }
  }
}
</script>

<style lang="scss" scoped>

#ContactBar{
  display: flex;
  justify-content: center;

  .bar-container{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    height: 31px;
    width: 100%;
    border-radius: 30px;
    padding: 3px 3px 3px 15px;
    align-items: center;
    background-color: white;
    filter: drop-shadow(3px 6px 10px rgba(96, 88, 88, 0.3));

    .phone-icon{
      color: #a0a0a0;
    }
    #ContactInlineInput{
      flex-grow: 1;
      padding-left: 7px;
      padding-right: 13px;
    }
    .send-button{
      display: flex;
      text-decoration: none;
      outline: none;
      border: 0;
      height: 100%;
      width: 110px;
      background-image: linear-gradient(to right top, #2b2b2b, #2d2d2d);
      border-radius: 30px;
      cursor: pointer;
      transition: all .3s ease-in-out;

      .button-label{
        margin: auto;
        font-family: "Bw Modelica Medium", serif;
        font-size: 10px;
        color: white;
      }

      &:hover{
        opacity: 0.9;
      }
    }
  }
}

</style>