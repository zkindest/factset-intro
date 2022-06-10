<script lang="ts">
export default {
  props: {
    title: String,
    description: String,
    loginType: {
      type: String,
      default: 'Advisor Login',
    },
  },
};
</script>
<template>
  <div class="login">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <form>
      <div class="mb-4">
        <label for="email">Email/Username</label>
        <b-form-input
          id="email"
          v-model="id"
          type="text"
          max="200"
          placeholder="Enter Email or Username"
        >
        </b-form-input>
      </div>
      <div class="mb-4">
        <label for="password">Pasword</label>
        <b-form-input
          id="password"
          v-model="password"
          type="password"
          min="6"
          max="15"
          placeholder="Enter Pasword"
        >
        </b-form-input>
      </div>
      <b-button squared variant="primary" class="w-100">
        {{ loginType }}</b-button
      >
    </form>
  </div>
</template>

<style scoped>
h1,
p {
  text-align: center;
}
.login {
  width: 100%;
  background-color: var(--color-gray);
  padding: 1.5rem 1.5rem 3rem;
}
form {
  width: 100%;
  margin: 0 auto;
}
@media (min-width: 768px) {
  form {
    width: 60%;
  }
}
@media (max-width: 768px) {
  h1 {
    font-size: 1.2rem;
  }
  p {
    font-size: 0.8rem;
  }
}
</style>
