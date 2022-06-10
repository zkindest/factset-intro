<script lang="ts">
export default {};
</script>

<template>
  <header>
    <div class="container">
      <router-link to="/">
        <div class="logo">
          <img src="../assets/logo.png" alt="Logo desc" />
        </div>
      </router-link>
      <div class="menu">
        <button class="menu-item icon" aria-label="Help">
          <b-icon
            icon="question-circle-fill"
            variant="primary"
            font-scale="2"
          />
        </button>
        <button class="menu-item icon" aria-label="User Menu">
          <b-icon icon="person-circle" font-scale="2" />
        </button>
        <div class="menu-item">
          <b-button squared variant="primary">Client Login</b-button>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  background-color: white;
  padding: 1.5rem;
  margin-bottom: 5px;
  box-shadow: 0 2px 4px -1px rgb(0 0 0 / 20%), 0 4px 5px 0 rgb(0 0 0 / 14%),
    0 1px 10px 0 rgb(0 0 0 / 12%);
}

.container {
  display: flex;
  justify-content: space-between;
  gap: 1rem;
}
.logo {
  height: 100%;
}

img {
  max-height: 3rem;
  width: 100%;
  height: 100%;
  object-fit: fill;
  object-position: center;
}

.menu {
  display: inline-flex;
  align-items: center;
}

.menu-item {
  cursor: pointer;
  background-color: transparent;
  border: 0;
}

.menu-item + .menu-item {
  margin-left: 1rem;
}
</style>
