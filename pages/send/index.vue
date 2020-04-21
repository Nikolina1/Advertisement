<template>
  <div class="send-page">
    <div class="first">
      <h1>You can fill the form and submit your ad here</h1>
    </div>
    <div class="second-form">
      <AdForm />
    </div>
  </div>
</template>

<script>
import AdForm from "@/components/Login/AdForm";
export default {
  components: {
    AdForm
  },
  head: {
    title: "Send"
  }
};
</script>


<style scoped>
.send-page {
  display: flex;
  align-items: center;
  background-image: url("~assets/images/bc.jpg");
}
.first {
  width: 50%;
}
.first h1 {
  font-size: 30px;
  color: #073b5e;
}
.second-form {
  text-align: center;
  justify-content: center;
  width: 50%;
  padding: 0px 20px 20px 20px;
}
</style>
