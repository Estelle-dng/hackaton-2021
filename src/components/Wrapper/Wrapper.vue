<template>
  <div id="main-wrapper">
    <slot />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
#main-wrapper {
  padding: 0 120px;
  @media (max-width: 900px) {
    padding: 0 60px;
  }
  @media (max-width: 550px) {
    padding: 0 10px;
  }
}
</style>
