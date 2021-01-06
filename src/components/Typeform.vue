<template>
  <div id="Typeform">
    <ProgramSelection id="ProgramSelection"/>
    <div class="input-card">
      <span class="prompt">
        Let's start with your name
      </span>
      <span class="input">
        <inline-input v-bind:inputData="name"/>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        You're most interested to study
      </span>
      <span class="input">
        <inline-input v-bind:inputData="course"/>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        And travel abroad to
      </span>
      <span class="input">
        <inline-input v-bind:inputData="country"/>
      </span>
    </div>
    <div class="input-card">
      <span class="prompt">
        Cool! It's best to reach you at
      </span>
      <span class="input">
        <inline-input v-bind:inputData="contact"/>
      </span>
    </div>
  </div>
</template>

<script>
import ProgramSelection from "@/components/ProgramSelection";
import InlineInput from "@/components/InlineInput";

export default {
  name: "Typeform",
  components: {
    InlineInput,
    ProgramSelection,
  },
  data() {
    return {
      program: "",
      name: {prompt: 'Your full name', input: 'Your full name', edit: false, isValid: false},
      course: {prompt: 'Interested major or course', input: 'Interested major or course', edit: false, isValid: false},
      country: {prompt: 'Preferred city or country?', input: 'Preferred city or country?', edit: false, isValid: false},
      contact: {prompt: 'Your mobile or email', input: 'Your mobile or email', edit: false, isValid: false},
    }
  }
}
</script>

<style lang="scss" scoped>

 #Typeform{
   display: flex;
   flex-direction: column;
   justify-content: flex-start;

   #ProgramSelection{
     height: 150px;
     width: 96%;
     margin-bottom: 1.7vh;
   }

   .input-card{
     align-self: center;
     margin-bottom: 1.7vh;
     display: flex;
     flex-direction: column;
     justify-content: space-evenly;
     padding: 9px 20px;
     width: 84%;
     height: 55px;
     border-radius: 10px;
     border: 1px solid rgba(112, 91, 91, 0.2);
     background-color: white;

     .prompt {
       font-family: "Bw Modelica Bold", serif;
       font-size: 13px;
       color: #4a4a4a;
     }
   }
 }

</style>