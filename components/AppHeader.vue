<template>
  <header>
    <RouterLink to="/" class="title">
      <img class="logo" src="~assets/icon.svg" alt="logo">
    </RouterLink>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
header {
  position: fixed;
  left: 0;
  top: 0;
  height: 48px;
  background: #fff;
  z-index: 9999;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 0 2px rgba(0, 0, 0, 0.25);
}
@supports (
  (-webkit-backdrop-filter: blur(4px)) or (backdrop-filter: blur(4px))
) {
  header {
    background-color: rgba(255, 255, 255, 0.5);
    -webkit-backdrop-filter: blur(4px);
    backdrop-filter: blur(4px);
  }
}
.title {
  text-decoration: none;
}
.logo {
  width: 32px;
  height: 32px;
}
</style>
