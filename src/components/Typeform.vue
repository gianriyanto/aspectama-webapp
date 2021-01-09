<template>
  <div id="Typeform">
    <ProgramSelection id="ProgramSelection" v-bind:selectionData="programs"/>

    <div class="input-card" v-bind:class="{'isvalid-border': name.isValid}">
      <span class="prompt">
        Let's start with your name
      </span>
      <span class="input">
        <inline-input v-bind:inputData="name"/>
      </span>
    </div>

    <div class="disabled-card" v-if="!name.isValid">
      <span class="prompt">
        You're most interested to study
      </span>
      <span class="input">
        Interested major or course
      </span>
    </div>
    <div class="input-card" v-else>
      <span class="prompt">
        You're most interested to study
      </span>
      <span class="input">
        <inline-input v-bind:inputData="course"/>
      </span>
    </div>

    <div class="disabled-card" v-if="!course.isValid || !name.isValid">
      <span class="prompt">
        And travel abroad to
      </span>
      <span class="input">
        Preferred city or country?
      </span>
    </div>
    <div class="input-card" v-else>
      <span class="prompt">
        And travel abroad to
      </span>
      <span class="input">
        <inline-input v-bind:inputData="country"/>
      </span>
    </div>

    <div class="disabled-card" v-if="!country.isValid || !course.isValid || !name.isValid">
      <span class="prompt">
        Cool! It's best to reach you at
      </span>
      <span class="input">
        Your mobile or email
      </span>
    </div>
    <div class="input-card" v-else>
      <span class="prompt">
        Cool! It's best to reach you at
      </span>
      <span class="input">
        <inline-input v-bind:inputData="contact"/>
      </span>
    </div>

    <div v-if="country.isValid && course.isValid && name.isValid && contact.isValid" class="footer-container">
      <span class="footer-text">
        Thanks {{ name.input.split(' ')[0] }}, chat soon!
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
      programs: [{programName: 'College Foundation', isSelected: false, imageURL:'team_work.svg'}, {programName: 'Under Graduate', isSelected: false, imageURL:'career_-2.svg'}, {programName: 'Post Graduate', isSelected: false, imageURL:'knowledge_.svg'} ],
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
     height: 160px;
     width: 100%;
     margin-bottom: 1.7vh;
   }

   .input-card{
     align-self: center;
     margin-bottom: 1.7vh;
     display: flex;
     flex-direction: column;
     justify-content: space-evenly;
     padding: 7px 20px;
     width: 86%;
     height: 62px;
     border-radius: 7px;
     border: 1px solid #dddddd;
     background-color: white;
     transition: all .4s ease-in-out;

     .prompt {
       font-family: "Bw Modelica Bold", serif;
       font-size: 14px;
       color: #434343;
     }
   }

   .isvalid-border{
     border: 1px solid #85cdbc;
   }

   .disabled-card{
     align-self: center;
     margin-bottom: 1.7vh;
     display: flex;
     flex-direction: column;
     justify-content: space-evenly;
     padding: 7px 20px;
     width: 86%;
     height: 62px;
     border-radius: 7px;
     border: 1px solid rgba(112, 91, 91, 0.1);
     background-color: white;
     opacity: 0.7;

     .prompt {
       font-family: "Bw Modelica Bold", serif;
       font-size: 14px;
       color: #d7d7d7;
     }

     .input{
       font-family: "Bw Modelica Regular", serif;
       font-size: 14px;
       color: #d7d7d7;
     }
   }

   .footer-container{
     padding-left: 5px;
     padding-top: 5px;
     display: flex;
     flex-direction: column;
     height: fit-content;

     .footer-text{
       font-family: "Bw Modelica Light", serif;
       font-size: 14px;
       color: #1f1f1f;
     }
   }
 }

</style>