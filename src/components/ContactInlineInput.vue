<template>
  <div id="ContactInlineInput">
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
      </div>
    </div>
  </div>
</template>

<script>

export default {
  field: "InlineInput",
  props: ['inputData'],
  components: {
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
        this.field.input = input;
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

#ContactInlineInput{
  font-family: "Bw Modelica Medium", serif;
  font-size: 13px;

  .input-editing{
    font-family: "Bw Modelica Medium", serif;
    font-size: 13px;
    color: #5f5f5f;
    width: 100%;
    border: none;
    outline: none;
  }

  .input-card{
    display: flex;
    flex-direction: row;
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