<template>
  <div id="InlineInput">
    <label v-if="field.edit">
      <input
          class="input-editing"
          v-model="field.input"
          v-on:blur="field.edit=false; onChangeText(field.input); $emit('update')"
          v-on:keyup.enter="$event.target.blur()"
          v-focus>
    </label>
    <div v-else class="input-card">
      <div :class="applyInputStyle(field.input)">
        <label @click="onEditText"> {{field.input}} </label>
        <check-circle-icon size="1x" class="check-icon"></check-circle-icon>
      </div>
    </div>
  </div>
</template>

<script>
import { CheckCircleIcon } from 'vue-feather-icons'

export default {
  field: "InlineInput",
  props: ['inputData'],
  components: {
    CheckCircleIcon,
  },
  data() {
    return {
      field: this.inputData,
    }
  },
  methods: {
    onEditText: function() {
      this.field.input = '';
      this.field.edit = true;
    },
    onChangeText: function(input) {
      //check if name input is valid
      if (input === '') {
        this.field.input = this.field.prompt;
        this.field.edit = false;
        this.field.isValid = false;
      } else {
        this.field.input = input.charAt(0).toUpperCase() + input.slice(1);
        this.field.isValid = true;
      }
    },
    applyInputStyle: function(input) {
      return [(input.length>0 && input !== this.field.prompt) ? 'input-has-value-style' : 'input-no-value-style']
    }
  },
  directives: {
    focus: {
      inserted (el) {
        el.focus()
      }
    }
  }
}
</script>

<style lang="scss" scoped>

#InlineInput{
  font-family: "Bw Modelica Regular", serif;
  font-size: 13px;

  .input-editing{
    font-family: "Bw Modelica Regular", serif;
    font-size: 13px;
    color: #5f5f5f;
    width: 98%;
    border: transparent;
    outline: transparent;
    background-color: transparent;
    border-bottom: thin solid #7eb1dd;
  }

  .input-card{
    display: flex;
    flex-direction: row;
  }
  .check-icon{
    padding-left: 3px;
    transform: translateY(2px);
    font-size: 13px;
    color: #16a075;
  }
  .input-has-value-style{
    color: #458fcf;
  }
  .input-no-value-style{
    color: darkgrey;
    width: fit-content;
  }
}

</style>