<script lang="ts">
import LoginForm from '../components/LoginForm.vue';
export default {
  data() {
    return {
      text: '',
    };
  },
  components: { LoginForm },
};
</script>
<template>
  <div class="wrapper">
    <div class="container">
      <div class="login-wrapper">
        <div class="col-sm-8">
          <LoginForm
            :title="'Ashfield Client Portal'"
            :description="'DEEP ROOTS, MODERN APPROACH'"
            :loginType="'Advisor Login'"
          />
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  height: 100%;
  width: 100%;
  background: url('../assets/cover-image.jpg') center bottom no-repeat fixed;
  background-color: #eee;
  background-size: cover !important;
  background-position: 50% !important;
}

.container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 auto;
  margin-top: -3rem;
}
.login-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
