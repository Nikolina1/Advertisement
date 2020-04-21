<template>
  <button class="button" :class="btnStyle" v-bind="$attrs" v-on="$listeners">
    <slot />
  </button>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    btnStyle: {
      type: String,
      default: ""
    }
  }
};
</script>


<style scoped>
.button {
  font: inherit;
  background-color: #073b5e;
  color: rgb(252, 253, 253);
  padding: 5px;
  cursor: pointer;
  border: 1px solid black;
  font-weight: 500;
}

.button:hover,
.button:active {
  background-color: rgb(119, 131, 146);
  border: 1px solid #073b5e;
}

.inverted {
  background-color: #073b5e;
  color: rgb(248, 245, 245);
  border: 1px solid transparent;
}

.inverted:hover,
.inverted:active {
  color: rgb(250, 243, 243);
  background-color: rgb(119, 131, 146);
  border: 1px solid transparent;
}

.cancel {
  background-color: #073b5e;
  color: rgb(255, 255, 255);
  border: 1px solid transparent;
}

.cancel:hover,
.cancel:active {
  background-color: rgb(119, 131, 146);
  border: 1px solid transparent;
}
</style>
