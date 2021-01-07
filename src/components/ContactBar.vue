<template>
  <div id="ContactBar">
    <div class="bar-container">
      <contact-inline-input class="input-field" v-bind:inputData="contact"/>
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

export default {
  name: "ContactBar",
  components: {
    ContactInlineInput,
  },
  data() {
    return {
      contact: {prompt: 'Your contact phone or email', input: 'Your contact phone or email', edit: false, isValid: false},
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
    height: 36px;
    width: 100%;
    border-radius: 50px;
    padding: 3px 3px 3px 25px;
    align-items: center;
    background-color: white;
    box-shadow: 0 5px 25px 1px rgba(77, 79, 109, 0.2);

    .input-field{
      flex-grow: 1;
      padding-right: 13px;
    }
    .send-button{
      display: flex;
      text-decoration: none;
      outline: none;
      border: 0;
      height: 100%;
      width: 120px;
      background-color: #1f1f1f;
      border-radius: 32px;
      cursor: pointer;
      transition: all .3s ease-in-out;

      .button-label{
        margin: auto;
        font-family: "Bw Modelica Medium", serif;
        font-size: 11px;
        color: white;
      }

      &:hover{
        opacity: 0.9;
      }
    }
  }
}

</style>