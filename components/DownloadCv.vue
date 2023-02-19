<template>
  <button class="btn">دانلود رزومه</button>
</template>
<script>
export default {}
</script>
<style lang="scss" scoped>
.btn {
  height: 35px;
  width: 80px;
  font-size: 12px;
  font-weight: 500;
  background: $red-color;
  color: $white;
  border-radius: 6px;
  border: none;
  cursor: pointer;
  @include media(md) {
    font-size: 14px;
    height: 40px;
    width: 100px;
  }
}
</style>
