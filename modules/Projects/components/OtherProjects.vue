<template>
  <div :class="$style.samples">
    <sliderBox :data="data" :options="options" />
  </div>
</template>
<script lang="ts" setup>
  import {ref} from 'vue';
  import sliderBox from '@ui/components/SliderBox/Main.vue';
  import {useProjects} from '@modules/Home/controller/composables/projects';
  const {data} = useProjects();

  const options = ref({
    slidesPerView: '4',
    breakpoints: {
      320: {
        slidesPerView: 1,
        spaceBetween: 20
      },

      768: {
        slidesPerView: 2,
        spaceBetween: 30
      },
      1024: {
        slidesPerView: 3,
        spaceBetween: 30
      },
      1600: {
        slidesPerView: 4,
        spaceBetween: 30
      }
    }
  });
</script>
<style lang="scss" module>
  .samples {
    padding: 0 10px;
  }
</style>
