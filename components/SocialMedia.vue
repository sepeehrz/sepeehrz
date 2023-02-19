<template>
  <div class="social">
    <a href="/" class="social-item">
      <i class="lab la-instagram"></i>
    </a>
    <a href="/" class="social-item">
      <i class="lab la-telegram"></i>
    </a>
    <a href="/" class="social-item">
      <i class="lab la-github"></i>
    </a>
    <a href="/" class="social-item">
      <i class="lab la-linkedin"></i>
    </a>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.social {
  position: absolute;
  bottom: 10%;
  left: 50%;
  transform: translateX(-50%);
  color: #fff;
  width: 80%;
  display: flex;
  justify-content: space-between;

  i {
    color: #fff;
    font-size: 50px;
  }
  @include media(md) {
    bottom: 20%;
    width: 50%;
  }
}
</style>
