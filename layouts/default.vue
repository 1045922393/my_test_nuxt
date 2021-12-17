<template>
  <div>
    <h2>这是在layout下面的通用布局</h2>
    <div class="flex_layout">
      <nuxt class="flex_left"></nuxt>
      <div class="flex_right"></div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.flex_layout {
  display: flex;
}

.flex_left {
  flex: 1;
}

.flex_right {
  flex: 0 0 200px;
  height: 500px;
  background-color: papayawhip;
}
</style>
