<template>
  <div class="wrapper">
    <div class="content">
      <div class="title">سپهر ضرغامی | توسعه دهنده وب</div>
      <div class="text">
        لورم ایپسوم یا طرح‌نما (به انگلیسی: Lorem ipsum) به متنی آزمایشی و
        بی‌معنی در صنعت چاپ، صفحه‌آرایی و طراحی گرافیک گفته می‌شود. طراح گرافیک
        از این متن به عنوان عنصری از ترکیب بندی برای پر کردن صفحه و ارایه اولیه
        شکل ظاهری و کلی طرح سفارش گرفته شده استفاده می نماید، تا از نظر گرافیکی
        نشانگر چگونگی نوع و اندازه فونت و ظاهر متن باشد. معمولا طراحان گرافیک
        برای صفحه‌آرایی، نخست از متن‌های آزمایشی و بی‌معنی استفاده می‌کنند تا
        صرفا به مشتری یا صاحب کار خود نشان دهند که صفحه طراحی یا صفحه بندی شده
        بعد از اینکه متن در آن قرار گیرد چگونه به نظر می‌رسد و قلم‌ها و
        اندازه‌بندی‌ها چگونه در نظر گرفته
      </div>
      <div class="cv">
        <DownloadCV />
      </div>
    </div>
    <Social />
  </div>
</template>

<script>
import Social from './SocialMedia.vue'
import DownloadCV from './DownloadCv.vue'
export default {
  name: 'Index',
  components: {
    Social,
    DownloadCV,
  },
}
</script>
<style lang="scss">
.wrapper {
  background: url(~/assets/images/img/Home/bg.jpg) top center no-repeat;
  background-size: auto 100%;
  height: 100vh;
  position: relative;
}
.content {
  padding: 25% 0 0;
  width: 100%;
  color: white;
  @include media(md) {
    width: 50%;
    padding: 100px 25px 0;
  }
  .title {
    font-size: 22px;
    margin-bottom: 10px;
    word-spacing: -3px;
    font-weight: bold;
    padding-right: 16px;
    @include media(md) {
      margin-bottom: 20px;
      font-size: 30px;
    }
  }
  .text {
    word-spacing: -3px;
    font-size: 16px;
    font-weight: 500;
    line-height: 30px;
    text-align: justify;
    height: 50vh;
    overflow: hidden;
    overflow-y: auto;
    padding: 0 16px;
    @include media(md) {
      height: 250px;
      line-height: 35px;
      font-size: 20px;
    }
  }
  .cv {
    width: 100%;
    text-align: center;
  }
}
</style>
