<template>
  <form @submit.prevent="onSave">
    <AppControlInput v-model="author">Full name</AppControlInput>
    <AppControlInput v-model="ad">Name of the ad</AppControlInput>
    <AppControlInput control-type="textarea" v-model="description">Ad description</AppControlInput>
    <AppControlInput control-type="textarea" v-model="addition">Additional details</AppControlInput>
    <AppButton type="submit">Save</AppButton>
    <AppButton type="button" style="margin-left: 10px" btn-style="cancel" @click="onCancel">Cancel</AppButton>
  </form>
</template>

<script>
import AppControlInput from "@/components/UI/AppControlInput";
import AppButton from "@/components/UI/AppButton";

export default {
  name: "AdForm",
  components: {
    AppControlInput,
    AppButton
  },

  methods: {
    onSave() {
      this.$emit("submit");
    },
    onCancel() {
      this.$router.push("/");
    }
  }
};
</script>

<style scoped>
</style>

