<template>
  <!--First section -->
  <div class="bg-cover bg-custom-bg bg-center mx-20 mt-4 rounded-xl max-h-80 ">
    <div class="text-center">
      <span class="font-bold lg:text-6xl text-Text sm:text-xl sm:flex-wrap sm:text-wrap ">Kampuni Ekulembeddemu mu by’Okusengula mu Uganda</span>
    </div>

    <!-- Button   -->
    <div class="text-center">
      <button class="bg-Primary text-black font-bold text-white sm:text-sm mt-24 my-20 rounded-full px-4 py-3">
        FUNA QUOTE YA BWEREERE -->
      </button>
    </div>
  </div>

  <!-- Video section -->

  <div class="bg-Primary mx-20 my-4 rounded-xl">
    <div class="text-white text-center pt-4">
      <span class="text-6xl font-bold font-mono sm:text-xl">Fine Moving</span> <br>
      <span class="font-bold">Funa akabonero ku bumanyirivu bwa Nellion</span>
    </div>
    <div class="px-10 py-6">
      <iframe src="https://www.youtube.com/embed/5hztbtl0BY0"
              title="Professional House Shifting in Uganda with Nellions"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              referrerpolicy="strict-origin-when-cross-origin" allowfullscreen
              class="h-[350px] w-[80%] lg:hidden flex mx-auto mb-2 rounded "></iframe>
    </div>
  </div>
  <!-- Two column section-->
  <div class="flex flex-row px-20">
    <!--    image column  -->
    <div class="flex-1 py-20 px-4">
      <img
          src="/assets/images/bg-1.png"
          alt="No image detected"
          class="">
    </div>
    <!--    Text column-->
    <div class="flex-1 py-48 ">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet corporis dolor inventore, nam odio sequi
        similique soluta tempore veritatis vero! Accusantium commodi consequuntur exercitationem, iusto minima porro
        quibusdam reiciendis ullam.
      </p>
    </div>

  </div>

<!--  Slider-->
  <Swiper/>

<!--  FAQ-->
  <FAQ/>

<!-- Contact us -->

  <Contact/>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import FAQ from "~/components/FAQ.vue";

const count = ref(0)
</script>


