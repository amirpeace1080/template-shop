<template>
  <div>
    <Header />
    <Slider />

    <v-container class="mt-3 mb-3">
      <v-row>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/d0dc31c892be8cf1408e4e14580b3f479da66bd1_1648897133.png"
          />
          <p class="subtitle-pic">دیجی کالا جت</p>
        </v-col>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/3317332ca672c49f8c7eae60e64ad511005e4660_1655015357.png"
          />
          <p class="subtitle-pic">دیجی استایل</p>
        </v-col>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/ac127167132653d14c758748b07824a6a7643a31_1648897095.png"
          />
          <p class="subtitle-pic">دیجی پی</p>
        </v-col>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/17bb6daa07ae2ec11867fb7320ed6f79b26f1f4b_1648897081.png"
          />
          <p class="subtitle-pic">دیجی کالا مهر</p>
        </v-col>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/967cbaa25713ca4d0e58cb5aaf0e486ab986d460_1648898393.png"
          />
          <p class="subtitle-pic">ماموریت ها</p>
        </v-col>
        <v-col lg="2" cols="3">
          <v-img
            width="52"
            height="52"
            src="https://dkstatics-public.digikala.com/digikala-bellatrix/78ccd40cbf305fb067de78ddab5be84f69589c8d_1648897009.png"
          />
          <p class="subtitle-pic">دیجی پلاس</p>
        </v-col>
      </v-row>
    </v-container>

    <NewItems class="mt-5 mb-5" />

    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Slider from "@/components/Slider.vue";
import NewItems from "@/components/NewItems.vue";
import Footer from '@/components/Footer.vue'

export default {
  name: "Home",

  components: {
    Header,
    Slider,
    NewItems,
    Footer,
  },
};
</script>

<style scoped>
.subtitle-pic {
  font-size: 11px;
  font-weight: 700;
  line-height: 24px;
}
</style>
